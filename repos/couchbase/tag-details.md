<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `couchbase`

-	[`couchbase:6.0.5`](#couchbase605)
-	[`couchbase:6.5.2`](#couchbase652)
-	[`couchbase:6.6.5`](#couchbase665)
-	[`couchbase:7.0.3`](#couchbase703)
-	[`couchbase:community`](#couchbasecommunity)
-	[`couchbase:community-6.6.0`](#couchbasecommunity-660)
-	[`couchbase:community-7.0.2`](#couchbasecommunity-702)
-	[`couchbase:enterprise`](#couchbaseenterprise)
-	[`couchbase:enterprise-6.0.5`](#couchbaseenterprise-605)
-	[`couchbase:enterprise-6.5.2`](#couchbaseenterprise-652)
-	[`couchbase:enterprise-6.6.5`](#couchbaseenterprise-665)
-	[`couchbase:enterprise-7.0.3`](#couchbaseenterprise-703)
-	[`couchbase:latest`](#couchbaselatest)

## `couchbase:6.0.5`

```console
$ docker pull couchbase@sha256:f9235779854daa0f5086cab8643b04edb9174778022a013046d0ec431d435af6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `couchbase:6.0.5` - linux; amd64

```console
$ docker pull couchbase@sha256:50306e689ca3d28bc4cf08a63cde4130f3fb7899f746b6765948655220ab179a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **466.1 MB (466120858 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d7ea04df160ef1266c43115c9be766670952aa17848dd497dd9ba8ebec92704`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Fri, 29 Apr 2022 23:20:51 GMT
ADD file:f657a56a18426c3a88d620a7024e7b91424d926e7b47faa6a97c2369c4c4a228 in / 
# Fri, 29 Apr 2022 23:20:51 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 00:11:49 GMT
LABEL maintainer=docker@couchbase.com
# Sat, 30 Apr 2022 00:14:34 GMT
RUN set -x &&     apt-get update &&     apt-get install -yq runit wget chrpath tzdata man     lsof lshw sysstat net-tools numactl python-httplib2 &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Sat, 30 Apr 2022 00:14:35 GMT
RUN if [ ! -x /usr/sbin/runsvdir-start ]; then         cp -a /etc/runit/2 /usr/sbin/runsvdir-start;     fi
# Sat, 30 Apr 2022 00:14:35 GMT
ARG CB_VERSION=6.0.5
# Sat, 30 Apr 2022 00:14:35 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.5
# Sat, 30 Apr 2022 00:14:35 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_6.0.5-ubuntu18.04_amd64.deb
# Sat, 30 Apr 2022 00:14:35 GMT
ARG CB_SHA256=6b152590867a58d771cffc22774d3cd66c916defcbeeeb339aca8d0a8e6d7f8d
# Sat, 30 Apr 2022 00:14:35 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Sat, 30 Apr 2022 00:14:36 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.5-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.5 CB_SHA256=6b152590867a58d771cffc22774d3cd66c916defcbeeeb339aca8d0a8e6d7f8d CB_VERSION=6.0.5
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Sat, 30 Apr 2022 00:15:31 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.5-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.5 CB_SHA256=6b152590867a58d771cffc22774d3cd66c916defcbeeeb339aca8d0a8e6d7f8d CB_VERSION=6.0.5
RUN set -x &&     export INSTALL_DONT_START_SERVER=1 &&     wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE &&     echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - &&     apt-get update &&     apt-get install -y ./$CB_PACKAGE &&     rm -f ./$CB_PACKAGE &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Sat, 30 Apr 2022 00:15:33 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.5-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.5 CB_SHA256=6b152590867a58d771cffc22774d3cd66c916defcbeeeb339aca8d0a8e6d7f8d CB_VERSION=6.0.5
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Sat, 30 Apr 2022 00:15:34 GMT
COPY file:d6a307209223b2df102f46f07fd186e09fac7114db2c965bb54097d3b4d3b989 in /etc/service/couchbase-server/run 
# Sat, 30 Apr 2022 00:15:34 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.5-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.5 CB_SHA256=6b152590867a58d771cffc22774d3cd66c916defcbeeeb339aca8d0a8e6d7f8d CB_VERSION=6.0.5
RUN mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Sat, 30 Apr 2022 00:15:34 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Sat, 30 Apr 2022 00:15:35 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.5-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.5 CB_SHA256=6b152590867a58d771cffc22774d3cd66c916defcbeeeb339aca8d0a8e6d7f8d CB_VERSION=6.0.5
RUN ln -s dummy.sh /usr/local/bin/iptables-save &&     ln -s dummy.sh /usr/local/bin/lvdisplay &&     ln -s dummy.sh /usr/local/bin/vgdisplay &&     ln -s dummy.sh /usr/local/bin/pvdisplay
# Sat, 30 Apr 2022 00:15:35 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.5-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.5 CB_SHA256=6b152590867a58d771cffc22774d3cd66c916defcbeeeb339aca8d0a8e6d7f8d CB_VERSION=6.0.5
RUN chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl
# Sat, 30 Apr 2022 00:15:35 GMT
COPY file:d816a67f62bfba76d2812cefbe92252afa13f3852775c3e68599df7741e90cb7 in / 
# Sat, 30 Apr 2022 00:15:36 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 30 Apr 2022 00:15:36 GMT
CMD ["couchbase-server"]
# Sat, 30 Apr 2022 00:15:36 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Sat, 30 Apr 2022 00:15:36 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:40dd5be53814ae70b2898558673b7ea18d58bf7ab3433560b9ce3cb76d9ff0b1`  
		Last Modified: Fri, 29 Apr 2022 23:22:07 GMT  
		Size: 26.7 MB (26709108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfde595bbf77f9f882becea2554e11fb68bdc2ed67be2a0ca3ab93b2a8e49cff`  
		Last Modified: Sat, 30 Apr 2022 00:20:34 GMT  
		Size: 15.9 MB (15918912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84ccb59dfcda9556def1bbc8283f1b7be19631589f0de035ea23199f268989d3`  
		Last Modified: Sat, 30 Apr 2022 00:20:30 GMT  
		Size: 266.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b01d393883f27c086d6a93ba060675ed40ba156c338021fbd72cbb042964946f`  
		Last Modified: Sat, 30 Apr 2022 00:20:30 GMT  
		Size: 2.0 KB (1963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df4708548cc8ecbed1cf773a42f051e67ce079acd1944b258867e33694149dd7`  
		Last Modified: Sat, 30 Apr 2022 00:21:08 GMT  
		Size: 423.4 MB (423362799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25a8fd04a156e32ac4f2707e165ebd41bce031579e4783441827035be8161f9c`  
		Last Modified: Sat, 30 Apr 2022 00:20:30 GMT  
		Size: 191.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b7fdf4876c37245db240610b6f3d33f87c19ff3e646bee18aba32a5c19c51fd`  
		Last Modified: Sat, 30 Apr 2022 00:20:29 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d72c4626e9476266400aadcd452aac6347e688f6087408c114658be387923c1`  
		Last Modified: Sat, 30 Apr 2022 00:20:27 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b2c636e83d08d0f38eebb344b4c6b927e2c10d09ac74f779efb17024bb6546c`  
		Last Modified: Sat, 30 Apr 2022 00:20:27 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79b854237426234651c46a8b651e9321ac0869dea0e44542c8ab27db12759805`  
		Last Modified: Sat, 30 Apr 2022 00:20:27 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbe47a9e327ff459ffe2c301941c92c6e831dafd5bea18d6c5d77c8bc4d7432f`  
		Last Modified: Sat, 30 Apr 2022 00:20:27 GMT  
		Size: 125.6 KB (125556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d86e5a98e04b278372888fbd0d911c838374b6b3bb50a42a672ac4813a4f8fde`  
		Last Modified: Sat, 30 Apr 2022 00:20:28 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchbase:6.5.2`

```console
$ docker pull couchbase@sha256:4e19cf0e5ec5f0c57e0bc44d9170ac011243a1fc9cc37a0ebd0362d8dd0bc4ac
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `couchbase:6.5.2` - linux; amd64

```console
$ docker pull couchbase@sha256:b8f43ad49a00b04e0a670b530cdad2633c97add377dddca10ab235d21a694d5f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **503.8 MB (503759986 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90f3c9f7ee3c535ad7673a245614a05f9ab4ced807cc3a3a2aaf4815fd2253aa`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Fri, 29 Apr 2022 23:20:51 GMT
ADD file:f657a56a18426c3a88d620a7024e7b91424d926e7b47faa6a97c2369c4c4a228 in / 
# Fri, 29 Apr 2022 23:20:51 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 00:11:49 GMT
LABEL maintainer=docker@couchbase.com
# Sat, 30 Apr 2022 00:15:40 GMT
ARG UPDATE_COMMAND=apt-get update -y -q
# Sat, 30 Apr 2022 00:15:40 GMT
ARG CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Sat, 30 Apr 2022 00:15:49 GMT
# ARGS: CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ${UPDATE_COMMAND}     && apt-get install -y -q wget tzdata       lsof lshw sysstat net-tools numactl bzip2 runit     && ${CLEANUP_COMMAND}
# Sat, 30 Apr 2022 00:15:49 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/6.5.2
# Sat, 30 Apr 2022 00:15:49 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_6.5.2-ubuntu18.04_amd64.deb
# Sat, 30 Apr 2022 00:15:49 GMT
ARG CB_PACKAGE_NAME=couchbase-server
# Sat, 30 Apr 2022 00:15:49 GMT
ARG CB_SHA256=62f9ffad86eab90137701baab421586af49fe0e7c458bb047b6c364c6ad11684
# Sat, 30 Apr 2022 00:15:49 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Sat, 30 Apr 2022 00:15:50 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.5.2-ubuntu18.04_amd64.deb CB_PACKAGE_NAME=couchbase-server CB_RELEASE_URL=https://packages.couchbase.com/releases/6.5.2 CB_SHA256=62f9ffad86eab90137701baab421586af49fe0e7c458bb047b6c364c6ad11684 CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Sat, 30 Apr 2022 00:17:21 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.5.2-ubuntu18.04_amd64.deb CB_PACKAGE_NAME=couchbase-server CB_RELEASE_URL=https://packages.couchbase.com/releases/6.5.2 CB_SHA256=62f9ffad86eab90137701baab421586af49fe0e7c458bb047b6c364c6ad11684 CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && export INSTALL_DONT_START_SERVER=1     && wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE     && echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c -     && ${UPDATE_COMMAND}     && dpkg --unpack ./$CB_PACKAGE     && sed -i -e '/Best heuristic/ a \ \ \ \ [ -d /run/systemd/system ] && return 1; return 0' /opt/couchbase/bin/install/systemd-ctl     && dpkg --configure couchbase-server     && apt-get install -yf     && rm -f ./$CB_PACKAGE     && ${CLEANUP_COMMAND}     && rm -rf /tmp/* /var/tmp/*
# Sat, 30 Apr 2022 00:17:24 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.5.2-ubuntu18.04_amd64.deb CB_PACKAGE_NAME=couchbase-server CB_RELEASE_URL=https://packages.couchbase.com/releases/6.5.2 CB_SHA256=62f9ffad86eab90137701baab421586af49fe0e7c458bb047b6c364c6ad11684 CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Sat, 30 Apr 2022 00:17:24 GMT
COPY file:018fa38d92aa0a4679f57c2d43b5c14547b2c603cab6ec7fd3240af5545472b5 in /etc/service/couchbase-server/run 
# Sat, 30 Apr 2022 00:17:25 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.5.2-ubuntu18.04_amd64.deb CB_PACKAGE_NAME=couchbase-server CB_RELEASE_URL=https://packages.couchbase.com/releases/6.5.2 CB_SHA256=62f9ffad86eab90137701baab421586af49fe0e7c458bb047b6c364c6ad11684 CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Sat, 30 Apr 2022 00:17:25 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Sat, 30 Apr 2022 00:17:26 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.5.2-ubuntu18.04_amd64.deb CB_PACKAGE_NAME=couchbase-server CB_RELEASE_URL=https://packages.couchbase.com/releases/6.5.2 CB_SHA256=62f9ffad86eab90137701baab421586af49fe0e7c458bb047b6c364c6ad11684 CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ln -s dummy.sh /usr/local/bin/iptables-save     && ln -s dummy.sh /usr/local/bin/lvdisplay     && ln -s dummy.sh /usr/local/bin/vgdisplay     && ln -s dummy.sh /usr/local/bin/pvdisplay
# Sat, 30 Apr 2022 00:17:34 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.5.2-ubuntu18.04_amd64.deb CB_PACKAGE_NAME=couchbase-server CB_RELEASE_URL=https://packages.couchbase.com/releases/6.5.2 CB_SHA256=62f9ffad86eab90137701baab421586af49fe0e7c458bb047b6c364c6ad11684 CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -ex     &&  if [ ! -e /opt/couchbase/bin/curl.real ]; then             ${UPDATE_COMMAND};             apt-get install -y chrpath;             chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl;             apt-get remove -y chrpath;             apt-get autoremove -y;             ${CLEANUP_COMMAND};         fi
# Sat, 30 Apr 2022 00:17:34 GMT
COPY file:6e5292e89c7124e038a0d80ea3b942bff1ed578e67a07e764b041ea95b129aa3 in / 
# Sat, 30 Apr 2022 00:17:34 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 30 Apr 2022 00:17:34 GMT
CMD ["couchbase-server"]
# Sat, 30 Apr 2022 00:17:34 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Sat, 30 Apr 2022 00:17:34 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:40dd5be53814ae70b2898558673b7ea18d58bf7ab3433560b9ce3cb76d9ff0b1`  
		Last Modified: Fri, 29 Apr 2022 23:22:07 GMT  
		Size: 26.7 MB (26709108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae179a0fd9533e29049994a549a8b8d0fecafeaf5bf3cae63a0526d2310f88bc`  
		Last Modified: Sat, 30 Apr 2022 00:21:22 GMT  
		Size: 5.6 MB (5638867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d412ed7f219ba0b874ba637945dadab1ba637c8fca1c5a8e814c01c798e74793`  
		Last Modified: Sat, 30 Apr 2022 00:21:20 GMT  
		Size: 2.0 KB (1959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0769600ac1a446b2d12b7a2e921c35c2293a2787023ef472c94f7245f1748aca`  
		Last Modified: Sat, 30 Apr 2022 00:22:09 GMT  
		Size: 471.0 MB (470974353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7314e0df3b04b61df78cf2836e723ee00f9ce2f8b8d24a40e942eb88e3c3e930`  
		Last Modified: Sat, 30 Apr 2022 00:21:21 GMT  
		Size: 192.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:852f9263b4256b1809121ab87ca18d1fa517923bcdb07793ec11c58e6d294943`  
		Last Modified: Sat, 30 Apr 2022 00:21:20 GMT  
		Size: 745.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a48c59bade46100d8a807f338c009aaae34fd15ae31fe4f1d149faf82cdbad17`  
		Last Modified: Sat, 30 Apr 2022 00:21:18 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40a2ec2096780171d7e5236a7f1a8af282c6bb4f7521c266adf47ad15e9a1b33`  
		Last Modified: Sat, 30 Apr 2022 00:21:18 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5483146720dfb8433e50e99472d841b711fe4dd0809596697daa1dc16a00ebea`  
		Last Modified: Sat, 30 Apr 2022 00:21:18 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5d80eca6318c4acf977b52ac7946e3ecdc488a6aac1084a16edba7c13df33c6`  
		Last Modified: Sat, 30 Apr 2022 00:21:18 GMT  
		Size: 433.2 KB (433154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82e52f7d98be3607228b093351115339effa1a17e884a5530b389ceedd062073`  
		Last Modified: Sat, 30 Apr 2022 00:21:18 GMT  
		Size: 868.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchbase:6.6.5`

```console
$ docker pull couchbase@sha256:3886eb23092c8e42c9113ae8b3c2913be8e323130a958739c783bc3e3cd7e9d5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `couchbase:6.6.5` - linux; amd64

```console
$ docker pull couchbase@sha256:02a08c0d00ee19dac6652145fd6f6afbb243fef8b4edea071ed39c99f68f0495
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **541.2 MB (541151121 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8c7bffdfe1ce5fd50c58e005901ba305dd06b5da3993bae9f5913eb9aea1ddd`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Wed, 02 Feb 2022 02:14:45 GMT
ADD file:3ccf747d646089ed7fbb43c40c45dd43e86f0674115f856efada93c7e4a63624 in / 
# Wed, 02 Feb 2022 02:14:46 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 02:43:34 GMT
LABEL maintainer=docker@couchbase.com
# Wed, 02 Feb 2022 02:46:36 GMT
ARG UPDATE_COMMAND=apt-get update -y -q
# Wed, 02 Feb 2022 02:46:37 GMT
ARG CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Wed, 02 Feb 2022 02:46:46 GMT
# ARGS: CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ${UPDATE_COMMAND}     && apt-get install -y -q wget tzdata       lsof lshw sysstat net-tools numactl bzip2 runit     && ${CLEANUP_COMMAND}
# Wed, 02 Feb 2022 02:46:46 GMT
ARG CB_VERSION=6.6.5
# Wed, 02 Feb 2022 02:46:46 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.5
# Wed, 02 Feb 2022 02:46:46 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_6.6.5-ubuntu20.04_amd64.deb
# Wed, 02 Feb 2022 02:46:47 GMT
ARG CB_SHA256=fb2da1880ea993dc7a5695c6fbe14cde62024d865a71a7d44ab653f0f633d4c6
# Wed, 02 Feb 2022 02:46:47 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Wed, 02 Feb 2022 02:46:48 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.5-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.5 CB_SHA256=fb2da1880ea993dc7a5695c6fbe14cde62024d865a71a7d44ab653f0f633d4c6 CB_VERSION=6.6.5 CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Wed, 02 Feb 2022 02:47:48 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.5-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.5 CB_SHA256=fb2da1880ea993dc7a5695c6fbe14cde62024d865a71a7d44ab653f0f633d4c6 CB_VERSION=6.6.5 CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && export INSTALL_DONT_START_SERVER=1     && wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE     && echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c -     && ${UPDATE_COMMAND}     && apt-get install -y ./$CB_PACKAGE     && rm -f ./$CB_PACKAGE     && ${CLEANUP_COMMAND}     && rm -rf /tmp/* /var/tmp/*
# Wed, 02 Feb 2022 02:47:50 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.5-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.5 CB_SHA256=fb2da1880ea993dc7a5695c6fbe14cde62024d865a71a7d44ab653f0f633d4c6 CB_VERSION=6.6.5 CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Wed, 02 Feb 2022 02:47:50 GMT
COPY file:018fa38d92aa0a4679f57c2d43b5c14547b2c603cab6ec7fd3240af5545472b5 in /etc/service/couchbase-server/run 
# Wed, 02 Feb 2022 02:47:51 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.5-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.5 CB_SHA256=fb2da1880ea993dc7a5695c6fbe14cde62024d865a71a7d44ab653f0f633d4c6 CB_VERSION=6.6.5 CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Wed, 02 Feb 2022 02:47:51 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Wed, 02 Feb 2022 02:47:52 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.5-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.5 CB_SHA256=fb2da1880ea993dc7a5695c6fbe14cde62024d865a71a7d44ab653f0f633d4c6 CB_VERSION=6.6.5 CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ln -s dummy.sh /usr/local/bin/iptables-save     && ln -s dummy.sh /usr/local/bin/lvdisplay     && ln -s dummy.sh /usr/local/bin/vgdisplay     && ln -s dummy.sh /usr/local/bin/pvdisplay
# Wed, 02 Feb 2022 02:47:59 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.5-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.5 CB_SHA256=fb2da1880ea993dc7a5695c6fbe14cde62024d865a71a7d44ab653f0f633d4c6 CB_VERSION=6.6.5 CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -ex     &&  if [ ! -e /opt/couchbase/bin/curl.real ]; then             ${UPDATE_COMMAND};             apt-get install -y chrpath;             chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl;             apt-get remove -y chrpath;             apt-get autoremove -y;             ${CLEANUP_COMMAND};         fi
# Wed, 02 Feb 2022 02:47:59 GMT
COPY file:6e5292e89c7124e038a0d80ea3b942bff1ed578e67a07e764b041ea95b129aa3 in / 
# Wed, 02 Feb 2022 02:48:00 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 02 Feb 2022 02:48:00 GMT
CMD ["couchbase-server"]
# Wed, 02 Feb 2022 02:48:00 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Wed, 02 Feb 2022 02:48:00 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:08c01a0ec47e82ebe2bec112f373d160983a6d1e9e66627f66a3322bc403221b`  
		Last Modified: Wed, 02 Feb 2022 02:16:20 GMT  
		Size: 28.6 MB (28564099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1754ce27a7ccb86d31d56d18a4e72ba9d67be285a916c8bd17248b727560a47d`  
		Last Modified: Wed, 02 Feb 2022 02:54:22 GMT  
		Size: 6.3 MB (6252084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd5f7756f763ab2246a969908f94fa0b42406e43c41ad14c419d0ad54beb50d9`  
		Last Modified: Wed, 02 Feb 2022 02:54:20 GMT  
		Size: 1.8 KB (1828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dbc09136fe05f40c619d016d0bba8dd53e94b083e1744226711ea3057fa8379`  
		Last Modified: Wed, 02 Feb 2022 02:55:16 GMT  
		Size: 505.9 MB (505890801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef8fd0fde82ac5cd771ba6993145c59631f0e463809c2b727bd0056ad5f63665`  
		Last Modified: Wed, 02 Feb 2022 02:54:20 GMT  
		Size: 191.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef8719c5cb0fb42529c032006f2414cd51e3ae277a9a9e8e322c4fd2f5d92e80`  
		Last Modified: Wed, 02 Feb 2022 02:54:20 GMT  
		Size: 743.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad063a0ccee34a72b08b383b143fd7c7f0069884c8a984966f56a6bd38c51f3d`  
		Last Modified: Wed, 02 Feb 2022 02:54:18 GMT  
		Size: 280.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf1ec1e07f8149650f4c98a98a9259281d8fe9725da7995f86c9f57a58ec8dee`  
		Last Modified: Wed, 02 Feb 2022 02:54:18 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efdb27013dd5b6ec10d9b8b8778d61a0573b2146537c7a716824bde5f3650be4`  
		Last Modified: Wed, 02 Feb 2022 02:54:18 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b151da713f459104635e6d2bee7174258be998280138a69ec849ad19260f6129`  
		Last Modified: Wed, 02 Feb 2022 02:54:18 GMT  
		Size: 439.8 KB (439771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3fbf1915f342936bd4612edd42a845a199ff81e6bea379983490571b46ef6fd`  
		Last Modified: Wed, 02 Feb 2022 02:54:18 GMT  
		Size: 868.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchbase:7.0.3`

```console
$ docker pull couchbase@sha256:09d0fb59d4f8df68a5a5352bbb172cb41608eb961e1ede38c41b044cb2359461
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `couchbase:7.0.3` - linux; amd64

```console
$ docker pull couchbase@sha256:cc0a5a62c8664ba8684335f195650691b6476a99be5849805d5a13ba572ab9e7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **653.6 MB (653562427 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:24f8a22a0df0012dc1a1270128f1a15a4ee18a95e7f7f253b413dd92181cc97a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Fri, 29 Apr 2022 23:20:59 GMT
ADD file:7009ad0ee0bbe5ed7f381792e07347e260e6896aeee0d80597808065120fa96b in / 
# Fri, 29 Apr 2022 23:20:59 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 00:04:47 GMT
LABEL maintainer=docker@couchbase.com
# Sat, 30 Apr 2022 00:04:47 GMT
ARG UPDATE_COMMAND=apt-get update -y -q
# Sat, 30 Apr 2022 00:04:48 GMT
ARG CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Sat, 30 Apr 2022 00:05:04 GMT
# ARGS: CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ${UPDATE_COMMAND}     && apt-get install -y -q wget tzdata       lsof lshw sysstat net-tools numactl bzip2 runit     && ${CLEANUP_COMMAND}
# Sat, 30 Apr 2022 00:05:04 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.3-MP1
# Sat, 30 Apr 2022 00:05:04 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_7.0.3-MP1-ubuntu20.04_amd64.deb
# Sat, 30 Apr 2022 00:05:04 GMT
ARG CB_SHA256=a1bfcc476e01c71a212c2ed5026f24f3df01b3591c24dcf45678fdb2625cfc0f
# Sat, 30 Apr 2022 00:05:04 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Sat, 30 Apr 2022 00:05:05 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.3-MP1-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.3-MP1 CB_SHA256=a1bfcc476e01c71a212c2ed5026f24f3df01b3591c24dcf45678fdb2625cfc0f CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Sat, 30 Apr 2022 00:07:01 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.3-MP1-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.3-MP1 CB_SHA256=a1bfcc476e01c71a212c2ed5026f24f3df01b3591c24dcf45678fdb2625cfc0f CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && export INSTALL_DONT_START_SERVER=1     && wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE     && echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c -     && ${UPDATE_COMMAND}     && apt-get install -y ./$CB_PACKAGE     && rm -f ./$CB_PACKAGE     && ${CLEANUP_COMMAND}     && rm -rf /tmp/* /var/tmp/*
# Sat, 30 Apr 2022 00:07:07 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.3-MP1-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.3-MP1 CB_SHA256=a1bfcc476e01c71a212c2ed5026f24f3df01b3591c24dcf45678fdb2625cfc0f CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Sat, 30 Apr 2022 00:07:07 GMT
COPY file:018fa38d92aa0a4679f57c2d43b5c14547b2c603cab6ec7fd3240af5545472b5 in /etc/service/couchbase-server/run 
# Sat, 30 Apr 2022 00:07:07 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.3-MP1-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.3-MP1 CB_SHA256=a1bfcc476e01c71a212c2ed5026f24f3df01b3591c24dcf45678fdb2625cfc0f CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Sat, 30 Apr 2022 00:07:07 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Sat, 30 Apr 2022 00:07:08 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.3-MP1-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.3-MP1 CB_SHA256=a1bfcc476e01c71a212c2ed5026f24f3df01b3591c24dcf45678fdb2625cfc0f CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ln -s dummy.sh /usr/local/bin/iptables-save     && ln -s dummy.sh /usr/local/bin/lvdisplay     && ln -s dummy.sh /usr/local/bin/vgdisplay     && ln -s dummy.sh /usr/local/bin/pvdisplay
# Sat, 30 Apr 2022 00:07:14 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.3-MP1-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.3-MP1 CB_SHA256=a1bfcc476e01c71a212c2ed5026f24f3df01b3591c24dcf45678fdb2625cfc0f CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -ex     &&  if [ ! -e /opt/couchbase/bin/curl.real ]; then             ${UPDATE_COMMAND};             apt-get install -y chrpath;             chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl;             apt-get remove -y chrpath;             apt-get autoremove -y;             ${CLEANUP_COMMAND};         fi
# Sat, 30 Apr 2022 00:07:14 GMT
COPY file:6e5292e89c7124e038a0d80ea3b942bff1ed578e67a07e764b041ea95b129aa3 in / 
# Sat, 30 Apr 2022 00:07:14 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 30 Apr 2022 00:07:15 GMT
CMD ["couchbase-server"]
# Sat, 30 Apr 2022 00:07:15 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Sat, 30 Apr 2022 00:07:15 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:d5fd17ec1767521cf97f61568096bfc9a7cd9c2d149576a7b43930c5a97062b0`  
		Last Modified: Thu, 28 Apr 2022 03:03:21 GMT  
		Size: 28.6 MB (28566230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76937b0923f63ef62ef0ce2435f73244f7f909cc74136aba1228f2e2574af748`  
		Last Modified: Sat, 30 Apr 2022 00:18:06 GMT  
		Size: 6.3 MB (6250617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce99684904adf2c3f56e5d7abd675e5cf6a024381ea64a827e805e2022974da6`  
		Last Modified: Sat, 30 Apr 2022 00:18:05 GMT  
		Size: 1.8 KB (1835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff533d3886c8143e80c8fcce9834656e1796453ca5f6e579442e59e644fb9aa8`  
		Last Modified: Sat, 30 Apr 2022 00:19:09 GMT  
		Size: 618.3 MB (618297660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:244f8c789e91a9b9c853463ba29dfb9da147c72b8d9bf54e5e3b0b34ae85d84a`  
		Last Modified: Sat, 30 Apr 2022 00:18:05 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ac7ffc32bcefda82cafad3d09e24ff3bb1643231bf1c5df473999927f9a0029`  
		Last Modified: Sat, 30 Apr 2022 00:18:05 GMT  
		Size: 736.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fbe28691c5e53c547e3f6750a7300ccb0f093986c50167e69281f51db18b2b2`  
		Last Modified: Sat, 30 Apr 2022 00:18:02 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0b46d9ecfa389b345724069f06b58b43916e7ad0d55d6b757729079a2e77337`  
		Last Modified: Sat, 30 Apr 2022 00:18:02 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a747a0b4e81b2d4a1436f1498f57d42f9ae15b9d4126e6d9ced78261052955c1`  
		Last Modified: Sat, 30 Apr 2022 00:18:03 GMT  
		Size: 217.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e71663811e7ab33e06489f5a666fcc8174db799b918054c69565853d630a8f2`  
		Last Modified: Sat, 30 Apr 2022 00:18:03 GMT  
		Size: 443.6 KB (443560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f20164e41e2fec4dc4897c33ac3ad902b50c2d83da7c0e19a4f85c566323b12`  
		Last Modified: Sat, 30 Apr 2022 00:18:02 GMT  
		Size: 868.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchbase:community`

```console
$ docker pull couchbase@sha256:cacc48d84f6cb0d217d76ef214325b25842bd6b8fe5af87a7675754e67846d10
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `couchbase:community` - linux; amd64

```console
$ docker pull couchbase@sha256:5eecc82a485c2c8791b9c82672ac003ade5d3608366e3979b8561307337820ca
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **429.0 MB (429022236 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c2a1babbec08293d5c0187fb2092a26ce27be742ec7d9f901f15b340dbb24a73`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Fri, 29 Apr 2022 23:20:59 GMT
ADD file:7009ad0ee0bbe5ed7f381792e07347e260e6896aeee0d80597808065120fa96b in / 
# Fri, 29 Apr 2022 23:20:59 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 00:04:47 GMT
LABEL maintainer=docker@couchbase.com
# Sat, 30 Apr 2022 00:07:34 GMT
RUN set -x &&     apt-get update &&     apt-get install -yq runit wget chrpath tzdata     lsof lshw sysstat net-tools numactl bzip2 &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Sat, 30 Apr 2022 00:07:35 GMT
RUN if [ ! -x /usr/sbin/runsvdir-start ]; then         cp -a /etc/runit/2 /usr/sbin/runsvdir-start;     fi
# Sat, 30 Apr 2022 00:07:35 GMT
ARG CB_VERSION=7.0.2
# Sat, 30 Apr 2022 00:07:35 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.2
# Sat, 30 Apr 2022 00:07:35 GMT
ARG CB_PACKAGE=couchbase-server-community_7.0.2-ubuntu20.04_amd64.deb
# Sat, 30 Apr 2022 00:07:36 GMT
ARG CB_SHA256=f935dcad5c04b553a3c56d782c8d9cb782cbd1cf88878a425ba5f9d45d08120e
# Sat, 30 Apr 2022 00:07:36 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Sat, 30 Apr 2022 00:07:36 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.0.2-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.2 CB_SHA256=f935dcad5c04b553a3c56d782c8d9cb782cbd1cf88878a425ba5f9d45d08120e CB_VERSION=7.0.2
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Sat, 30 Apr 2022 00:08:26 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.0.2-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.2 CB_SHA256=f935dcad5c04b553a3c56d782c8d9cb782cbd1cf88878a425ba5f9d45d08120e CB_VERSION=7.0.2
RUN set -x &&     export INSTALL_DONT_START_SERVER=1 &&     wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE &&     echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - &&     apt-get update &&     apt-get install -y ./$CB_PACKAGE &&     rm -f ./$CB_PACKAGE &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Sat, 30 Apr 2022 00:08:30 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.0.2-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.2 CB_SHA256=f935dcad5c04b553a3c56d782c8d9cb782cbd1cf88878a425ba5f9d45d08120e CB_VERSION=7.0.2
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Sat, 30 Apr 2022 00:08:30 GMT
COPY file:cf9c7c8a9eda8a5fefcaa60d67181024b8a07b30eb318d4c9591b33a95ca6680 in /etc/service/couchbase-server/run 
# Sat, 30 Apr 2022 00:08:31 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.0.2-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.2 CB_SHA256=f935dcad5c04b553a3c56d782c8d9cb782cbd1cf88878a425ba5f9d45d08120e CB_VERSION=7.0.2
RUN mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Sat, 30 Apr 2022 00:08:31 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Sat, 30 Apr 2022 00:08:31 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.0.2-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.2 CB_SHA256=f935dcad5c04b553a3c56d782c8d9cb782cbd1cf88878a425ba5f9d45d08120e CB_VERSION=7.0.2
RUN ln -s dummy.sh /usr/local/bin/iptables-save &&     ln -s dummy.sh /usr/local/bin/lvdisplay &&     ln -s dummy.sh /usr/local/bin/vgdisplay &&     ln -s dummy.sh /usr/local/bin/pvdisplay
# Sat, 30 Apr 2022 00:08:32 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.0.2-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.2 CB_SHA256=f935dcad5c04b553a3c56d782c8d9cb782cbd1cf88878a425ba5f9d45d08120e CB_VERSION=7.0.2
RUN chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl
# Sat, 30 Apr 2022 00:08:32 GMT
COPY file:d816a67f62bfba76d2812cefbe92252afa13f3852775c3e68599df7741e90cb7 in / 
# Sat, 30 Apr 2022 00:08:32 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 30 Apr 2022 00:08:32 GMT
CMD ["couchbase-server"]
# Sat, 30 Apr 2022 00:08:32 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Sat, 30 Apr 2022 00:08:32 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:d5fd17ec1767521cf97f61568096bfc9a7cd9c2d149576a7b43930c5a97062b0`  
		Last Modified: Thu, 28 Apr 2022 03:03:21 GMT  
		Size: 28.6 MB (28566230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb3557df45000fab4a156d3d854e0e4e1fa62fc6744e80dd551b0cbe51261382`  
		Last Modified: Sat, 30 Apr 2022 00:19:32 GMT  
		Size: 6.3 MB (6260259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b44832538c57317a4d2d2b80f48727f4d217252e0c1bca9c91764bd3c52a311f`  
		Last Modified: Sat, 30 Apr 2022 00:19:29 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13d30557d2ae3752e5656d5e84ddfae00bbe5f1ee403e60214744c746db794b3`  
		Last Modified: Sat, 30 Apr 2022 00:19:29 GMT  
		Size: 1.8 KB (1834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05b022756e9eff4e2e5043cb6659cab72580afe823cb389bb288654a2fc7198c`  
		Last Modified: Sat, 30 Apr 2022 00:20:16 GMT  
		Size: 394.1 MB (394061761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54953e785e715fc3f75b5da9872ef7e4cd20b3722a207b4a7f618e7b15b68c4b`  
		Last Modified: Sat, 30 Apr 2022 00:19:29 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:365e976ccb685fa81ab103237d8da5e28ccc337555fdd76dcd3c0460a98a103b`  
		Last Modified: Sat, 30 Apr 2022 00:19:29 GMT  
		Size: 602.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da18e09f47baa880cfade31cac7432f3c5253afe94850de0ff5f68a9d6f3206c`  
		Last Modified: Sat, 30 Apr 2022 00:19:26 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:902ecff6559e761c4792e2329e0fde5bb97f16ea8fc06f5fc3671a5ff5417786`  
		Last Modified: Sat, 30 Apr 2022 00:19:27 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:062a2e7b179327ace70e89151a9cb12948137758865a2aa292d140a8f32090b5`  
		Last Modified: Sat, 30 Apr 2022 00:19:27 GMT  
		Size: 217.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:068a0ecce2ebd008f15d64aa4c009579552ba84fd613c91906bd3efca784ab5e`  
		Last Modified: Sat, 30 Apr 2022 00:19:26 GMT  
		Size: 129.5 KB (129509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d1ef33dbf8866706153e7fe6b13631c7678e3c90427e5a23f0cdceadba7c100`  
		Last Modified: Sat, 30 Apr 2022 00:19:26 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchbase:community-6.6.0`

```console
$ docker pull couchbase@sha256:fdd1d32c15ba32f2ede75472b17d2d46faa091b2dda3e7a332f985cdcc90162b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `couchbase:community-6.6.0` - linux; amd64

```console
$ docker pull couchbase@sha256:d201c08a35d3c387891b7db0f9b738729f3ca699c1e78bd3cffc97053314dc97
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **354.2 MB (354218743 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cc22a56175d8ceef0a6c9b673b56e89cfacb9872a41898a14e8cad76c3f1e9c1`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Wed, 02 Feb 2022 02:14:36 GMT
ADD file:c6039a4f004b6b6c2e4c281a228d64d8410cb9fdf0c67776f84bb173d3522be1 in / 
# Wed, 02 Feb 2022 02:14:36 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 02:48:15 GMT
LABEL maintainer=docker@couchbase.com
# Wed, 02 Feb 2022 02:48:45 GMT
RUN set -x &&     apt-get update &&     apt-get install -yq runit wget chrpath tzdata man     lsof lshw sysstat net-tools numactl bzip2 &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Wed, 02 Feb 2022 02:48:46 GMT
RUN if [ ! -x /usr/sbin/runsvdir-start ]; then         cp -a /etc/runit/2 /usr/sbin/runsvdir-start;     fi
# Wed, 02 Feb 2022 02:48:46 GMT
ARG CB_VERSION=6.6.0
# Wed, 02 Feb 2022 02:48:46 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0
# Wed, 02 Feb 2022 02:48:47 GMT
ARG CB_PACKAGE=couchbase-server-community_6.6.0-ubuntu18.04_amd64.deb
# Wed, 02 Feb 2022 02:48:47 GMT
ARG CB_SHA256=9b196cd7be81d7d6b179838e9d30164fdb7a1f27e96678e61e24e9fe5c93f559
# Wed, 02 Feb 2022 02:48:47 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Wed, 02 Feb 2022 02:48:48 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_6.6.0-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=9b196cd7be81d7d6b179838e9d30164fdb7a1f27e96678e61e24e9fe5c93f559 CB_VERSION=6.6.0
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Wed, 02 Feb 2022 02:49:34 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_6.6.0-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=9b196cd7be81d7d6b179838e9d30164fdb7a1f27e96678e61e24e9fe5c93f559 CB_VERSION=6.6.0
RUN set -x &&     export INSTALL_DONT_START_SERVER=1 &&     wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE &&     echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - &&     apt-get update &&     apt-get install -y ./$CB_PACKAGE &&     rm -f ./$CB_PACKAGE &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Wed, 02 Feb 2022 02:49:35 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_6.6.0-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=9b196cd7be81d7d6b179838e9d30164fdb7a1f27e96678e61e24e9fe5c93f559 CB_VERSION=6.6.0
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Wed, 02 Feb 2022 02:49:35 GMT
COPY file:d6a307209223b2df102f46f07fd186e09fac7114db2c965bb54097d3b4d3b989 in /etc/service/couchbase-server/run 
# Wed, 02 Feb 2022 02:49:36 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_6.6.0-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=9b196cd7be81d7d6b179838e9d30164fdb7a1f27e96678e61e24e9fe5c93f559 CB_VERSION=6.6.0
RUN mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Wed, 02 Feb 2022 02:49:37 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Wed, 02 Feb 2022 02:49:37 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_6.6.0-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=9b196cd7be81d7d6b179838e9d30164fdb7a1f27e96678e61e24e9fe5c93f559 CB_VERSION=6.6.0
RUN ln -s dummy.sh /usr/local/bin/iptables-save &&     ln -s dummy.sh /usr/local/bin/lvdisplay &&     ln -s dummy.sh /usr/local/bin/vgdisplay &&     ln -s dummy.sh /usr/local/bin/pvdisplay
# Wed, 02 Feb 2022 02:49:38 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_6.6.0-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=9b196cd7be81d7d6b179838e9d30164fdb7a1f27e96678e61e24e9fe5c93f559 CB_VERSION=6.6.0
RUN chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl
# Wed, 02 Feb 2022 02:49:38 GMT
COPY file:d816a67f62bfba76d2812cefbe92252afa13f3852775c3e68599df7741e90cb7 in / 
# Wed, 02 Feb 2022 02:49:39 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 02 Feb 2022 02:49:39 GMT
CMD ["couchbase-server"]
# Wed, 02 Feb 2022 02:49:39 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Wed, 02 Feb 2022 02:49:39 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:68e7bb398b9ff421236990bfeaf5c1feab26c590eed93489e245375c23551e2a`  
		Last Modified: Sat, 29 Jan 2022 14:35:20 GMT  
		Size: 26.7 MB (26708066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e425b875a003fc3d1cb0261376c6c7b06f317ab62edc525973f364a81fa715b6`  
		Last Modified: Wed, 02 Feb 2022 02:55:33 GMT  
		Size: 7.4 MB (7369685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db3acdc189fe79683161c15fb20351332b6fa980f57cbbf2c14f9bc7a91839b1`  
		Last Modified: Wed, 02 Feb 2022 02:55:31 GMT  
		Size: 264.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:216d4566df698875020ff56135b7c4b9ccec4f3ed1ac3bf3647dbe9236e6e44d`  
		Last Modified: Wed, 02 Feb 2022 02:55:30 GMT  
		Size: 2.0 KB (1962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8a90fe8027662b5c454b3410922cf215003675074534f975f0fc8bfe298e55b`  
		Last Modified: Wed, 02 Feb 2022 02:56:08 GMT  
		Size: 320.0 MB (320018322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5181984dfb9361c67df2c5b5993c6cc4f3b6065bfcbf12064a6661a56f279da5`  
		Last Modified: Wed, 02 Feb 2022 02:55:29 GMT  
		Size: 191.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b9dbdaf5435709bc5339630f695ff46a9380d7db3b17b9042c96d3e027fd13a`  
		Last Modified: Wed, 02 Feb 2022 02:55:29 GMT  
		Size: 473.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d53a24c87a7220452e0949585ac9559d60825e6ef9e70e29411569fc08e95e2e`  
		Last Modified: Wed, 02 Feb 2022 02:55:27 GMT  
		Size: 281.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:677095b029f2d6edf084c96e7c2cfa782c4450b6afa0fd39e253e8e0d62b2baf`  
		Last Modified: Wed, 02 Feb 2022 02:55:27 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ebc26fc42224cfbda435889d30e771ad96c02654c19e9fc3beb0e7f2eba22fe`  
		Last Modified: Wed, 02 Feb 2022 02:55:27 GMT  
		Size: 217.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aefcba46347e465d160a8620560e12acac13b728cfbb45fadb512c02ce03d94`  
		Last Modified: Wed, 02 Feb 2022 02:55:27 GMT  
		Size: 118.2 KB (118189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f556ceef96e57756240bf0d787fb91e7436f7630832ebb86197ffff68c7f143e`  
		Last Modified: Wed, 02 Feb 2022 02:55:27 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchbase:community-7.0.2`

```console
$ docker pull couchbase@sha256:cacc48d84f6cb0d217d76ef214325b25842bd6b8fe5af87a7675754e67846d10
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `couchbase:community-7.0.2` - linux; amd64

```console
$ docker pull couchbase@sha256:5eecc82a485c2c8791b9c82672ac003ade5d3608366e3979b8561307337820ca
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **429.0 MB (429022236 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c2a1babbec08293d5c0187fb2092a26ce27be742ec7d9f901f15b340dbb24a73`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Fri, 29 Apr 2022 23:20:59 GMT
ADD file:7009ad0ee0bbe5ed7f381792e07347e260e6896aeee0d80597808065120fa96b in / 
# Fri, 29 Apr 2022 23:20:59 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 00:04:47 GMT
LABEL maintainer=docker@couchbase.com
# Sat, 30 Apr 2022 00:07:34 GMT
RUN set -x &&     apt-get update &&     apt-get install -yq runit wget chrpath tzdata     lsof lshw sysstat net-tools numactl bzip2 &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Sat, 30 Apr 2022 00:07:35 GMT
RUN if [ ! -x /usr/sbin/runsvdir-start ]; then         cp -a /etc/runit/2 /usr/sbin/runsvdir-start;     fi
# Sat, 30 Apr 2022 00:07:35 GMT
ARG CB_VERSION=7.0.2
# Sat, 30 Apr 2022 00:07:35 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.2
# Sat, 30 Apr 2022 00:07:35 GMT
ARG CB_PACKAGE=couchbase-server-community_7.0.2-ubuntu20.04_amd64.deb
# Sat, 30 Apr 2022 00:07:36 GMT
ARG CB_SHA256=f935dcad5c04b553a3c56d782c8d9cb782cbd1cf88878a425ba5f9d45d08120e
# Sat, 30 Apr 2022 00:07:36 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Sat, 30 Apr 2022 00:07:36 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.0.2-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.2 CB_SHA256=f935dcad5c04b553a3c56d782c8d9cb782cbd1cf88878a425ba5f9d45d08120e CB_VERSION=7.0.2
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Sat, 30 Apr 2022 00:08:26 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.0.2-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.2 CB_SHA256=f935dcad5c04b553a3c56d782c8d9cb782cbd1cf88878a425ba5f9d45d08120e CB_VERSION=7.0.2
RUN set -x &&     export INSTALL_DONT_START_SERVER=1 &&     wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE &&     echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - &&     apt-get update &&     apt-get install -y ./$CB_PACKAGE &&     rm -f ./$CB_PACKAGE &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Sat, 30 Apr 2022 00:08:30 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.0.2-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.2 CB_SHA256=f935dcad5c04b553a3c56d782c8d9cb782cbd1cf88878a425ba5f9d45d08120e CB_VERSION=7.0.2
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Sat, 30 Apr 2022 00:08:30 GMT
COPY file:cf9c7c8a9eda8a5fefcaa60d67181024b8a07b30eb318d4c9591b33a95ca6680 in /etc/service/couchbase-server/run 
# Sat, 30 Apr 2022 00:08:31 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.0.2-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.2 CB_SHA256=f935dcad5c04b553a3c56d782c8d9cb782cbd1cf88878a425ba5f9d45d08120e CB_VERSION=7.0.2
RUN mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Sat, 30 Apr 2022 00:08:31 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Sat, 30 Apr 2022 00:08:31 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.0.2-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.2 CB_SHA256=f935dcad5c04b553a3c56d782c8d9cb782cbd1cf88878a425ba5f9d45d08120e CB_VERSION=7.0.2
RUN ln -s dummy.sh /usr/local/bin/iptables-save &&     ln -s dummy.sh /usr/local/bin/lvdisplay &&     ln -s dummy.sh /usr/local/bin/vgdisplay &&     ln -s dummy.sh /usr/local/bin/pvdisplay
# Sat, 30 Apr 2022 00:08:32 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.0.2-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.2 CB_SHA256=f935dcad5c04b553a3c56d782c8d9cb782cbd1cf88878a425ba5f9d45d08120e CB_VERSION=7.0.2
RUN chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl
# Sat, 30 Apr 2022 00:08:32 GMT
COPY file:d816a67f62bfba76d2812cefbe92252afa13f3852775c3e68599df7741e90cb7 in / 
# Sat, 30 Apr 2022 00:08:32 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 30 Apr 2022 00:08:32 GMT
CMD ["couchbase-server"]
# Sat, 30 Apr 2022 00:08:32 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Sat, 30 Apr 2022 00:08:32 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:d5fd17ec1767521cf97f61568096bfc9a7cd9c2d149576a7b43930c5a97062b0`  
		Last Modified: Thu, 28 Apr 2022 03:03:21 GMT  
		Size: 28.6 MB (28566230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb3557df45000fab4a156d3d854e0e4e1fa62fc6744e80dd551b0cbe51261382`  
		Last Modified: Sat, 30 Apr 2022 00:19:32 GMT  
		Size: 6.3 MB (6260259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b44832538c57317a4d2d2b80f48727f4d217252e0c1bca9c91764bd3c52a311f`  
		Last Modified: Sat, 30 Apr 2022 00:19:29 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13d30557d2ae3752e5656d5e84ddfae00bbe5f1ee403e60214744c746db794b3`  
		Last Modified: Sat, 30 Apr 2022 00:19:29 GMT  
		Size: 1.8 KB (1834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05b022756e9eff4e2e5043cb6659cab72580afe823cb389bb288654a2fc7198c`  
		Last Modified: Sat, 30 Apr 2022 00:20:16 GMT  
		Size: 394.1 MB (394061761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54953e785e715fc3f75b5da9872ef7e4cd20b3722a207b4a7f618e7b15b68c4b`  
		Last Modified: Sat, 30 Apr 2022 00:19:29 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:365e976ccb685fa81ab103237d8da5e28ccc337555fdd76dcd3c0460a98a103b`  
		Last Modified: Sat, 30 Apr 2022 00:19:29 GMT  
		Size: 602.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da18e09f47baa880cfade31cac7432f3c5253afe94850de0ff5f68a9d6f3206c`  
		Last Modified: Sat, 30 Apr 2022 00:19:26 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:902ecff6559e761c4792e2329e0fde5bb97f16ea8fc06f5fc3671a5ff5417786`  
		Last Modified: Sat, 30 Apr 2022 00:19:27 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:062a2e7b179327ace70e89151a9cb12948137758865a2aa292d140a8f32090b5`  
		Last Modified: Sat, 30 Apr 2022 00:19:27 GMT  
		Size: 217.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:068a0ecce2ebd008f15d64aa4c009579552ba84fd613c91906bd3efca784ab5e`  
		Last Modified: Sat, 30 Apr 2022 00:19:26 GMT  
		Size: 129.5 KB (129509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d1ef33dbf8866706153e7fe6b13631c7678e3c90427e5a23f0cdceadba7c100`  
		Last Modified: Sat, 30 Apr 2022 00:19:26 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchbase:enterprise`

```console
$ docker pull couchbase@sha256:09d0fb59d4f8df68a5a5352bbb172cb41608eb961e1ede38c41b044cb2359461
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `couchbase:enterprise` - linux; amd64

```console
$ docker pull couchbase@sha256:cc0a5a62c8664ba8684335f195650691b6476a99be5849805d5a13ba572ab9e7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **653.6 MB (653562427 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:24f8a22a0df0012dc1a1270128f1a15a4ee18a95e7f7f253b413dd92181cc97a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Fri, 29 Apr 2022 23:20:59 GMT
ADD file:7009ad0ee0bbe5ed7f381792e07347e260e6896aeee0d80597808065120fa96b in / 
# Fri, 29 Apr 2022 23:20:59 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 00:04:47 GMT
LABEL maintainer=docker@couchbase.com
# Sat, 30 Apr 2022 00:04:47 GMT
ARG UPDATE_COMMAND=apt-get update -y -q
# Sat, 30 Apr 2022 00:04:48 GMT
ARG CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Sat, 30 Apr 2022 00:05:04 GMT
# ARGS: CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ${UPDATE_COMMAND}     && apt-get install -y -q wget tzdata       lsof lshw sysstat net-tools numactl bzip2 runit     && ${CLEANUP_COMMAND}
# Sat, 30 Apr 2022 00:05:04 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.3-MP1
# Sat, 30 Apr 2022 00:05:04 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_7.0.3-MP1-ubuntu20.04_amd64.deb
# Sat, 30 Apr 2022 00:05:04 GMT
ARG CB_SHA256=a1bfcc476e01c71a212c2ed5026f24f3df01b3591c24dcf45678fdb2625cfc0f
# Sat, 30 Apr 2022 00:05:04 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Sat, 30 Apr 2022 00:05:05 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.3-MP1-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.3-MP1 CB_SHA256=a1bfcc476e01c71a212c2ed5026f24f3df01b3591c24dcf45678fdb2625cfc0f CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Sat, 30 Apr 2022 00:07:01 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.3-MP1-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.3-MP1 CB_SHA256=a1bfcc476e01c71a212c2ed5026f24f3df01b3591c24dcf45678fdb2625cfc0f CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && export INSTALL_DONT_START_SERVER=1     && wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE     && echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c -     && ${UPDATE_COMMAND}     && apt-get install -y ./$CB_PACKAGE     && rm -f ./$CB_PACKAGE     && ${CLEANUP_COMMAND}     && rm -rf /tmp/* /var/tmp/*
# Sat, 30 Apr 2022 00:07:07 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.3-MP1-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.3-MP1 CB_SHA256=a1bfcc476e01c71a212c2ed5026f24f3df01b3591c24dcf45678fdb2625cfc0f CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Sat, 30 Apr 2022 00:07:07 GMT
COPY file:018fa38d92aa0a4679f57c2d43b5c14547b2c603cab6ec7fd3240af5545472b5 in /etc/service/couchbase-server/run 
# Sat, 30 Apr 2022 00:07:07 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.3-MP1-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.3-MP1 CB_SHA256=a1bfcc476e01c71a212c2ed5026f24f3df01b3591c24dcf45678fdb2625cfc0f CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Sat, 30 Apr 2022 00:07:07 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Sat, 30 Apr 2022 00:07:08 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.3-MP1-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.3-MP1 CB_SHA256=a1bfcc476e01c71a212c2ed5026f24f3df01b3591c24dcf45678fdb2625cfc0f CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ln -s dummy.sh /usr/local/bin/iptables-save     && ln -s dummy.sh /usr/local/bin/lvdisplay     && ln -s dummy.sh /usr/local/bin/vgdisplay     && ln -s dummy.sh /usr/local/bin/pvdisplay
# Sat, 30 Apr 2022 00:07:14 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.3-MP1-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.3-MP1 CB_SHA256=a1bfcc476e01c71a212c2ed5026f24f3df01b3591c24dcf45678fdb2625cfc0f CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -ex     &&  if [ ! -e /opt/couchbase/bin/curl.real ]; then             ${UPDATE_COMMAND};             apt-get install -y chrpath;             chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl;             apt-get remove -y chrpath;             apt-get autoremove -y;             ${CLEANUP_COMMAND};         fi
# Sat, 30 Apr 2022 00:07:14 GMT
COPY file:6e5292e89c7124e038a0d80ea3b942bff1ed578e67a07e764b041ea95b129aa3 in / 
# Sat, 30 Apr 2022 00:07:14 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 30 Apr 2022 00:07:15 GMT
CMD ["couchbase-server"]
# Sat, 30 Apr 2022 00:07:15 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Sat, 30 Apr 2022 00:07:15 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:d5fd17ec1767521cf97f61568096bfc9a7cd9c2d149576a7b43930c5a97062b0`  
		Last Modified: Thu, 28 Apr 2022 03:03:21 GMT  
		Size: 28.6 MB (28566230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76937b0923f63ef62ef0ce2435f73244f7f909cc74136aba1228f2e2574af748`  
		Last Modified: Sat, 30 Apr 2022 00:18:06 GMT  
		Size: 6.3 MB (6250617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce99684904adf2c3f56e5d7abd675e5cf6a024381ea64a827e805e2022974da6`  
		Last Modified: Sat, 30 Apr 2022 00:18:05 GMT  
		Size: 1.8 KB (1835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff533d3886c8143e80c8fcce9834656e1796453ca5f6e579442e59e644fb9aa8`  
		Last Modified: Sat, 30 Apr 2022 00:19:09 GMT  
		Size: 618.3 MB (618297660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:244f8c789e91a9b9c853463ba29dfb9da147c72b8d9bf54e5e3b0b34ae85d84a`  
		Last Modified: Sat, 30 Apr 2022 00:18:05 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ac7ffc32bcefda82cafad3d09e24ff3bb1643231bf1c5df473999927f9a0029`  
		Last Modified: Sat, 30 Apr 2022 00:18:05 GMT  
		Size: 736.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fbe28691c5e53c547e3f6750a7300ccb0f093986c50167e69281f51db18b2b2`  
		Last Modified: Sat, 30 Apr 2022 00:18:02 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0b46d9ecfa389b345724069f06b58b43916e7ad0d55d6b757729079a2e77337`  
		Last Modified: Sat, 30 Apr 2022 00:18:02 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a747a0b4e81b2d4a1436f1498f57d42f9ae15b9d4126e6d9ced78261052955c1`  
		Last Modified: Sat, 30 Apr 2022 00:18:03 GMT  
		Size: 217.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e71663811e7ab33e06489f5a666fcc8174db799b918054c69565853d630a8f2`  
		Last Modified: Sat, 30 Apr 2022 00:18:03 GMT  
		Size: 443.6 KB (443560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f20164e41e2fec4dc4897c33ac3ad902b50c2d83da7c0e19a4f85c566323b12`  
		Last Modified: Sat, 30 Apr 2022 00:18:02 GMT  
		Size: 868.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchbase:enterprise-6.0.5`

```console
$ docker pull couchbase@sha256:f9235779854daa0f5086cab8643b04edb9174778022a013046d0ec431d435af6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `couchbase:enterprise-6.0.5` - linux; amd64

```console
$ docker pull couchbase@sha256:50306e689ca3d28bc4cf08a63cde4130f3fb7899f746b6765948655220ab179a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **466.1 MB (466120858 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d7ea04df160ef1266c43115c9be766670952aa17848dd497dd9ba8ebec92704`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Fri, 29 Apr 2022 23:20:51 GMT
ADD file:f657a56a18426c3a88d620a7024e7b91424d926e7b47faa6a97c2369c4c4a228 in / 
# Fri, 29 Apr 2022 23:20:51 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 00:11:49 GMT
LABEL maintainer=docker@couchbase.com
# Sat, 30 Apr 2022 00:14:34 GMT
RUN set -x &&     apt-get update &&     apt-get install -yq runit wget chrpath tzdata man     lsof lshw sysstat net-tools numactl python-httplib2 &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Sat, 30 Apr 2022 00:14:35 GMT
RUN if [ ! -x /usr/sbin/runsvdir-start ]; then         cp -a /etc/runit/2 /usr/sbin/runsvdir-start;     fi
# Sat, 30 Apr 2022 00:14:35 GMT
ARG CB_VERSION=6.0.5
# Sat, 30 Apr 2022 00:14:35 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.5
# Sat, 30 Apr 2022 00:14:35 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_6.0.5-ubuntu18.04_amd64.deb
# Sat, 30 Apr 2022 00:14:35 GMT
ARG CB_SHA256=6b152590867a58d771cffc22774d3cd66c916defcbeeeb339aca8d0a8e6d7f8d
# Sat, 30 Apr 2022 00:14:35 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Sat, 30 Apr 2022 00:14:36 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.5-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.5 CB_SHA256=6b152590867a58d771cffc22774d3cd66c916defcbeeeb339aca8d0a8e6d7f8d CB_VERSION=6.0.5
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Sat, 30 Apr 2022 00:15:31 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.5-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.5 CB_SHA256=6b152590867a58d771cffc22774d3cd66c916defcbeeeb339aca8d0a8e6d7f8d CB_VERSION=6.0.5
RUN set -x &&     export INSTALL_DONT_START_SERVER=1 &&     wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE &&     echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - &&     apt-get update &&     apt-get install -y ./$CB_PACKAGE &&     rm -f ./$CB_PACKAGE &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Sat, 30 Apr 2022 00:15:33 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.5-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.5 CB_SHA256=6b152590867a58d771cffc22774d3cd66c916defcbeeeb339aca8d0a8e6d7f8d CB_VERSION=6.0.5
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Sat, 30 Apr 2022 00:15:34 GMT
COPY file:d6a307209223b2df102f46f07fd186e09fac7114db2c965bb54097d3b4d3b989 in /etc/service/couchbase-server/run 
# Sat, 30 Apr 2022 00:15:34 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.5-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.5 CB_SHA256=6b152590867a58d771cffc22774d3cd66c916defcbeeeb339aca8d0a8e6d7f8d CB_VERSION=6.0.5
RUN mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Sat, 30 Apr 2022 00:15:34 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Sat, 30 Apr 2022 00:15:35 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.5-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.5 CB_SHA256=6b152590867a58d771cffc22774d3cd66c916defcbeeeb339aca8d0a8e6d7f8d CB_VERSION=6.0.5
RUN ln -s dummy.sh /usr/local/bin/iptables-save &&     ln -s dummy.sh /usr/local/bin/lvdisplay &&     ln -s dummy.sh /usr/local/bin/vgdisplay &&     ln -s dummy.sh /usr/local/bin/pvdisplay
# Sat, 30 Apr 2022 00:15:35 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.5-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.5 CB_SHA256=6b152590867a58d771cffc22774d3cd66c916defcbeeeb339aca8d0a8e6d7f8d CB_VERSION=6.0.5
RUN chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl
# Sat, 30 Apr 2022 00:15:35 GMT
COPY file:d816a67f62bfba76d2812cefbe92252afa13f3852775c3e68599df7741e90cb7 in / 
# Sat, 30 Apr 2022 00:15:36 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 30 Apr 2022 00:15:36 GMT
CMD ["couchbase-server"]
# Sat, 30 Apr 2022 00:15:36 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Sat, 30 Apr 2022 00:15:36 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:40dd5be53814ae70b2898558673b7ea18d58bf7ab3433560b9ce3cb76d9ff0b1`  
		Last Modified: Fri, 29 Apr 2022 23:22:07 GMT  
		Size: 26.7 MB (26709108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfde595bbf77f9f882becea2554e11fb68bdc2ed67be2a0ca3ab93b2a8e49cff`  
		Last Modified: Sat, 30 Apr 2022 00:20:34 GMT  
		Size: 15.9 MB (15918912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84ccb59dfcda9556def1bbc8283f1b7be19631589f0de035ea23199f268989d3`  
		Last Modified: Sat, 30 Apr 2022 00:20:30 GMT  
		Size: 266.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b01d393883f27c086d6a93ba060675ed40ba156c338021fbd72cbb042964946f`  
		Last Modified: Sat, 30 Apr 2022 00:20:30 GMT  
		Size: 2.0 KB (1963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df4708548cc8ecbed1cf773a42f051e67ce079acd1944b258867e33694149dd7`  
		Last Modified: Sat, 30 Apr 2022 00:21:08 GMT  
		Size: 423.4 MB (423362799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25a8fd04a156e32ac4f2707e165ebd41bce031579e4783441827035be8161f9c`  
		Last Modified: Sat, 30 Apr 2022 00:20:30 GMT  
		Size: 191.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b7fdf4876c37245db240610b6f3d33f87c19ff3e646bee18aba32a5c19c51fd`  
		Last Modified: Sat, 30 Apr 2022 00:20:29 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d72c4626e9476266400aadcd452aac6347e688f6087408c114658be387923c1`  
		Last Modified: Sat, 30 Apr 2022 00:20:27 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b2c636e83d08d0f38eebb344b4c6b927e2c10d09ac74f779efb17024bb6546c`  
		Last Modified: Sat, 30 Apr 2022 00:20:27 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79b854237426234651c46a8b651e9321ac0869dea0e44542c8ab27db12759805`  
		Last Modified: Sat, 30 Apr 2022 00:20:27 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbe47a9e327ff459ffe2c301941c92c6e831dafd5bea18d6c5d77c8bc4d7432f`  
		Last Modified: Sat, 30 Apr 2022 00:20:27 GMT  
		Size: 125.6 KB (125556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d86e5a98e04b278372888fbd0d911c838374b6b3bb50a42a672ac4813a4f8fde`  
		Last Modified: Sat, 30 Apr 2022 00:20:28 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchbase:enterprise-6.5.2`

```console
$ docker pull couchbase@sha256:4e19cf0e5ec5f0c57e0bc44d9170ac011243a1fc9cc37a0ebd0362d8dd0bc4ac
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `couchbase:enterprise-6.5.2` - linux; amd64

```console
$ docker pull couchbase@sha256:b8f43ad49a00b04e0a670b530cdad2633c97add377dddca10ab235d21a694d5f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **503.8 MB (503759986 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90f3c9f7ee3c535ad7673a245614a05f9ab4ced807cc3a3a2aaf4815fd2253aa`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Fri, 29 Apr 2022 23:20:51 GMT
ADD file:f657a56a18426c3a88d620a7024e7b91424d926e7b47faa6a97c2369c4c4a228 in / 
# Fri, 29 Apr 2022 23:20:51 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 00:11:49 GMT
LABEL maintainer=docker@couchbase.com
# Sat, 30 Apr 2022 00:15:40 GMT
ARG UPDATE_COMMAND=apt-get update -y -q
# Sat, 30 Apr 2022 00:15:40 GMT
ARG CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Sat, 30 Apr 2022 00:15:49 GMT
# ARGS: CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ${UPDATE_COMMAND}     && apt-get install -y -q wget tzdata       lsof lshw sysstat net-tools numactl bzip2 runit     && ${CLEANUP_COMMAND}
# Sat, 30 Apr 2022 00:15:49 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/6.5.2
# Sat, 30 Apr 2022 00:15:49 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_6.5.2-ubuntu18.04_amd64.deb
# Sat, 30 Apr 2022 00:15:49 GMT
ARG CB_PACKAGE_NAME=couchbase-server
# Sat, 30 Apr 2022 00:15:49 GMT
ARG CB_SHA256=62f9ffad86eab90137701baab421586af49fe0e7c458bb047b6c364c6ad11684
# Sat, 30 Apr 2022 00:15:49 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Sat, 30 Apr 2022 00:15:50 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.5.2-ubuntu18.04_amd64.deb CB_PACKAGE_NAME=couchbase-server CB_RELEASE_URL=https://packages.couchbase.com/releases/6.5.2 CB_SHA256=62f9ffad86eab90137701baab421586af49fe0e7c458bb047b6c364c6ad11684 CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Sat, 30 Apr 2022 00:17:21 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.5.2-ubuntu18.04_amd64.deb CB_PACKAGE_NAME=couchbase-server CB_RELEASE_URL=https://packages.couchbase.com/releases/6.5.2 CB_SHA256=62f9ffad86eab90137701baab421586af49fe0e7c458bb047b6c364c6ad11684 CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && export INSTALL_DONT_START_SERVER=1     && wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE     && echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c -     && ${UPDATE_COMMAND}     && dpkg --unpack ./$CB_PACKAGE     && sed -i -e '/Best heuristic/ a \ \ \ \ [ -d /run/systemd/system ] && return 1; return 0' /opt/couchbase/bin/install/systemd-ctl     && dpkg --configure couchbase-server     && apt-get install -yf     && rm -f ./$CB_PACKAGE     && ${CLEANUP_COMMAND}     && rm -rf /tmp/* /var/tmp/*
# Sat, 30 Apr 2022 00:17:24 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.5.2-ubuntu18.04_amd64.deb CB_PACKAGE_NAME=couchbase-server CB_RELEASE_URL=https://packages.couchbase.com/releases/6.5.2 CB_SHA256=62f9ffad86eab90137701baab421586af49fe0e7c458bb047b6c364c6ad11684 CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Sat, 30 Apr 2022 00:17:24 GMT
COPY file:018fa38d92aa0a4679f57c2d43b5c14547b2c603cab6ec7fd3240af5545472b5 in /etc/service/couchbase-server/run 
# Sat, 30 Apr 2022 00:17:25 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.5.2-ubuntu18.04_amd64.deb CB_PACKAGE_NAME=couchbase-server CB_RELEASE_URL=https://packages.couchbase.com/releases/6.5.2 CB_SHA256=62f9ffad86eab90137701baab421586af49fe0e7c458bb047b6c364c6ad11684 CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Sat, 30 Apr 2022 00:17:25 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Sat, 30 Apr 2022 00:17:26 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.5.2-ubuntu18.04_amd64.deb CB_PACKAGE_NAME=couchbase-server CB_RELEASE_URL=https://packages.couchbase.com/releases/6.5.2 CB_SHA256=62f9ffad86eab90137701baab421586af49fe0e7c458bb047b6c364c6ad11684 CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ln -s dummy.sh /usr/local/bin/iptables-save     && ln -s dummy.sh /usr/local/bin/lvdisplay     && ln -s dummy.sh /usr/local/bin/vgdisplay     && ln -s dummy.sh /usr/local/bin/pvdisplay
# Sat, 30 Apr 2022 00:17:34 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.5.2-ubuntu18.04_amd64.deb CB_PACKAGE_NAME=couchbase-server CB_RELEASE_URL=https://packages.couchbase.com/releases/6.5.2 CB_SHA256=62f9ffad86eab90137701baab421586af49fe0e7c458bb047b6c364c6ad11684 CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -ex     &&  if [ ! -e /opt/couchbase/bin/curl.real ]; then             ${UPDATE_COMMAND};             apt-get install -y chrpath;             chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl;             apt-get remove -y chrpath;             apt-get autoremove -y;             ${CLEANUP_COMMAND};         fi
# Sat, 30 Apr 2022 00:17:34 GMT
COPY file:6e5292e89c7124e038a0d80ea3b942bff1ed578e67a07e764b041ea95b129aa3 in / 
# Sat, 30 Apr 2022 00:17:34 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 30 Apr 2022 00:17:34 GMT
CMD ["couchbase-server"]
# Sat, 30 Apr 2022 00:17:34 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Sat, 30 Apr 2022 00:17:34 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:40dd5be53814ae70b2898558673b7ea18d58bf7ab3433560b9ce3cb76d9ff0b1`  
		Last Modified: Fri, 29 Apr 2022 23:22:07 GMT  
		Size: 26.7 MB (26709108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae179a0fd9533e29049994a549a8b8d0fecafeaf5bf3cae63a0526d2310f88bc`  
		Last Modified: Sat, 30 Apr 2022 00:21:22 GMT  
		Size: 5.6 MB (5638867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d412ed7f219ba0b874ba637945dadab1ba637c8fca1c5a8e814c01c798e74793`  
		Last Modified: Sat, 30 Apr 2022 00:21:20 GMT  
		Size: 2.0 KB (1959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0769600ac1a446b2d12b7a2e921c35c2293a2787023ef472c94f7245f1748aca`  
		Last Modified: Sat, 30 Apr 2022 00:22:09 GMT  
		Size: 471.0 MB (470974353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7314e0df3b04b61df78cf2836e723ee00f9ce2f8b8d24a40e942eb88e3c3e930`  
		Last Modified: Sat, 30 Apr 2022 00:21:21 GMT  
		Size: 192.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:852f9263b4256b1809121ab87ca18d1fa517923bcdb07793ec11c58e6d294943`  
		Last Modified: Sat, 30 Apr 2022 00:21:20 GMT  
		Size: 745.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a48c59bade46100d8a807f338c009aaae34fd15ae31fe4f1d149faf82cdbad17`  
		Last Modified: Sat, 30 Apr 2022 00:21:18 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40a2ec2096780171d7e5236a7f1a8af282c6bb4f7521c266adf47ad15e9a1b33`  
		Last Modified: Sat, 30 Apr 2022 00:21:18 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5483146720dfb8433e50e99472d841b711fe4dd0809596697daa1dc16a00ebea`  
		Last Modified: Sat, 30 Apr 2022 00:21:18 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5d80eca6318c4acf977b52ac7946e3ecdc488a6aac1084a16edba7c13df33c6`  
		Last Modified: Sat, 30 Apr 2022 00:21:18 GMT  
		Size: 433.2 KB (433154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82e52f7d98be3607228b093351115339effa1a17e884a5530b389ceedd062073`  
		Last Modified: Sat, 30 Apr 2022 00:21:18 GMT  
		Size: 868.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchbase:enterprise-6.6.5`

```console
$ docker pull couchbase@sha256:3886eb23092c8e42c9113ae8b3c2913be8e323130a958739c783bc3e3cd7e9d5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `couchbase:enterprise-6.6.5` - linux; amd64

```console
$ docker pull couchbase@sha256:02a08c0d00ee19dac6652145fd6f6afbb243fef8b4edea071ed39c99f68f0495
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **541.2 MB (541151121 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8c7bffdfe1ce5fd50c58e005901ba305dd06b5da3993bae9f5913eb9aea1ddd`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Wed, 02 Feb 2022 02:14:45 GMT
ADD file:3ccf747d646089ed7fbb43c40c45dd43e86f0674115f856efada93c7e4a63624 in / 
# Wed, 02 Feb 2022 02:14:46 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 02:43:34 GMT
LABEL maintainer=docker@couchbase.com
# Wed, 02 Feb 2022 02:46:36 GMT
ARG UPDATE_COMMAND=apt-get update -y -q
# Wed, 02 Feb 2022 02:46:37 GMT
ARG CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Wed, 02 Feb 2022 02:46:46 GMT
# ARGS: CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ${UPDATE_COMMAND}     && apt-get install -y -q wget tzdata       lsof lshw sysstat net-tools numactl bzip2 runit     && ${CLEANUP_COMMAND}
# Wed, 02 Feb 2022 02:46:46 GMT
ARG CB_VERSION=6.6.5
# Wed, 02 Feb 2022 02:46:46 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.5
# Wed, 02 Feb 2022 02:46:46 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_6.6.5-ubuntu20.04_amd64.deb
# Wed, 02 Feb 2022 02:46:47 GMT
ARG CB_SHA256=fb2da1880ea993dc7a5695c6fbe14cde62024d865a71a7d44ab653f0f633d4c6
# Wed, 02 Feb 2022 02:46:47 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Wed, 02 Feb 2022 02:46:48 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.5-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.5 CB_SHA256=fb2da1880ea993dc7a5695c6fbe14cde62024d865a71a7d44ab653f0f633d4c6 CB_VERSION=6.6.5 CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Wed, 02 Feb 2022 02:47:48 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.5-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.5 CB_SHA256=fb2da1880ea993dc7a5695c6fbe14cde62024d865a71a7d44ab653f0f633d4c6 CB_VERSION=6.6.5 CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && export INSTALL_DONT_START_SERVER=1     && wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE     && echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c -     && ${UPDATE_COMMAND}     && apt-get install -y ./$CB_PACKAGE     && rm -f ./$CB_PACKAGE     && ${CLEANUP_COMMAND}     && rm -rf /tmp/* /var/tmp/*
# Wed, 02 Feb 2022 02:47:50 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.5-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.5 CB_SHA256=fb2da1880ea993dc7a5695c6fbe14cde62024d865a71a7d44ab653f0f633d4c6 CB_VERSION=6.6.5 CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Wed, 02 Feb 2022 02:47:50 GMT
COPY file:018fa38d92aa0a4679f57c2d43b5c14547b2c603cab6ec7fd3240af5545472b5 in /etc/service/couchbase-server/run 
# Wed, 02 Feb 2022 02:47:51 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.5-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.5 CB_SHA256=fb2da1880ea993dc7a5695c6fbe14cde62024d865a71a7d44ab653f0f633d4c6 CB_VERSION=6.6.5 CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Wed, 02 Feb 2022 02:47:51 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Wed, 02 Feb 2022 02:47:52 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.5-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.5 CB_SHA256=fb2da1880ea993dc7a5695c6fbe14cde62024d865a71a7d44ab653f0f633d4c6 CB_VERSION=6.6.5 CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ln -s dummy.sh /usr/local/bin/iptables-save     && ln -s dummy.sh /usr/local/bin/lvdisplay     && ln -s dummy.sh /usr/local/bin/vgdisplay     && ln -s dummy.sh /usr/local/bin/pvdisplay
# Wed, 02 Feb 2022 02:47:59 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.5-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.5 CB_SHA256=fb2da1880ea993dc7a5695c6fbe14cde62024d865a71a7d44ab653f0f633d4c6 CB_VERSION=6.6.5 CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -ex     &&  if [ ! -e /opt/couchbase/bin/curl.real ]; then             ${UPDATE_COMMAND};             apt-get install -y chrpath;             chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl;             apt-get remove -y chrpath;             apt-get autoremove -y;             ${CLEANUP_COMMAND};         fi
# Wed, 02 Feb 2022 02:47:59 GMT
COPY file:6e5292e89c7124e038a0d80ea3b942bff1ed578e67a07e764b041ea95b129aa3 in / 
# Wed, 02 Feb 2022 02:48:00 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 02 Feb 2022 02:48:00 GMT
CMD ["couchbase-server"]
# Wed, 02 Feb 2022 02:48:00 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Wed, 02 Feb 2022 02:48:00 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:08c01a0ec47e82ebe2bec112f373d160983a6d1e9e66627f66a3322bc403221b`  
		Last Modified: Wed, 02 Feb 2022 02:16:20 GMT  
		Size: 28.6 MB (28564099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1754ce27a7ccb86d31d56d18a4e72ba9d67be285a916c8bd17248b727560a47d`  
		Last Modified: Wed, 02 Feb 2022 02:54:22 GMT  
		Size: 6.3 MB (6252084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd5f7756f763ab2246a969908f94fa0b42406e43c41ad14c419d0ad54beb50d9`  
		Last Modified: Wed, 02 Feb 2022 02:54:20 GMT  
		Size: 1.8 KB (1828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dbc09136fe05f40c619d016d0bba8dd53e94b083e1744226711ea3057fa8379`  
		Last Modified: Wed, 02 Feb 2022 02:55:16 GMT  
		Size: 505.9 MB (505890801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef8fd0fde82ac5cd771ba6993145c59631f0e463809c2b727bd0056ad5f63665`  
		Last Modified: Wed, 02 Feb 2022 02:54:20 GMT  
		Size: 191.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef8719c5cb0fb42529c032006f2414cd51e3ae277a9a9e8e322c4fd2f5d92e80`  
		Last Modified: Wed, 02 Feb 2022 02:54:20 GMT  
		Size: 743.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad063a0ccee34a72b08b383b143fd7c7f0069884c8a984966f56a6bd38c51f3d`  
		Last Modified: Wed, 02 Feb 2022 02:54:18 GMT  
		Size: 280.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf1ec1e07f8149650f4c98a98a9259281d8fe9725da7995f86c9f57a58ec8dee`  
		Last Modified: Wed, 02 Feb 2022 02:54:18 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efdb27013dd5b6ec10d9b8b8778d61a0573b2146537c7a716824bde5f3650be4`  
		Last Modified: Wed, 02 Feb 2022 02:54:18 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b151da713f459104635e6d2bee7174258be998280138a69ec849ad19260f6129`  
		Last Modified: Wed, 02 Feb 2022 02:54:18 GMT  
		Size: 439.8 KB (439771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3fbf1915f342936bd4612edd42a845a199ff81e6bea379983490571b46ef6fd`  
		Last Modified: Wed, 02 Feb 2022 02:54:18 GMT  
		Size: 868.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchbase:enterprise-7.0.3`

```console
$ docker pull couchbase@sha256:09d0fb59d4f8df68a5a5352bbb172cb41608eb961e1ede38c41b044cb2359461
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `couchbase:enterprise-7.0.3` - linux; amd64

```console
$ docker pull couchbase@sha256:cc0a5a62c8664ba8684335f195650691b6476a99be5849805d5a13ba572ab9e7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **653.6 MB (653562427 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:24f8a22a0df0012dc1a1270128f1a15a4ee18a95e7f7f253b413dd92181cc97a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Fri, 29 Apr 2022 23:20:59 GMT
ADD file:7009ad0ee0bbe5ed7f381792e07347e260e6896aeee0d80597808065120fa96b in / 
# Fri, 29 Apr 2022 23:20:59 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 00:04:47 GMT
LABEL maintainer=docker@couchbase.com
# Sat, 30 Apr 2022 00:04:47 GMT
ARG UPDATE_COMMAND=apt-get update -y -q
# Sat, 30 Apr 2022 00:04:48 GMT
ARG CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Sat, 30 Apr 2022 00:05:04 GMT
# ARGS: CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ${UPDATE_COMMAND}     && apt-get install -y -q wget tzdata       lsof lshw sysstat net-tools numactl bzip2 runit     && ${CLEANUP_COMMAND}
# Sat, 30 Apr 2022 00:05:04 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.3-MP1
# Sat, 30 Apr 2022 00:05:04 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_7.0.3-MP1-ubuntu20.04_amd64.deb
# Sat, 30 Apr 2022 00:05:04 GMT
ARG CB_SHA256=a1bfcc476e01c71a212c2ed5026f24f3df01b3591c24dcf45678fdb2625cfc0f
# Sat, 30 Apr 2022 00:05:04 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Sat, 30 Apr 2022 00:05:05 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.3-MP1-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.3-MP1 CB_SHA256=a1bfcc476e01c71a212c2ed5026f24f3df01b3591c24dcf45678fdb2625cfc0f CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Sat, 30 Apr 2022 00:07:01 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.3-MP1-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.3-MP1 CB_SHA256=a1bfcc476e01c71a212c2ed5026f24f3df01b3591c24dcf45678fdb2625cfc0f CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && export INSTALL_DONT_START_SERVER=1     && wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE     && echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c -     && ${UPDATE_COMMAND}     && apt-get install -y ./$CB_PACKAGE     && rm -f ./$CB_PACKAGE     && ${CLEANUP_COMMAND}     && rm -rf /tmp/* /var/tmp/*
# Sat, 30 Apr 2022 00:07:07 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.3-MP1-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.3-MP1 CB_SHA256=a1bfcc476e01c71a212c2ed5026f24f3df01b3591c24dcf45678fdb2625cfc0f CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Sat, 30 Apr 2022 00:07:07 GMT
COPY file:018fa38d92aa0a4679f57c2d43b5c14547b2c603cab6ec7fd3240af5545472b5 in /etc/service/couchbase-server/run 
# Sat, 30 Apr 2022 00:07:07 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.3-MP1-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.3-MP1 CB_SHA256=a1bfcc476e01c71a212c2ed5026f24f3df01b3591c24dcf45678fdb2625cfc0f CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Sat, 30 Apr 2022 00:07:07 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Sat, 30 Apr 2022 00:07:08 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.3-MP1-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.3-MP1 CB_SHA256=a1bfcc476e01c71a212c2ed5026f24f3df01b3591c24dcf45678fdb2625cfc0f CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ln -s dummy.sh /usr/local/bin/iptables-save     && ln -s dummy.sh /usr/local/bin/lvdisplay     && ln -s dummy.sh /usr/local/bin/vgdisplay     && ln -s dummy.sh /usr/local/bin/pvdisplay
# Sat, 30 Apr 2022 00:07:14 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.3-MP1-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.3-MP1 CB_SHA256=a1bfcc476e01c71a212c2ed5026f24f3df01b3591c24dcf45678fdb2625cfc0f CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -ex     &&  if [ ! -e /opt/couchbase/bin/curl.real ]; then             ${UPDATE_COMMAND};             apt-get install -y chrpath;             chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl;             apt-get remove -y chrpath;             apt-get autoremove -y;             ${CLEANUP_COMMAND};         fi
# Sat, 30 Apr 2022 00:07:14 GMT
COPY file:6e5292e89c7124e038a0d80ea3b942bff1ed578e67a07e764b041ea95b129aa3 in / 
# Sat, 30 Apr 2022 00:07:14 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 30 Apr 2022 00:07:15 GMT
CMD ["couchbase-server"]
# Sat, 30 Apr 2022 00:07:15 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Sat, 30 Apr 2022 00:07:15 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:d5fd17ec1767521cf97f61568096bfc9a7cd9c2d149576a7b43930c5a97062b0`  
		Last Modified: Thu, 28 Apr 2022 03:03:21 GMT  
		Size: 28.6 MB (28566230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76937b0923f63ef62ef0ce2435f73244f7f909cc74136aba1228f2e2574af748`  
		Last Modified: Sat, 30 Apr 2022 00:18:06 GMT  
		Size: 6.3 MB (6250617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce99684904adf2c3f56e5d7abd675e5cf6a024381ea64a827e805e2022974da6`  
		Last Modified: Sat, 30 Apr 2022 00:18:05 GMT  
		Size: 1.8 KB (1835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff533d3886c8143e80c8fcce9834656e1796453ca5f6e579442e59e644fb9aa8`  
		Last Modified: Sat, 30 Apr 2022 00:19:09 GMT  
		Size: 618.3 MB (618297660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:244f8c789e91a9b9c853463ba29dfb9da147c72b8d9bf54e5e3b0b34ae85d84a`  
		Last Modified: Sat, 30 Apr 2022 00:18:05 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ac7ffc32bcefda82cafad3d09e24ff3bb1643231bf1c5df473999927f9a0029`  
		Last Modified: Sat, 30 Apr 2022 00:18:05 GMT  
		Size: 736.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fbe28691c5e53c547e3f6750a7300ccb0f093986c50167e69281f51db18b2b2`  
		Last Modified: Sat, 30 Apr 2022 00:18:02 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0b46d9ecfa389b345724069f06b58b43916e7ad0d55d6b757729079a2e77337`  
		Last Modified: Sat, 30 Apr 2022 00:18:02 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a747a0b4e81b2d4a1436f1498f57d42f9ae15b9d4126e6d9ced78261052955c1`  
		Last Modified: Sat, 30 Apr 2022 00:18:03 GMT  
		Size: 217.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e71663811e7ab33e06489f5a666fcc8174db799b918054c69565853d630a8f2`  
		Last Modified: Sat, 30 Apr 2022 00:18:03 GMT  
		Size: 443.6 KB (443560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f20164e41e2fec4dc4897c33ac3ad902b50c2d83da7c0e19a4f85c566323b12`  
		Last Modified: Sat, 30 Apr 2022 00:18:02 GMT  
		Size: 868.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchbase:latest`

```console
$ docker pull couchbase@sha256:09d0fb59d4f8df68a5a5352bbb172cb41608eb961e1ede38c41b044cb2359461
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `couchbase:latest` - linux; amd64

```console
$ docker pull couchbase@sha256:cc0a5a62c8664ba8684335f195650691b6476a99be5849805d5a13ba572ab9e7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **653.6 MB (653562427 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:24f8a22a0df0012dc1a1270128f1a15a4ee18a95e7f7f253b413dd92181cc97a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Fri, 29 Apr 2022 23:20:59 GMT
ADD file:7009ad0ee0bbe5ed7f381792e07347e260e6896aeee0d80597808065120fa96b in / 
# Fri, 29 Apr 2022 23:20:59 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 00:04:47 GMT
LABEL maintainer=docker@couchbase.com
# Sat, 30 Apr 2022 00:04:47 GMT
ARG UPDATE_COMMAND=apt-get update -y -q
# Sat, 30 Apr 2022 00:04:48 GMT
ARG CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Sat, 30 Apr 2022 00:05:04 GMT
# ARGS: CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ${UPDATE_COMMAND}     && apt-get install -y -q wget tzdata       lsof lshw sysstat net-tools numactl bzip2 runit     && ${CLEANUP_COMMAND}
# Sat, 30 Apr 2022 00:05:04 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.3-MP1
# Sat, 30 Apr 2022 00:05:04 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_7.0.3-MP1-ubuntu20.04_amd64.deb
# Sat, 30 Apr 2022 00:05:04 GMT
ARG CB_SHA256=a1bfcc476e01c71a212c2ed5026f24f3df01b3591c24dcf45678fdb2625cfc0f
# Sat, 30 Apr 2022 00:05:04 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Sat, 30 Apr 2022 00:05:05 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.3-MP1-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.3-MP1 CB_SHA256=a1bfcc476e01c71a212c2ed5026f24f3df01b3591c24dcf45678fdb2625cfc0f CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Sat, 30 Apr 2022 00:07:01 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.3-MP1-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.3-MP1 CB_SHA256=a1bfcc476e01c71a212c2ed5026f24f3df01b3591c24dcf45678fdb2625cfc0f CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && export INSTALL_DONT_START_SERVER=1     && wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE     && echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c -     && ${UPDATE_COMMAND}     && apt-get install -y ./$CB_PACKAGE     && rm -f ./$CB_PACKAGE     && ${CLEANUP_COMMAND}     && rm -rf /tmp/* /var/tmp/*
# Sat, 30 Apr 2022 00:07:07 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.3-MP1-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.3-MP1 CB_SHA256=a1bfcc476e01c71a212c2ed5026f24f3df01b3591c24dcf45678fdb2625cfc0f CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Sat, 30 Apr 2022 00:07:07 GMT
COPY file:018fa38d92aa0a4679f57c2d43b5c14547b2c603cab6ec7fd3240af5545472b5 in /etc/service/couchbase-server/run 
# Sat, 30 Apr 2022 00:07:07 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.3-MP1-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.3-MP1 CB_SHA256=a1bfcc476e01c71a212c2ed5026f24f3df01b3591c24dcf45678fdb2625cfc0f CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Sat, 30 Apr 2022 00:07:07 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Sat, 30 Apr 2022 00:07:08 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.3-MP1-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.3-MP1 CB_SHA256=a1bfcc476e01c71a212c2ed5026f24f3df01b3591c24dcf45678fdb2625cfc0f CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ln -s dummy.sh /usr/local/bin/iptables-save     && ln -s dummy.sh /usr/local/bin/lvdisplay     && ln -s dummy.sh /usr/local/bin/vgdisplay     && ln -s dummy.sh /usr/local/bin/pvdisplay
# Sat, 30 Apr 2022 00:07:14 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.3-MP1-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.3-MP1 CB_SHA256=a1bfcc476e01c71a212c2ed5026f24f3df01b3591c24dcf45678fdb2625cfc0f CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -ex     &&  if [ ! -e /opt/couchbase/bin/curl.real ]; then             ${UPDATE_COMMAND};             apt-get install -y chrpath;             chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl;             apt-get remove -y chrpath;             apt-get autoremove -y;             ${CLEANUP_COMMAND};         fi
# Sat, 30 Apr 2022 00:07:14 GMT
COPY file:6e5292e89c7124e038a0d80ea3b942bff1ed578e67a07e764b041ea95b129aa3 in / 
# Sat, 30 Apr 2022 00:07:14 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 30 Apr 2022 00:07:15 GMT
CMD ["couchbase-server"]
# Sat, 30 Apr 2022 00:07:15 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Sat, 30 Apr 2022 00:07:15 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:d5fd17ec1767521cf97f61568096bfc9a7cd9c2d149576a7b43930c5a97062b0`  
		Last Modified: Thu, 28 Apr 2022 03:03:21 GMT  
		Size: 28.6 MB (28566230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76937b0923f63ef62ef0ce2435f73244f7f909cc74136aba1228f2e2574af748`  
		Last Modified: Sat, 30 Apr 2022 00:18:06 GMT  
		Size: 6.3 MB (6250617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce99684904adf2c3f56e5d7abd675e5cf6a024381ea64a827e805e2022974da6`  
		Last Modified: Sat, 30 Apr 2022 00:18:05 GMT  
		Size: 1.8 KB (1835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff533d3886c8143e80c8fcce9834656e1796453ca5f6e579442e59e644fb9aa8`  
		Last Modified: Sat, 30 Apr 2022 00:19:09 GMT  
		Size: 618.3 MB (618297660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:244f8c789e91a9b9c853463ba29dfb9da147c72b8d9bf54e5e3b0b34ae85d84a`  
		Last Modified: Sat, 30 Apr 2022 00:18:05 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ac7ffc32bcefda82cafad3d09e24ff3bb1643231bf1c5df473999927f9a0029`  
		Last Modified: Sat, 30 Apr 2022 00:18:05 GMT  
		Size: 736.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fbe28691c5e53c547e3f6750a7300ccb0f093986c50167e69281f51db18b2b2`  
		Last Modified: Sat, 30 Apr 2022 00:18:02 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0b46d9ecfa389b345724069f06b58b43916e7ad0d55d6b757729079a2e77337`  
		Last Modified: Sat, 30 Apr 2022 00:18:02 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a747a0b4e81b2d4a1436f1498f57d42f9ae15b9d4126e6d9ced78261052955c1`  
		Last Modified: Sat, 30 Apr 2022 00:18:03 GMT  
		Size: 217.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e71663811e7ab33e06489f5a666fcc8174db799b918054c69565853d630a8f2`  
		Last Modified: Sat, 30 Apr 2022 00:18:03 GMT  
		Size: 443.6 KB (443560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f20164e41e2fec4dc4897c33ac3ad902b50c2d83da7c0e19a4f85c566323b12`  
		Last Modified: Sat, 30 Apr 2022 00:18:02 GMT  
		Size: 868.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
