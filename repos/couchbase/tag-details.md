<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `couchbase`

-	[`couchbase:6.0.1`](#couchbase601)
-	[`couchbase:6.0.2`](#couchbase602)
-	[`couchbase:6.0.3`](#couchbase603)
-	[`couchbase:6.0.4`](#couchbase604)
-	[`couchbase:6.0.5`](#couchbase605)
-	[`couchbase:6.5.0`](#couchbase650)
-	[`couchbase:6.5.1`](#couchbase651)
-	[`couchbase:6.6.0`](#couchbase660)
-	[`couchbase:6.6.1`](#couchbase661)
-	[`couchbase:6.6.2`](#couchbase662)
-	[`couchbase:7.0.0-beta`](#couchbase700-beta)
-	[`couchbase:community`](#couchbasecommunity)
-	[`couchbase:community-6.5.0`](#couchbasecommunity-650)
-	[`couchbase:community-6.5.1`](#couchbasecommunity-651)
-	[`couchbase:community-6.6.0`](#couchbasecommunity-660)
-	[`couchbase:community-7.0.0-beta`](#couchbasecommunity-700-beta)
-	[`couchbase:enterprise`](#couchbaseenterprise)
-	[`couchbase:enterprise-6.0.1`](#couchbaseenterprise-601)
-	[`couchbase:enterprise-6.0.2`](#couchbaseenterprise-602)
-	[`couchbase:enterprise-6.0.3`](#couchbaseenterprise-603)
-	[`couchbase:enterprise-6.0.4`](#couchbaseenterprise-604)
-	[`couchbase:enterprise-6.0.5`](#couchbaseenterprise-605)
-	[`couchbase:enterprise-6.5.0`](#couchbaseenterprise-650)
-	[`couchbase:enterprise-6.5.1`](#couchbaseenterprise-651)
-	[`couchbase:enterprise-6.6.0`](#couchbaseenterprise-660)
-	[`couchbase:enterprise-6.6.1`](#couchbaseenterprise-661)
-	[`couchbase:enterprise-6.6.2`](#couchbaseenterprise-662)
-	[`couchbase:enterprise-7.0.0-beta`](#couchbaseenterprise-700-beta)
-	[`couchbase:latest`](#couchbaselatest)

## `couchbase:6.0.1`

```console
$ docker pull couchbase@sha256:8a8ff02997140ad599d86bdda34d3850b70e8ae4c5bbd16ad3ccbd74d6f28f1c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `couchbase:6.0.1` - linux; amd64

```console
$ docker pull couchbase@sha256:c43f4fb868048e12d20013e12446753da51bb2f9fb3175b303ac67a017569c7b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **455.2 MB (455212187 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4640a8f2c7d8cbfe809363c1881b4ed21c91deeb471fea7f15cbbb82a2bd7678`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Tue, 13 Jul 2021 22:29:15 GMT
ADD file:7274ece1917848683250bbeda9eacf6eb7510481cbaa177880e3a60b4133e35b in / 
# Tue, 13 Jul 2021 22:29:15 GMT
CMD ["bash"]
# Tue, 13 Jul 2021 23:56:52 GMT
LABEL maintainer=docker@couchbase.com
# Tue, 13 Jul 2021 23:59:19 GMT
RUN set -x &&     apt-get update &&     apt-get install -yq runit wget chrpath tzdata man     lsof lshw sysstat net-tools numactl python-httplib2 &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Tue, 13 Jul 2021 23:59:21 GMT
RUN if [ ! -x /usr/sbin/runsvdir-start ]; then         cp -a /etc/runit/2 /usr/sbin/runsvdir-start;     fi
# Wed, 14 Jul 2021 00:12:02 GMT
ARG CB_VERSION=6.0.1
# Wed, 14 Jul 2021 00:12:02 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.1
# Wed, 14 Jul 2021 00:12:02 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_6.0.1-ubuntu18.04_amd64.deb
# Wed, 14 Jul 2021 00:12:02 GMT
ARG CB_SHA256=68deed9ba855e2a84500ae99a787c415fc85b4d4dc1140be28ae6f56662bafea
# Wed, 14 Jul 2021 00:12:02 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Wed, 14 Jul 2021 00:12:03 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.1-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.1 CB_SHA256=68deed9ba855e2a84500ae99a787c415fc85b4d4dc1140be28ae6f56662bafea CB_VERSION=6.0.1
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Wed, 14 Jul 2021 00:12:58 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.1-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.1 CB_SHA256=68deed9ba855e2a84500ae99a787c415fc85b4d4dc1140be28ae6f56662bafea CB_VERSION=6.0.1
RUN set -x &&     export INSTALL_DONT_START_SERVER=1 &&     wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE &&     echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - &&     apt-get update &&     apt-get install -y ./$CB_PACKAGE &&     rm -f ./$CB_PACKAGE &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Wed, 14 Jul 2021 00:13:01 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.1-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.1 CB_SHA256=68deed9ba855e2a84500ae99a787c415fc85b4d4dc1140be28ae6f56662bafea CB_VERSION=6.0.1
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Wed, 14 Jul 2021 00:13:02 GMT
COPY file:d6a307209223b2df102f46f07fd186e09fac7114db2c965bb54097d3b4d3b989 in /etc/service/couchbase-server/run 
# Wed, 14 Jul 2021 00:13:03 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.1-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.1 CB_SHA256=68deed9ba855e2a84500ae99a787c415fc85b4d4dc1140be28ae6f56662bafea CB_VERSION=6.0.1
RUN mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Wed, 14 Jul 2021 00:13:03 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Wed, 14 Jul 2021 00:13:04 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.1-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.1 CB_SHA256=68deed9ba855e2a84500ae99a787c415fc85b4d4dc1140be28ae6f56662bafea CB_VERSION=6.0.1
RUN ln -s dummy.sh /usr/local/bin/iptables-save &&     ln -s dummy.sh /usr/local/bin/lvdisplay &&     ln -s dummy.sh /usr/local/bin/vgdisplay &&     ln -s dummy.sh /usr/local/bin/pvdisplay
# Wed, 14 Jul 2021 00:13:05 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.1-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.1 CB_SHA256=68deed9ba855e2a84500ae99a787c415fc85b4d4dc1140be28ae6f56662bafea CB_VERSION=6.0.1
RUN chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl
# Wed, 14 Jul 2021 00:13:05 GMT
COPY file:d816a67f62bfba76d2812cefbe92252afa13f3852775c3e68599df7741e90cb7 in / 
# Wed, 14 Jul 2021 00:13:05 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 14 Jul 2021 00:13:06 GMT
CMD ["couchbase-server"]
# Wed, 14 Jul 2021 00:13:06 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Wed, 14 Jul 2021 00:13:06 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:e7ae86ffe2df0787131a4c49ace1b018fd38d62929b007d86bdd1f825e56a852`  
		Last Modified: Tue, 13 Jul 2021 22:31:03 GMT  
		Size: 26.7 MB (26706145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31fa1d32440e9d869ef3438e5bfc1ad70daed7feb9b3a6d493072814a7eeea31`  
		Last Modified: Wed, 14 Jul 2021 00:19:32 GMT  
		Size: 15.9 MB (15922983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d3525b15f6ce5dff724448cd14b2fc3b4cff8ed696b456b2adf085528b5b2a2`  
		Last Modified: Wed, 14 Jul 2021 00:19:25 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72469b72d916f06e1121875a4727378ce8e398344dd61e579da3d0022b4f1cfe`  
		Last Modified: Wed, 14 Jul 2021 00:27:45 GMT  
		Size: 2.0 KB (1967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e74faa62fbf1d0b232e99e243790e3d245175d846416cc1ec738bce2039b01b6`  
		Last Modified: Wed, 14 Jul 2021 00:28:30 GMT  
		Size: 412.5 MB (412453000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3beaaa08e768bed1f2afbe8bbfa872cbdada91cfcf137379493ffefdcf01d2ad`  
		Last Modified: Wed, 14 Jul 2021 00:27:45 GMT  
		Size: 192.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3514b1349e8e01bb0852f5b739ad43c39ca84603a7ed474d3b0f2d42cc0c56ba`  
		Last Modified: Wed, 14 Jul 2021 00:27:45 GMT  
		Size: 482.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22667dd57035a153fc93b73e7620cd2d4a3d93b4dfaf27fd18fa4420e51d4839`  
		Last Modified: Wed, 14 Jul 2021 00:27:43 GMT  
		Size: 279.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4acae565a322b393595022ffd46a892c759fb8bff66f336be20a85859eb69d1`  
		Last Modified: Wed, 14 Jul 2021 00:27:43 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca61a2cf9c63ee0d58f811dedfcdc21b1450a7300912c4f39623bc94d29ccfdb`  
		Last Modified: Wed, 14 Jul 2021 00:27:43 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38fb7c3ce891142743af0f1d199837fea51349a8e0c0dc97a8ca6e1ff8e1ac68`  
		Last Modified: Wed, 14 Jul 2021 00:27:43 GMT  
		Size: 125.6 KB (125561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7607bacfa9601b6de1181ce26531001ed4e89ffcc99715593147ff8e34bca9f6`  
		Last Modified: Wed, 14 Jul 2021 00:27:43 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchbase:6.0.2`

```console
$ docker pull couchbase@sha256:de9b5c24c995523a83b7dac6f8bfd73ff9a076f9a2f8722eb4d757368718eb25
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `couchbase:6.0.2` - linux; amd64

```console
$ docker pull couchbase@sha256:8e02ada2704dcb26338bb9676552bae57a134806f8498eb6183e5506ba3e037d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **463.4 MB (463382896 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3447021d7164a497e86563e16ad4820b4fea2b0497b535f71b74e15f6cd1cac0`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Tue, 13 Jul 2021 22:29:15 GMT
ADD file:7274ece1917848683250bbeda9eacf6eb7510481cbaa177880e3a60b4133e35b in / 
# Tue, 13 Jul 2021 22:29:15 GMT
CMD ["bash"]
# Tue, 13 Jul 2021 23:56:52 GMT
LABEL maintainer=docker@couchbase.com
# Tue, 13 Jul 2021 23:59:19 GMT
RUN set -x &&     apt-get update &&     apt-get install -yq runit wget chrpath tzdata man     lsof lshw sysstat net-tools numactl python-httplib2 &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Tue, 13 Jul 2021 23:59:21 GMT
RUN if [ ! -x /usr/sbin/runsvdir-start ]; then         cp -a /etc/runit/2 /usr/sbin/runsvdir-start;     fi
# Wed, 14 Jul 2021 00:10:21 GMT
ARG CB_VERSION=6.0.2
# Wed, 14 Jul 2021 00:10:21 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.2
# Wed, 14 Jul 2021 00:10:21 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_6.0.2-ubuntu18.04_amd64.deb
# Wed, 14 Jul 2021 00:10:22 GMT
ARG CB_SHA256=5410a56cefd7a9c624a2d64e474058b43a90e8d66c73fea6b2a8b16a4f6fe14d
# Wed, 14 Jul 2021 00:10:22 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Wed, 14 Jul 2021 00:10:23 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.2-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.2 CB_SHA256=5410a56cefd7a9c624a2d64e474058b43a90e8d66c73fea6b2a8b16a4f6fe14d CB_VERSION=6.0.2
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Wed, 14 Jul 2021 00:11:22 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.2-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.2 CB_SHA256=5410a56cefd7a9c624a2d64e474058b43a90e8d66c73fea6b2a8b16a4f6fe14d CB_VERSION=6.0.2
RUN set -x &&     export INSTALL_DONT_START_SERVER=1 &&     wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE &&     echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - &&     apt-get update &&     apt-get install -y ./$CB_PACKAGE &&     rm -f ./$CB_PACKAGE &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Wed, 14 Jul 2021 00:11:44 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.2-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.2 CB_SHA256=5410a56cefd7a9c624a2d64e474058b43a90e8d66c73fea6b2a8b16a4f6fe14d CB_VERSION=6.0.2
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Wed, 14 Jul 2021 00:11:45 GMT
COPY file:d6a307209223b2df102f46f07fd186e09fac7114db2c965bb54097d3b4d3b989 in /etc/service/couchbase-server/run 
# Wed, 14 Jul 2021 00:11:46 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.2-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.2 CB_SHA256=5410a56cefd7a9c624a2d64e474058b43a90e8d66c73fea6b2a8b16a4f6fe14d CB_VERSION=6.0.2
RUN mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Wed, 14 Jul 2021 00:11:46 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Wed, 14 Jul 2021 00:11:47 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.2-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.2 CB_SHA256=5410a56cefd7a9c624a2d64e474058b43a90e8d66c73fea6b2a8b16a4f6fe14d CB_VERSION=6.0.2
RUN ln -s dummy.sh /usr/local/bin/iptables-save &&     ln -s dummy.sh /usr/local/bin/lvdisplay &&     ln -s dummy.sh /usr/local/bin/vgdisplay &&     ln -s dummy.sh /usr/local/bin/pvdisplay
# Wed, 14 Jul 2021 00:11:48 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.2-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.2 CB_SHA256=5410a56cefd7a9c624a2d64e474058b43a90e8d66c73fea6b2a8b16a4f6fe14d CB_VERSION=6.0.2
RUN chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl
# Wed, 14 Jul 2021 00:11:48 GMT
COPY file:d816a67f62bfba76d2812cefbe92252afa13f3852775c3e68599df7741e90cb7 in / 
# Wed, 14 Jul 2021 00:11:48 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 14 Jul 2021 00:11:48 GMT
CMD ["couchbase-server"]
# Wed, 14 Jul 2021 00:11:49 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Wed, 14 Jul 2021 00:11:49 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:e7ae86ffe2df0787131a4c49ace1b018fd38d62929b007d86bdd1f825e56a852`  
		Last Modified: Tue, 13 Jul 2021 22:31:03 GMT  
		Size: 26.7 MB (26706145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31fa1d32440e9d869ef3438e5bfc1ad70daed7feb9b3a6d493072814a7eeea31`  
		Last Modified: Wed, 14 Jul 2021 00:19:32 GMT  
		Size: 15.9 MB (15922983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d3525b15f6ce5dff724448cd14b2fc3b4cff8ed696b456b2adf085528b5b2a2`  
		Last Modified: Wed, 14 Jul 2021 00:19:25 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:603249a8f1cf0ebf8e676e6ef0d97a7b00c518fe588dc65c9f16b286de5d3b36`  
		Last Modified: Wed, 14 Jul 2021 00:26:49 GMT  
		Size: 2.0 KB (1969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2d9534b3cb8baf23f515c8f4b7762851a6f2e2df6e333c9401160236fa48652`  
		Last Modified: Wed, 14 Jul 2021 00:27:30 GMT  
		Size: 420.6 MB (420623712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8283ee9491704f4dae8db18fcb0eda7f2a3af0fd8514d793d9e217559047cec`  
		Last Modified: Wed, 14 Jul 2021 00:26:48 GMT  
		Size: 192.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20342722cce538c85079a8afa2a8f5a029ae981ec1a690f5ed86b8c2b8af0342`  
		Last Modified: Wed, 14 Jul 2021 00:26:48 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4afda51548d5dc06330535b173566c9209c2c3f0c6d7e43b6ae194f5bfe71253`  
		Last Modified: Wed, 14 Jul 2021 00:26:46 GMT  
		Size: 279.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0989364a544fa2d17eb0cf25aca82520310b7579e1156302d1d658d392a52f7`  
		Last Modified: Wed, 14 Jul 2021 00:26:46 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:061c137e4d88835c0cb2dd20e925a1b684f62e175d060d5ec379619f3409740f`  
		Last Modified: Wed, 14 Jul 2021 00:26:46 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05303718e4140b55b907377dfeba8672fd0ca32a0139a191030d221f374aa84f`  
		Last Modified: Wed, 14 Jul 2021 00:26:46 GMT  
		Size: 125.6 KB (125561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9eb0f57abd2ba900921d5e40f9576d7e21f0a593e230604d7de7dcce7088837`  
		Last Modified: Wed, 14 Jul 2021 00:26:46 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchbase:6.0.3`

```console
$ docker pull couchbase@sha256:2ca33951fcd428a03147f116657c80f76dc896bf5a50d905343da158440aa8fc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `couchbase:6.0.3` - linux; amd64

```console
$ docker pull couchbase@sha256:324edff57c7aee2a917507acbdbc43474bbb02dbfea393467fae937cafe810bf
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **465.9 MB (465906748 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c47f7d8e17933f975153e288308212811e5463ecef3aed61207441a5aff8a1fd`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Tue, 13 Jul 2021 22:29:15 GMT
ADD file:7274ece1917848683250bbeda9eacf6eb7510481cbaa177880e3a60b4133e35b in / 
# Tue, 13 Jul 2021 22:29:15 GMT
CMD ["bash"]
# Tue, 13 Jul 2021 23:56:52 GMT
LABEL maintainer=docker@couchbase.com
# Tue, 13 Jul 2021 23:59:19 GMT
RUN set -x &&     apt-get update &&     apt-get install -yq runit wget chrpath tzdata man     lsof lshw sysstat net-tools numactl python-httplib2 &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Tue, 13 Jul 2021 23:59:21 GMT
RUN if [ ! -x /usr/sbin/runsvdir-start ]; then         cp -a /etc/runit/2 /usr/sbin/runsvdir-start;     fi
# Wed, 14 Jul 2021 00:09:09 GMT
ARG CB_VERSION=6.0.3
# Wed, 14 Jul 2021 00:09:10 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.3
# Wed, 14 Jul 2021 00:09:10 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_6.0.3-ubuntu18.04_amd64.deb
# Wed, 14 Jul 2021 00:09:10 GMT
ARG CB_SHA256=8ee814ea8d99141de5493a6a24423c6a5dc4e01b8393dce87ca1639630315382
# Wed, 14 Jul 2021 00:09:10 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Wed, 14 Jul 2021 00:09:11 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.3-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.3 CB_SHA256=8ee814ea8d99141de5493a6a24423c6a5dc4e01b8393dce87ca1639630315382 CB_VERSION=6.0.3
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Wed, 14 Jul 2021 00:10:10 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.3-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.3 CB_SHA256=8ee814ea8d99141de5493a6a24423c6a5dc4e01b8393dce87ca1639630315382 CB_VERSION=6.0.3
RUN set -x &&     export INSTALL_DONT_START_SERVER=1 &&     wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE &&     echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - &&     apt-get update &&     apt-get install -y ./$CB_PACKAGE &&     rm -f ./$CB_PACKAGE &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Wed, 14 Jul 2021 00:10:13 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.3-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.3 CB_SHA256=8ee814ea8d99141de5493a6a24423c6a5dc4e01b8393dce87ca1639630315382 CB_VERSION=6.0.3
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Wed, 14 Jul 2021 00:10:14 GMT
COPY file:d6a307209223b2df102f46f07fd186e09fac7114db2c965bb54097d3b4d3b989 in /etc/service/couchbase-server/run 
# Wed, 14 Jul 2021 00:10:15 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.3-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.3 CB_SHA256=8ee814ea8d99141de5493a6a24423c6a5dc4e01b8393dce87ca1639630315382 CB_VERSION=6.0.3
RUN mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Wed, 14 Jul 2021 00:10:15 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Wed, 14 Jul 2021 00:10:16 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.3-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.3 CB_SHA256=8ee814ea8d99141de5493a6a24423c6a5dc4e01b8393dce87ca1639630315382 CB_VERSION=6.0.3
RUN ln -s dummy.sh /usr/local/bin/iptables-save &&     ln -s dummy.sh /usr/local/bin/lvdisplay &&     ln -s dummy.sh /usr/local/bin/vgdisplay &&     ln -s dummy.sh /usr/local/bin/pvdisplay
# Wed, 14 Jul 2021 00:10:17 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.3-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.3 CB_SHA256=8ee814ea8d99141de5493a6a24423c6a5dc4e01b8393dce87ca1639630315382 CB_VERSION=6.0.3
RUN chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl
# Wed, 14 Jul 2021 00:10:17 GMT
COPY file:d816a67f62bfba76d2812cefbe92252afa13f3852775c3e68599df7741e90cb7 in / 
# Wed, 14 Jul 2021 00:10:17 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 14 Jul 2021 00:10:17 GMT
CMD ["couchbase-server"]
# Wed, 14 Jul 2021 00:10:18 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Wed, 14 Jul 2021 00:10:18 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:e7ae86ffe2df0787131a4c49ace1b018fd38d62929b007d86bdd1f825e56a852`  
		Last Modified: Tue, 13 Jul 2021 22:31:03 GMT  
		Size: 26.7 MB (26706145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31fa1d32440e9d869ef3438e5bfc1ad70daed7feb9b3a6d493072814a7eeea31`  
		Last Modified: Wed, 14 Jul 2021 00:19:32 GMT  
		Size: 15.9 MB (15922983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d3525b15f6ce5dff724448cd14b2fc3b4cff8ed696b456b2adf085528b5b2a2`  
		Last Modified: Wed, 14 Jul 2021 00:19:25 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a87df52b5ea3cc49700b53c210b5ebe99ddf87056405f040593913d9f8c47599`  
		Last Modified: Wed, 14 Jul 2021 00:25:53 GMT  
		Size: 2.0 KB (1971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efe050fd8c96c1333e825325cf2a385fb2249e29d2a86295a8e44fd26e78dd1e`  
		Last Modified: Wed, 14 Jul 2021 00:26:34 GMT  
		Size: 423.1 MB (423147566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8af8a25dfae3cd32c9b437073247d6a3f79fc9f14a2c35adb730a5503f9e60c9`  
		Last Modified: Wed, 14 Jul 2021 00:25:53 GMT  
		Size: 191.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02bc5e818d0b081fb9790b5b3167453695cd69f167069b9b06ca6d70bfab8cf7`  
		Last Modified: Wed, 14 Jul 2021 00:25:53 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ccf28a52d832dcbb2337c7c99775f02c93935a45ce1dea2ec475bd16c435a5f`  
		Last Modified: Wed, 14 Jul 2021 00:25:51 GMT  
		Size: 279.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cd5d7cd6e13a56c0d0b842454f92f5cc3dd403a7291e11f4cbf93ff55ec0ab1`  
		Last Modified: Wed, 14 Jul 2021 00:25:51 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afa89f6d24da70e562ae6fe8dfcc487049d11f579e6030507ec9c9f5a424be6c`  
		Last Modified: Wed, 14 Jul 2021 00:25:51 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c9a21894ad164f0f760611f64405966f7ae780078ca8608fe9ae565cf566550`  
		Last Modified: Wed, 14 Jul 2021 00:25:51 GMT  
		Size: 125.6 KB (125558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90487eb210f8d4f901f84dc0b9e61ccd2137b3c9d647fa38d7b708b44591b958`  
		Last Modified: Wed, 14 Jul 2021 00:25:51 GMT  
		Size: 858.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchbase:6.0.4`

```console
$ docker pull couchbase@sha256:b9898e94785b49ddba89e600193dde03e616a41e01676a743dbfb57f4c4d8110
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `couchbase:6.0.4` - linux; amd64

```console
$ docker pull couchbase@sha256:96f5f253b16b7bfef403f349c39c890efb991a3c76c53b8ff5df4e4554b8adc9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **467.2 MB (467173553 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3618f344592fa4de4ecc882a29a993cf8b8b094c2fb7f67ccf477d57095635b4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Tue, 13 Jul 2021 22:29:15 GMT
ADD file:7274ece1917848683250bbeda9eacf6eb7510481cbaa177880e3a60b4133e35b in / 
# Tue, 13 Jul 2021 22:29:15 GMT
CMD ["bash"]
# Tue, 13 Jul 2021 23:56:52 GMT
LABEL maintainer=docker@couchbase.com
# Tue, 13 Jul 2021 23:59:19 GMT
RUN set -x &&     apt-get update &&     apt-get install -yq runit wget chrpath tzdata man     lsof lshw sysstat net-tools numactl python-httplib2 &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Tue, 13 Jul 2021 23:59:21 GMT
RUN if [ ! -x /usr/sbin/runsvdir-start ]; then         cp -a /etc/runit/2 /usr/sbin/runsvdir-start;     fi
# Wed, 14 Jul 2021 00:07:57 GMT
ARG CB_VERSION=6.0.4
# Wed, 14 Jul 2021 00:07:58 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.4
# Wed, 14 Jul 2021 00:07:58 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_6.0.4-ubuntu18.04_amd64.deb
# Wed, 14 Jul 2021 00:07:58 GMT
ARG CB_SHA256=7dbe8dd074f9cabea69468ea488f9ffc19c04dab8fc2e98c937fa32704982aff
# Wed, 14 Jul 2021 00:07:58 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Wed, 14 Jul 2021 00:07:59 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.4-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.4 CB_SHA256=7dbe8dd074f9cabea69468ea488f9ffc19c04dab8fc2e98c937fa32704982aff CB_VERSION=6.0.4
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Wed, 14 Jul 2021 00:08:57 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.4-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.4 CB_SHA256=7dbe8dd074f9cabea69468ea488f9ffc19c04dab8fc2e98c937fa32704982aff CB_VERSION=6.0.4
RUN set -x &&     export INSTALL_DONT_START_SERVER=1 &&     wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE &&     echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - &&     apt-get update &&     apt-get install -y ./$CB_PACKAGE &&     rm -f ./$CB_PACKAGE &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Wed, 14 Jul 2021 00:09:01 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.4-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.4 CB_SHA256=7dbe8dd074f9cabea69468ea488f9ffc19c04dab8fc2e98c937fa32704982aff CB_VERSION=6.0.4
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Wed, 14 Jul 2021 00:09:01 GMT
COPY file:d6a307209223b2df102f46f07fd186e09fac7114db2c965bb54097d3b4d3b989 in /etc/service/couchbase-server/run 
# Wed, 14 Jul 2021 00:09:02 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.4-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.4 CB_SHA256=7dbe8dd074f9cabea69468ea488f9ffc19c04dab8fc2e98c937fa32704982aff CB_VERSION=6.0.4
RUN mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Wed, 14 Jul 2021 00:09:02 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Wed, 14 Jul 2021 00:09:03 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.4-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.4 CB_SHA256=7dbe8dd074f9cabea69468ea488f9ffc19c04dab8fc2e98c937fa32704982aff CB_VERSION=6.0.4
RUN ln -s dummy.sh /usr/local/bin/iptables-save &&     ln -s dummy.sh /usr/local/bin/lvdisplay &&     ln -s dummy.sh /usr/local/bin/vgdisplay &&     ln -s dummy.sh /usr/local/bin/pvdisplay
# Wed, 14 Jul 2021 00:09:04 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.4-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.4 CB_SHA256=7dbe8dd074f9cabea69468ea488f9ffc19c04dab8fc2e98c937fa32704982aff CB_VERSION=6.0.4
RUN chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl
# Wed, 14 Jul 2021 00:09:04 GMT
COPY file:d816a67f62bfba76d2812cefbe92252afa13f3852775c3e68599df7741e90cb7 in / 
# Wed, 14 Jul 2021 00:09:05 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 14 Jul 2021 00:09:05 GMT
CMD ["couchbase-server"]
# Wed, 14 Jul 2021 00:09:05 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Wed, 14 Jul 2021 00:09:05 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:e7ae86ffe2df0787131a4c49ace1b018fd38d62929b007d86bdd1f825e56a852`  
		Last Modified: Tue, 13 Jul 2021 22:31:03 GMT  
		Size: 26.7 MB (26706145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31fa1d32440e9d869ef3438e5bfc1ad70daed7feb9b3a6d493072814a7eeea31`  
		Last Modified: Wed, 14 Jul 2021 00:19:32 GMT  
		Size: 15.9 MB (15922983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d3525b15f6ce5dff724448cd14b2fc3b4cff8ed696b456b2adf085528b5b2a2`  
		Last Modified: Wed, 14 Jul 2021 00:19:25 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf3a3b7c6bc46ae495064fe52418dd279fc078f7a5b5559856421ec70a8ad99a`  
		Last Modified: Wed, 14 Jul 2021 00:24:58 GMT  
		Size: 2.0 KB (1967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba1cb08d8fd0ea9125e7f2d87cf3bd3f1ee8e2eb8785405e904163c7af85c13d`  
		Last Modified: Wed, 14 Jul 2021 00:25:39 GMT  
		Size: 424.4 MB (424414373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64dbdc5cb335c4fa20a1529faa766256f539e06f80663d2c3c6ac8d2e4e36379`  
		Last Modified: Wed, 14 Jul 2021 00:24:58 GMT  
		Size: 191.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f865105c048695dd483dfceb73c7027a13cc43c5b67a71ec9ce517ad7e869c8`  
		Last Modified: Wed, 14 Jul 2021 00:24:58 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fc175912ab464cab161e719cbcb7cad5f1ec658c6d06b6cf8690ba64eaf9368`  
		Last Modified: Wed, 14 Jul 2021 00:24:55 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc110d3d902ab016c5da32e4acf88ee20c51e7d5ae85b38d4199a74e6b673054`  
		Last Modified: Wed, 14 Jul 2021 00:24:56 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6ca51cc5fe51f0ca1792ce4e4a1e5d7ab3c454ecd5c8e94d6821cb50b08567b`  
		Last Modified: Wed, 14 Jul 2021 00:24:55 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fb188386e971655790488f4d29d36409eb1237a69784fe157f06cb6be00bbde`  
		Last Modified: Wed, 14 Jul 2021 00:24:56 GMT  
		Size: 125.6 KB (125563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57b04265b4d19130c58c8c2a29aa008d44939493416384508cee4656d92556c4`  
		Last Modified: Wed, 14 Jul 2021 00:24:55 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchbase:6.0.5`

```console
$ docker pull couchbase@sha256:c2794e735530e77e4001b1743f4de9249140987d29aa27bd3208490b6148feac
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `couchbase:6.0.5` - linux; amd64

```console
$ docker pull couchbase@sha256:6ac872346667262e6edc81280bd419cf62d39f56841fd5f984025003bfbeb4c9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **466.1 MB (466121401 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:75b0afca95bffb603ee6a94f16eb407d7d007aec985f78c3f19ca840f73039ae`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Tue, 13 Jul 2021 22:29:15 GMT
ADD file:7274ece1917848683250bbeda9eacf6eb7510481cbaa177880e3a60b4133e35b in / 
# Tue, 13 Jul 2021 22:29:15 GMT
CMD ["bash"]
# Tue, 13 Jul 2021 23:56:52 GMT
LABEL maintainer=docker@couchbase.com
# Tue, 13 Jul 2021 23:59:19 GMT
RUN set -x &&     apt-get update &&     apt-get install -yq runit wget chrpath tzdata man     lsof lshw sysstat net-tools numactl python-httplib2 &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Tue, 13 Jul 2021 23:59:21 GMT
RUN if [ ! -x /usr/sbin/runsvdir-start ]; then         cp -a /etc/runit/2 /usr/sbin/runsvdir-start;     fi
# Tue, 13 Jul 2021 23:59:21 GMT
ARG CB_VERSION=6.0.5
# Tue, 13 Jul 2021 23:59:21 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.5
# Tue, 13 Jul 2021 23:59:21 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_6.0.5-ubuntu18.04_amd64.deb
# Tue, 13 Jul 2021 23:59:22 GMT
ARG CB_SHA256=6b152590867a58d771cffc22774d3cd66c916defcbeeeb339aca8d0a8e6d7f8d
# Tue, 13 Jul 2021 23:59:22 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Tue, 13 Jul 2021 23:59:23 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.5-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.5 CB_SHA256=6b152590867a58d771cffc22774d3cd66c916defcbeeeb339aca8d0a8e6d7f8d CB_VERSION=6.0.5
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Wed, 14 Jul 2021 00:00:43 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.5-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.5 CB_SHA256=6b152590867a58d771cffc22774d3cd66c916defcbeeeb339aca8d0a8e6d7f8d CB_VERSION=6.0.5
RUN set -x &&     export INSTALL_DONT_START_SERVER=1 &&     wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE &&     echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - &&     apt-get update &&     apt-get install -y ./$CB_PACKAGE &&     rm -f ./$CB_PACKAGE &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Wed, 14 Jul 2021 00:00:48 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.5-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.5 CB_SHA256=6b152590867a58d771cffc22774d3cd66c916defcbeeeb339aca8d0a8e6d7f8d CB_VERSION=6.0.5
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Wed, 14 Jul 2021 00:00:48 GMT
COPY file:d6a307209223b2df102f46f07fd186e09fac7114db2c965bb54097d3b4d3b989 in /etc/service/couchbase-server/run 
# Wed, 14 Jul 2021 00:00:51 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.5-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.5 CB_SHA256=6b152590867a58d771cffc22774d3cd66c916defcbeeeb339aca8d0a8e6d7f8d CB_VERSION=6.0.5
RUN mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Wed, 14 Jul 2021 00:00:51 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Wed, 14 Jul 2021 00:00:53 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.5-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.5 CB_SHA256=6b152590867a58d771cffc22774d3cd66c916defcbeeeb339aca8d0a8e6d7f8d CB_VERSION=6.0.5
RUN ln -s dummy.sh /usr/local/bin/iptables-save &&     ln -s dummy.sh /usr/local/bin/lvdisplay &&     ln -s dummy.sh /usr/local/bin/vgdisplay &&     ln -s dummy.sh /usr/local/bin/pvdisplay
# Wed, 14 Jul 2021 00:00:55 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.5-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.5 CB_SHA256=6b152590867a58d771cffc22774d3cd66c916defcbeeeb339aca8d0a8e6d7f8d CB_VERSION=6.0.5
RUN chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl
# Wed, 14 Jul 2021 00:00:56 GMT
COPY file:d816a67f62bfba76d2812cefbe92252afa13f3852775c3e68599df7741e90cb7 in / 
# Wed, 14 Jul 2021 00:00:56 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 14 Jul 2021 00:00:56 GMT
CMD ["couchbase-server"]
# Wed, 14 Jul 2021 00:00:57 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Wed, 14 Jul 2021 00:00:57 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:e7ae86ffe2df0787131a4c49ace1b018fd38d62929b007d86bdd1f825e56a852`  
		Last Modified: Tue, 13 Jul 2021 22:31:03 GMT  
		Size: 26.7 MB (26706145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31fa1d32440e9d869ef3438e5bfc1ad70daed7feb9b3a6d493072814a7eeea31`  
		Last Modified: Wed, 14 Jul 2021 00:19:32 GMT  
		Size: 15.9 MB (15922983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d3525b15f6ce5dff724448cd14b2fc3b4cff8ed696b456b2adf085528b5b2a2`  
		Last Modified: Wed, 14 Jul 2021 00:19:25 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5037ab8e061c8ac8dad72c6524e345936c64f4b921675a172bc0e5010f417518`  
		Last Modified: Wed, 14 Jul 2021 00:19:25 GMT  
		Size: 2.0 KB (1965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:135a2ec4d68ab3615eee5adf0ba4849c3acded84ea71e89f3c4f90f3f2b46000`  
		Last Modified: Wed, 14 Jul 2021 00:20:06 GMT  
		Size: 423.4 MB (423362229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6252f42dee8be81dbc56a7d42819069889a1b6f05ffc9c7ae2bfb0fc5a96d21e`  
		Last Modified: Wed, 14 Jul 2021 00:19:25 GMT  
		Size: 192.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:367d2d96dc36d6ec07050b65770fc6156bff82ccbc4ae7cdbc9f1da33cc4d7c6`  
		Last Modified: Wed, 14 Jul 2021 00:19:25 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25344e400b0d1939e6d3604c68eb98da50e8ec09ba94b679cb5371d705c7fcf6`  
		Last Modified: Wed, 14 Jul 2021 00:19:22 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:433d9be8d5ce4f880ffb7c99b47c03e88c5d03f00da401df464f2d6c1b2beb0e`  
		Last Modified: Wed, 14 Jul 2021 00:19:22 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3a01dae8f15dac3896e3330d6a1fbf8c72daf2f103a232c6f3980fcd8eebff8`  
		Last Modified: Wed, 14 Jul 2021 00:19:22 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12f0a82152aca4cbcba222cc0a294adfd643c40c83ba98369a78679d25e669db`  
		Last Modified: Wed, 14 Jul 2021 00:19:22 GMT  
		Size: 125.6 KB (125558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f758726bd5203a0462981dad419faed39c665522bdf6c589c50b0ab5de2f4fc`  
		Last Modified: Wed, 14 Jul 2021 00:19:22 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchbase:6.5.0`

```console
$ docker pull couchbase@sha256:1c2654f480ef8427c0362829bdb0e6bda8645489ae87ddf0c7eb4424d43926de
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `couchbase:6.5.0` - linux; amd64

```console
$ docker pull couchbase@sha256:0ba3a6d5d0b1f8b73573443c85cfb167c56d785e5939fdeb85e19bfe853f7a3d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **542.2 MB (542234395 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b9e0bc7184a3f3607e09fb1c6277bef11bb409d1102601eb2315679ea469fcda`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Tue, 13 Jul 2021 22:29:15 GMT
ADD file:7274ece1917848683250bbeda9eacf6eb7510481cbaa177880e3a60b4133e35b in / 
# Tue, 13 Jul 2021 22:29:15 GMT
CMD ["bash"]
# Tue, 13 Jul 2021 23:56:52 GMT
LABEL maintainer=docker@couchbase.com
# Tue, 13 Jul 2021 23:57:29 GMT
RUN set -x &&     apt-get update &&     apt-get install -yq runit wget chrpath tzdata man     lsof lshw sysstat net-tools numactl bzip2 &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Tue, 13 Jul 2021 23:57:32 GMT
RUN if [ ! -x /usr/sbin/runsvdir-start ]; then         cp -a /etc/runit/2 /usr/sbin/runsvdir-start;     fi
# Wed, 14 Jul 2021 00:06:32 GMT
ARG CB_VERSION=6.5.0
# Wed, 14 Jul 2021 00:06:32 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/6.5.0
# Wed, 14 Jul 2021 00:06:32 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_6.5.0-ubuntu18.04_amd64.deb
# Wed, 14 Jul 2021 00:06:33 GMT
ARG CB_SHA256=b4cafdc048b0caba85c24b90e6823e9ec2adc32061cafc527ddc99d706d6bc05
# Wed, 14 Jul 2021 00:06:33 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Wed, 14 Jul 2021 00:06:34 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.5.0-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.5.0 CB_SHA256=b4cafdc048b0caba85c24b90e6823e9ec2adc32061cafc527ddc99d706d6bc05 CB_VERSION=6.5.0
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Wed, 14 Jul 2021 00:07:40 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.5.0-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.5.0 CB_SHA256=b4cafdc048b0caba85c24b90e6823e9ec2adc32061cafc527ddc99d706d6bc05 CB_VERSION=6.5.0
RUN set -x &&     export INSTALL_DONT_START_SERVER=1 &&     wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE &&     echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - &&     apt-get update &&     apt-get install -y ./$CB_PACKAGE &&     rm -f ./$CB_PACKAGE &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Wed, 14 Jul 2021 00:07:44 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.5.0-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.5.0 CB_SHA256=b4cafdc048b0caba85c24b90e6823e9ec2adc32061cafc527ddc99d706d6bc05 CB_VERSION=6.5.0
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Wed, 14 Jul 2021 00:07:44 GMT
COPY file:d6a307209223b2df102f46f07fd186e09fac7114db2c965bb54097d3b4d3b989 in /etc/service/couchbase-server/run 
# Wed, 14 Jul 2021 00:07:45 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.5.0-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.5.0 CB_SHA256=b4cafdc048b0caba85c24b90e6823e9ec2adc32061cafc527ddc99d706d6bc05 CB_VERSION=6.5.0
RUN mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Wed, 14 Jul 2021 00:07:46 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Wed, 14 Jul 2021 00:07:47 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.5.0-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.5.0 CB_SHA256=b4cafdc048b0caba85c24b90e6823e9ec2adc32061cafc527ddc99d706d6bc05 CB_VERSION=6.5.0
RUN ln -s dummy.sh /usr/local/bin/iptables-save &&     ln -s dummy.sh /usr/local/bin/lvdisplay &&     ln -s dummy.sh /usr/local/bin/vgdisplay &&     ln -s dummy.sh /usr/local/bin/pvdisplay
# Wed, 14 Jul 2021 00:07:48 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.5.0-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.5.0 CB_SHA256=b4cafdc048b0caba85c24b90e6823e9ec2adc32061cafc527ddc99d706d6bc05 CB_VERSION=6.5.0
RUN chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl
# Wed, 14 Jul 2021 00:07:48 GMT
COPY file:d816a67f62bfba76d2812cefbe92252afa13f3852775c3e68599df7741e90cb7 in / 
# Wed, 14 Jul 2021 00:07:48 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 14 Jul 2021 00:07:49 GMT
CMD ["couchbase-server"]
# Wed, 14 Jul 2021 00:07:49 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Wed, 14 Jul 2021 00:07:49 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:e7ae86ffe2df0787131a4c49ace1b018fd38d62929b007d86bdd1f825e56a852`  
		Last Modified: Tue, 13 Jul 2021 22:31:03 GMT  
		Size: 26.7 MB (26706145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f13c80c516e182839d6e6d6f7bc46ca9d41b722a2b3187d09071f91c78769b0e`  
		Last Modified: Wed, 14 Jul 2021 00:18:37 GMT  
		Size: 7.4 MB (7373539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fec6a0ae3c3d8baa9b4f7ebc733acffb0a42e2e7a0d032ceba2a7f11936f3e3`  
		Last Modified: Wed, 14 Jul 2021 00:18:32 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac6ea85b7eae8b65ce8bf5a4eb8113662d048fe6e441bf9a4991e60bb7dd7885`  
		Last Modified: Wed, 14 Jul 2021 00:23:48 GMT  
		Size: 2.0 KB (1967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a8011aa8d5035f6fc3dbe7d7cb0b105c9b577965b9c71df01c62496289b2b10`  
		Last Modified: Wed, 14 Jul 2021 00:24:42 GMT  
		Size: 508.0 MB (508032027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02ff4341f265f333cc4ceb54256f2d610e00758f05d923a042917ee66ad70511`  
		Last Modified: Wed, 14 Jul 2021 00:23:48 GMT  
		Size: 190.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b658f87e1af28571f5360142615d3d834cb1522744e1b723fbaabfe422d6379`  
		Last Modified: Wed, 14 Jul 2021 00:23:48 GMT  
		Size: 480.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20d662cda6464532e5fb76a7e6360315fe834be02bd469181a85c415a5290f0d`  
		Last Modified: Wed, 14 Jul 2021 00:23:45 GMT  
		Size: 280.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7922c732bdc393a6987356e98912481476b4263fa2b1b28d8d7909f2449509d`  
		Last Modified: Wed, 14 Jul 2021 00:23:45 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6636355b99c052dac173273a1e5ee36763b074a24efbf5b29a671a74c3fd2ef`  
		Last Modified: Wed, 14 Jul 2021 00:23:45 GMT  
		Size: 217.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71b3aaa3c22f7b1f6f546d2d79ca875bbf38e4b50142dba6a3b2a81398b58ab6`  
		Last Modified: Wed, 14 Jul 2021 00:23:45 GMT  
		Size: 118.2 KB (118191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5b9899b2afec881cb60078d0c8957eb38376978a5458875a029f6073abeaca7`  
		Last Modified: Wed, 14 Jul 2021 00:23:45 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchbase:6.5.1`

```console
$ docker pull couchbase@sha256:4d349e3b91534085e4b13c9b4e0ed589f522d756ee4d59d763fa55cb72e5e6dc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `couchbase:6.5.1` - linux; amd64

```console
$ docker pull couchbase@sha256:cbfc1f569121926922fc536dd0bb9c6eb28fb22c8ff1ce60c28a35adf3a8122a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **501.5 MB (501508958 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8fd049d1538297e8768ff6ebd7a142eccc58415a7575324e34c3a44c38d57418`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Tue, 13 Jul 2021 22:29:15 GMT
ADD file:7274ece1917848683250bbeda9eacf6eb7510481cbaa177880e3a60b4133e35b in / 
# Tue, 13 Jul 2021 22:29:15 GMT
CMD ["bash"]
# Tue, 13 Jul 2021 23:56:52 GMT
LABEL maintainer=docker@couchbase.com
# Tue, 13 Jul 2021 23:57:29 GMT
RUN set -x &&     apt-get update &&     apt-get install -yq runit wget chrpath tzdata man     lsof lshw sysstat net-tools numactl bzip2 &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Tue, 13 Jul 2021 23:57:32 GMT
RUN if [ ! -x /usr/sbin/runsvdir-start ]; then         cp -a /etc/runit/2 /usr/sbin/runsvdir-start;     fi
# Wed, 14 Jul 2021 00:04:52 GMT
ARG CB_VERSION=6.5.1
# Wed, 14 Jul 2021 00:04:52 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/6.5.1
# Wed, 14 Jul 2021 00:04:52 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_6.5.1-ubuntu18.04_amd64.deb
# Wed, 14 Jul 2021 00:04:53 GMT
ARG CB_SHA256=992fc9aef85c210cc2d782a1726f2ef56ceb322fd67c2e95500e276ff106e6ff
# Wed, 14 Jul 2021 00:04:53 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Wed, 14 Jul 2021 00:04:55 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.5.1-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.5.1 CB_SHA256=992fc9aef85c210cc2d782a1726f2ef56ceb322fd67c2e95500e276ff106e6ff CB_VERSION=6.5.1
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Wed, 14 Jul 2021 00:06:19 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.5.1-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.5.1 CB_SHA256=992fc9aef85c210cc2d782a1726f2ef56ceb322fd67c2e95500e276ff106e6ff CB_VERSION=6.5.1
RUN set -x &&     export INSTALL_DONT_START_SERVER=1 &&     wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE &&     echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - &&     apt-get update &&     apt-get install -y ./$CB_PACKAGE &&     rm -f ./$CB_PACKAGE &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Wed, 14 Jul 2021 00:06:23 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.5.1-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.5.1 CB_SHA256=992fc9aef85c210cc2d782a1726f2ef56ceb322fd67c2e95500e276ff106e6ff CB_VERSION=6.5.1
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Wed, 14 Jul 2021 00:06:23 GMT
COPY file:d6a307209223b2df102f46f07fd186e09fac7114db2c965bb54097d3b4d3b989 in /etc/service/couchbase-server/run 
# Wed, 14 Jul 2021 00:06:25 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.5.1-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.5.1 CB_SHA256=992fc9aef85c210cc2d782a1726f2ef56ceb322fd67c2e95500e276ff106e6ff CB_VERSION=6.5.1
RUN mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Wed, 14 Jul 2021 00:06:25 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Wed, 14 Jul 2021 00:06:26 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.5.1-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.5.1 CB_SHA256=992fc9aef85c210cc2d782a1726f2ef56ceb322fd67c2e95500e276ff106e6ff CB_VERSION=6.5.1
RUN ln -s dummy.sh /usr/local/bin/iptables-save &&     ln -s dummy.sh /usr/local/bin/lvdisplay &&     ln -s dummy.sh /usr/local/bin/vgdisplay &&     ln -s dummy.sh /usr/local/bin/pvdisplay
# Wed, 14 Jul 2021 00:06:28 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.5.1-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.5.1 CB_SHA256=992fc9aef85c210cc2d782a1726f2ef56ceb322fd67c2e95500e276ff106e6ff CB_VERSION=6.5.1
RUN chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl
# Wed, 14 Jul 2021 00:06:28 GMT
COPY file:d816a67f62bfba76d2812cefbe92252afa13f3852775c3e68599df7741e90cb7 in / 
# Wed, 14 Jul 2021 00:06:28 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 14 Jul 2021 00:06:28 GMT
CMD ["couchbase-server"]
# Wed, 14 Jul 2021 00:06:29 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Wed, 14 Jul 2021 00:06:29 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:e7ae86ffe2df0787131a4c49ace1b018fd38d62929b007d86bdd1f825e56a852`  
		Last Modified: Tue, 13 Jul 2021 22:31:03 GMT  
		Size: 26.7 MB (26706145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f13c80c516e182839d6e6d6f7bc46ca9d41b722a2b3187d09071f91c78769b0e`  
		Last Modified: Wed, 14 Jul 2021 00:18:37 GMT  
		Size: 7.4 MB (7373539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fec6a0ae3c3d8baa9b4f7ebc733acffb0a42e2e7a0d032ceba2a7f11936f3e3`  
		Last Modified: Wed, 14 Jul 2021 00:18:32 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab5dee3151e8e70190b53a3a3bbc9200259eb35893c26bfebc01c368a6ace06f`  
		Last Modified: Wed, 14 Jul 2021 00:22:39 GMT  
		Size: 2.0 KB (1972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaf6bdafc3bdaf035f1502520973205992dd71544a8e8bf663761e6d90796dc4`  
		Last Modified: Wed, 14 Jul 2021 00:23:34 GMT  
		Size: 467.3 MB (467306581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c3098c61a8491b51e575498cdf6045b7324bd6c78629edb107d3bc845dabba1`  
		Last Modified: Wed, 14 Jul 2021 00:22:39 GMT  
		Size: 190.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0773ef54b733514ca4ebbc3dcbb80e174ac2fc8e8a2f0321bfc839f27047ae8`  
		Last Modified: Wed, 14 Jul 2021 00:22:39 GMT  
		Size: 480.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da37c896a9bb745bff6201e8d9623dfb15618f306dd094d8e1235004c6b1c545`  
		Last Modified: Wed, 14 Jul 2021 00:22:36 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f091525ff6ca545246cc550e088b4da9e978f179f87a21f9232fee45a563e40b`  
		Last Modified: Wed, 14 Jul 2021 00:22:36 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cfc56ee30aeb0a400dc9a1cc3f6a7303bc24da14ebd14e6e786d2c6b3616cc5`  
		Last Modified: Wed, 14 Jul 2021 00:22:36 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0478a678346ea57fb828351fa802dcbfe44b0490394f261354dbb4f95ae06b58`  
		Last Modified: Wed, 14 Jul 2021 00:22:37 GMT  
		Size: 118.2 KB (118190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9d175ba0da7224c3f91c98e765a46767a7ed9297a898b36c253b52928187b73`  
		Last Modified: Wed, 14 Jul 2021 00:22:36 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchbase:6.6.0`

```console
$ docker pull couchbase@sha256:c63523e408d7fd3afc9471400ac47f738a895ca592daf543293393d5eccb1282
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `couchbase:6.6.0` - linux; amd64

```console
$ docker pull couchbase@sha256:14f998618570e30d08415634308be14529f8e934b51ef1c561a238201a75f096
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **527.3 MB (527322653 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5065e29d7a87e48e3b2538d0f535a6b03886c5f9ccb09f6dfffd6b9163573f7d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Tue, 13 Jul 2021 22:29:15 GMT
ADD file:7274ece1917848683250bbeda9eacf6eb7510481cbaa177880e3a60b4133e35b in / 
# Tue, 13 Jul 2021 22:29:15 GMT
CMD ["bash"]
# Tue, 13 Jul 2021 23:56:52 GMT
LABEL maintainer=docker@couchbase.com
# Tue, 13 Jul 2021 23:57:29 GMT
RUN set -x &&     apt-get update &&     apt-get install -yq runit wget chrpath tzdata man     lsof lshw sysstat net-tools numactl bzip2 &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Tue, 13 Jul 2021 23:57:32 GMT
RUN if [ ! -x /usr/sbin/runsvdir-start ]; then         cp -a /etc/runit/2 /usr/sbin/runsvdir-start;     fi
# Tue, 13 Jul 2021 23:57:32 GMT
ARG CB_VERSION=6.6.0
# Tue, 13 Jul 2021 23:57:32 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0
# Wed, 14 Jul 2021 00:03:11 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_6.6.0-ubuntu18.04_amd64.deb
# Wed, 14 Jul 2021 00:03:11 GMT
ARG CB_SHA256=8e7fd5434537094be2fbdfedf3ab5005f0f7d5b9d0578f59ce540b424215b728
# Wed, 14 Jul 2021 00:03:12 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Wed, 14 Jul 2021 00:03:14 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.0-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=8e7fd5434537094be2fbdfedf3ab5005f0f7d5b9d0578f59ce540b424215b728 CB_VERSION=6.6.0
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Wed, 14 Jul 2021 00:04:23 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.0-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=8e7fd5434537094be2fbdfedf3ab5005f0f7d5b9d0578f59ce540b424215b728 CB_VERSION=6.6.0
RUN set -x &&     export INSTALL_DONT_START_SERVER=1 &&     wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE &&     echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - &&     apt-get update &&     apt-get install -y ./$CB_PACKAGE &&     rm -f ./$CB_PACKAGE &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Wed, 14 Jul 2021 00:04:29 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.0-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=8e7fd5434537094be2fbdfedf3ab5005f0f7d5b9d0578f59ce540b424215b728 CB_VERSION=6.6.0
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Wed, 14 Jul 2021 00:04:29 GMT
COPY file:d6a307209223b2df102f46f07fd186e09fac7114db2c965bb54097d3b4d3b989 in /etc/service/couchbase-server/run 
# Wed, 14 Jul 2021 00:04:31 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.0-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=8e7fd5434537094be2fbdfedf3ab5005f0f7d5b9d0578f59ce540b424215b728 CB_VERSION=6.6.0
RUN mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Wed, 14 Jul 2021 00:04:32 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Wed, 14 Jul 2021 00:04:34 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.0-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=8e7fd5434537094be2fbdfedf3ab5005f0f7d5b9d0578f59ce540b424215b728 CB_VERSION=6.6.0
RUN ln -s dummy.sh /usr/local/bin/iptables-save &&     ln -s dummy.sh /usr/local/bin/lvdisplay &&     ln -s dummy.sh /usr/local/bin/vgdisplay &&     ln -s dummy.sh /usr/local/bin/pvdisplay
# Wed, 14 Jul 2021 00:04:36 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.0-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=8e7fd5434537094be2fbdfedf3ab5005f0f7d5b9d0578f59ce540b424215b728 CB_VERSION=6.6.0
RUN chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl
# Wed, 14 Jul 2021 00:04:36 GMT
COPY file:d816a67f62bfba76d2812cefbe92252afa13f3852775c3e68599df7741e90cb7 in / 
# Wed, 14 Jul 2021 00:04:36 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 14 Jul 2021 00:04:37 GMT
CMD ["couchbase-server"]
# Wed, 14 Jul 2021 00:04:37 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Wed, 14 Jul 2021 00:04:37 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:e7ae86ffe2df0787131a4c49ace1b018fd38d62929b007d86bdd1f825e56a852`  
		Last Modified: Tue, 13 Jul 2021 22:31:03 GMT  
		Size: 26.7 MB (26706145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f13c80c516e182839d6e6d6f7bc46ca9d41b722a2b3187d09071f91c78769b0e`  
		Last Modified: Wed, 14 Jul 2021 00:18:37 GMT  
		Size: 7.4 MB (7373539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fec6a0ae3c3d8baa9b4f7ebc733acffb0a42e2e7a0d032ceba2a7f11936f3e3`  
		Last Modified: Wed, 14 Jul 2021 00:18:32 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:beff1fabd9cf83626d6441f27e38595e1a37e842ba062f25b094dae598fec8e9`  
		Last Modified: Wed, 14 Jul 2021 00:21:29 GMT  
		Size: 2.0 KB (1968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91f0c28648ffc3d7438a50edd26aa3e046b56497a8eff6cc962f7fb9b34893f0`  
		Last Modified: Wed, 14 Jul 2021 00:22:23 GMT  
		Size: 493.1 MB (493120282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d71d047bc6c5881d40b2338128dfe1f70c8c2a84cc05858bcdd7f1c528be6278`  
		Last Modified: Wed, 14 Jul 2021 00:21:29 GMT  
		Size: 190.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2c02e2f983881fdc342643c2a1960010fa65d78f4b5ab41371728dac97bd9db`  
		Last Modified: Wed, 14 Jul 2021 00:21:29 GMT  
		Size: 479.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b58b74c5013e779d82b12a7bebd5a6684161c2c54aed4fc5ab1d89e36975011`  
		Last Modified: Wed, 14 Jul 2021 00:21:26 GMT  
		Size: 280.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b1f6a851d29532a08ec1b8ae8f218a6b884e6e1c0894700ea8d67d1d8521e82`  
		Last Modified: Wed, 14 Jul 2021 00:21:26 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbfec9fa5f7320af7b34ea68e7a091df7773884c8491b01ce13cd74623adf692`  
		Last Modified: Wed, 14 Jul 2021 00:21:26 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a26f4d875683ac9ae45a8f9141852ec801ec35844858650109df21a64313c1b7`  
		Last Modified: Wed, 14 Jul 2021 00:21:26 GMT  
		Size: 118.2 KB (118192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f37c9aa96adac79e5a02cdd8ab85bc2f4537d7c1ce3e9e1a922a9851f388e9c`  
		Last Modified: Wed, 14 Jul 2021 00:21:26 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchbase:6.6.1`

```console
$ docker pull couchbase@sha256:af6148a17dfdbfb30c187e7247fa5bff41f6a3dfe00b21e4fcf0a393d1e3cb3a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `couchbase:6.6.1` - linux; amd64

```console
$ docker pull couchbase@sha256:b71d901bea6d20aeaf635993d07a5763c08c01500c0f257d80dee19a1b02242b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **528.5 MB (528524928 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:17fa76aff6698eef0b73a35d09436f4cd1af6964ed3a0456b045170d3d054ecb`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Tue, 13 Jul 2021 22:29:15 GMT
ADD file:7274ece1917848683250bbeda9eacf6eb7510481cbaa177880e3a60b4133e35b in / 
# Tue, 13 Jul 2021 22:29:15 GMT
CMD ["bash"]
# Tue, 13 Jul 2021 23:56:52 GMT
LABEL maintainer=docker@couchbase.com
# Tue, 13 Jul 2021 23:57:29 GMT
RUN set -x &&     apt-get update &&     apt-get install -yq runit wget chrpath tzdata man     lsof lshw sysstat net-tools numactl bzip2 &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Tue, 13 Jul 2021 23:57:32 GMT
RUN if [ ! -x /usr/sbin/runsvdir-start ]; then         cp -a /etc/runit/2 /usr/sbin/runsvdir-start;     fi
# Wed, 14 Jul 2021 00:01:14 GMT
ARG CB_VERSION=6.6.1
# Wed, 14 Jul 2021 00:01:15 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.1
# Wed, 14 Jul 2021 00:01:15 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_6.6.1-ubuntu18.04_amd64.deb
# Wed, 14 Jul 2021 00:01:15 GMT
ARG CB_SHA256=4bd8210458905a5801e98bda0663d1214f6743465843f49ef9a52212636b5e89
# Wed, 14 Jul 2021 00:01:16 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Wed, 14 Jul 2021 00:01:17 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.1-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.1 CB_SHA256=4bd8210458905a5801e98bda0663d1214f6743465843f49ef9a52212636b5e89 CB_VERSION=6.6.1
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Wed, 14 Jul 2021 00:02:39 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.1-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.1 CB_SHA256=4bd8210458905a5801e98bda0663d1214f6743465843f49ef9a52212636b5e89 CB_VERSION=6.6.1
RUN set -x &&     export INSTALL_DONT_START_SERVER=1 &&     wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE &&     echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - &&     apt-get update &&     apt-get install -y ./$CB_PACKAGE &&     rm -f ./$CB_PACKAGE &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Wed, 14 Jul 2021 00:02:44 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.1-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.1 CB_SHA256=4bd8210458905a5801e98bda0663d1214f6743465843f49ef9a52212636b5e89 CB_VERSION=6.6.1
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Wed, 14 Jul 2021 00:02:45 GMT
COPY file:d6a307209223b2df102f46f07fd186e09fac7114db2c965bb54097d3b4d3b989 in /etc/service/couchbase-server/run 
# Wed, 14 Jul 2021 00:02:46 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.1-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.1 CB_SHA256=4bd8210458905a5801e98bda0663d1214f6743465843f49ef9a52212636b5e89 CB_VERSION=6.6.1
RUN mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Wed, 14 Jul 2021 00:02:47 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Wed, 14 Jul 2021 00:02:49 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.1-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.1 CB_SHA256=4bd8210458905a5801e98bda0663d1214f6743465843f49ef9a52212636b5e89 CB_VERSION=6.6.1
RUN ln -s dummy.sh /usr/local/bin/iptables-save &&     ln -s dummy.sh /usr/local/bin/lvdisplay &&     ln -s dummy.sh /usr/local/bin/vgdisplay &&     ln -s dummy.sh /usr/local/bin/pvdisplay
# Wed, 14 Jul 2021 00:02:51 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.1-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.1 CB_SHA256=4bd8210458905a5801e98bda0663d1214f6743465843f49ef9a52212636b5e89 CB_VERSION=6.6.1
RUN chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl
# Wed, 14 Jul 2021 00:02:51 GMT
COPY file:d816a67f62bfba76d2812cefbe92252afa13f3852775c3e68599df7741e90cb7 in / 
# Wed, 14 Jul 2021 00:02:52 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 14 Jul 2021 00:02:52 GMT
CMD ["couchbase-server"]
# Wed, 14 Jul 2021 00:02:52 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Wed, 14 Jul 2021 00:02:53 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:e7ae86ffe2df0787131a4c49ace1b018fd38d62929b007d86bdd1f825e56a852`  
		Last Modified: Tue, 13 Jul 2021 22:31:03 GMT  
		Size: 26.7 MB (26706145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f13c80c516e182839d6e6d6f7bc46ca9d41b722a2b3187d09071f91c78769b0e`  
		Last Modified: Wed, 14 Jul 2021 00:18:37 GMT  
		Size: 7.4 MB (7373539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fec6a0ae3c3d8baa9b4f7ebc733acffb0a42e2e7a0d032ceba2a7f11936f3e3`  
		Last Modified: Wed, 14 Jul 2021 00:18:32 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9286972580e33b72ccf9c3fce3fe227c9d6625574bf6787bf2d489723c906538`  
		Last Modified: Wed, 14 Jul 2021 00:20:19 GMT  
		Size: 2.0 KB (1963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1687b69a86447feeab1eb31298e4fb3b13c191ee68e30fa0a097164b9580893`  
		Last Modified: Wed, 14 Jul 2021 00:21:14 GMT  
		Size: 494.3 MB (494322565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1ba863fe24827037c66b30eddf1f16af20ea3e786b84e6e7850f1131b7ffd02`  
		Last Modified: Wed, 14 Jul 2021 00:20:19 GMT  
		Size: 190.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e747f934c61fd217d3d09b8b8b6213d8cf601b008e3c9033ec8e2ccfb56fc931`  
		Last Modified: Wed, 14 Jul 2021 00:20:19 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6342fbc05e2e7d8a699270d543c3e0da4bb5f587f8c43a6f491424bcb60e9304`  
		Last Modified: Wed, 14 Jul 2021 00:20:17 GMT  
		Size: 282.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a1f233d6e7725d9fa0bf5328e7c8b80e7efc71112be7507cb7a7bc06149f1b3`  
		Last Modified: Wed, 14 Jul 2021 00:20:17 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8081b1aafdb161c6c8f0021ee61ac6bfe1371824658432201dc2a3e59aa3a26b`  
		Last Modified: Wed, 14 Jul 2021 00:20:17 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1727ebe294a93614fb6a2674332ac66d4ac849581f75da275adb6abefb6b2746`  
		Last Modified: Wed, 14 Jul 2021 00:20:17 GMT  
		Size: 118.2 KB (118190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a64e65e5fc46d51deb08bee39f530bc2e4029b8b543da18e751fed8b428811aa`  
		Last Modified: Wed, 14 Jul 2021 00:20:17 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchbase:6.6.2`

```console
$ docker pull couchbase@sha256:f81f332a99b86514042eaf1194603d65c37404c2686d1ae3ec3855056247be5c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `couchbase:6.6.2` - linux; amd64

```console
$ docker pull couchbase@sha256:512ce0c9f998819d6e59f576cb24bc258775dfcfd52eee616427a5dec207eac3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **533.2 MB (533221032 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:00cc1f1af822aeda54b4e7859f621aaab1b8ac5a0eb0a97e0e89fdbdd7a005b1`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Tue, 13 Jul 2021 22:29:34 GMT
ADD file:5c3d9d2597e01d1cee8513ff0e1344e7791e6f582be2cbd1d5777dd204780f1c in / 
# Tue, 13 Jul 2021 22:29:34 GMT
CMD ["bash"]
# Tue, 13 Jul 2021 23:50:49 GMT
LABEL maintainer=docker@couchbase.com
# Tue, 13 Jul 2021 23:55:02 GMT
RUN set -x &&     apt-get update &&     apt-get install -yq runit wget chrpath tzdata     lsof lshw sysstat net-tools numactl bzip2 &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Tue, 13 Jul 2021 23:55:04 GMT
RUN if [ ! -x /usr/sbin/runsvdir-start ]; then         cp -a /etc/runit/2 /usr/sbin/runsvdir-start;     fi
# Tue, 13 Jul 2021 23:55:05 GMT
ARG CB_VERSION=6.6.2
# Tue, 13 Jul 2021 23:55:05 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.2
# Tue, 13 Jul 2021 23:55:06 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_6.6.2-ubuntu20.04_amd64.deb
# Tue, 13 Jul 2021 23:55:06 GMT
ARG CB_SHA256=41c033e6c1e98b0844a5cb5768e3769e7012d8374a6bd235c86e10db33b17afc
# Tue, 13 Jul 2021 23:55:06 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Tue, 13 Jul 2021 23:55:08 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.2-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.2 CB_SHA256=41c033e6c1e98b0844a5cb5768e3769e7012d8374a6bd235c86e10db33b17afc CB_VERSION=6.6.2
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Tue, 13 Jul 2021 23:56:27 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.2-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.2 CB_SHA256=41c033e6c1e98b0844a5cb5768e3769e7012d8374a6bd235c86e10db33b17afc CB_VERSION=6.6.2
RUN set -x &&     export INSTALL_DONT_START_SERVER=1 &&     wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE &&     echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - &&     apt-get update &&     apt-get install -y ./$CB_PACKAGE &&     rm -f ./$CB_PACKAGE &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Tue, 13 Jul 2021 23:56:32 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.2-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.2 CB_SHA256=41c033e6c1e98b0844a5cb5768e3769e7012d8374a6bd235c86e10db33b17afc CB_VERSION=6.6.2
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Tue, 13 Jul 2021 23:56:32 GMT
COPY file:d6a307209223b2df102f46f07fd186e09fac7114db2c965bb54097d3b4d3b989 in /etc/service/couchbase-server/run 
# Tue, 13 Jul 2021 23:56:34 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.2-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.2 CB_SHA256=41c033e6c1e98b0844a5cb5768e3769e7012d8374a6bd235c86e10db33b17afc CB_VERSION=6.6.2
RUN mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Tue, 13 Jul 2021 23:56:34 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Tue, 13 Jul 2021 23:56:36 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.2-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.2 CB_SHA256=41c033e6c1e98b0844a5cb5768e3769e7012d8374a6bd235c86e10db33b17afc CB_VERSION=6.6.2
RUN ln -s dummy.sh /usr/local/bin/iptables-save &&     ln -s dummy.sh /usr/local/bin/lvdisplay &&     ln -s dummy.sh /usr/local/bin/vgdisplay &&     ln -s dummy.sh /usr/local/bin/pvdisplay
# Tue, 13 Jul 2021 23:56:37 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.2-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.2 CB_SHA256=41c033e6c1e98b0844a5cb5768e3769e7012d8374a6bd235c86e10db33b17afc CB_VERSION=6.6.2
RUN chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl
# Tue, 13 Jul 2021 23:56:37 GMT
COPY file:d816a67f62bfba76d2812cefbe92252afa13f3852775c3e68599df7741e90cb7 in / 
# Tue, 13 Jul 2021 23:56:37 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 13 Jul 2021 23:56:38 GMT
CMD ["couchbase-server"]
# Tue, 13 Jul 2021 23:56:38 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Tue, 13 Jul 2021 23:56:38 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:a31c7b29f4ad2bd946738970f040825704a523ded1b9d6f9c7c7cafc6ab731df`  
		Last Modified: Tue, 13 Jul 2021 22:31:20 GMT  
		Size: 28.6 MB (28565863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f926d574d0b4b28f1f76deaa9aff956ebd84fca4c28ae00cb2342e321657edf3`  
		Last Modified: Wed, 14 Jul 2021 00:17:16 GMT  
		Size: 6.3 MB (6272606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ad3c9266985cc6da988565a76f19e617642668ced44547bb0e3b11af0301a00`  
		Last Modified: Wed, 14 Jul 2021 00:17:13 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23d163e5c68bca024eec49616679790ec8960fcde31526d8e29b5b1c38a9e872`  
		Last Modified: Wed, 14 Jul 2021 00:17:12 GMT  
		Size: 1.8 KB (1830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef2f5d79c085803411789e047e9ac102f5b17b68e9cffdcf72c199cabae6f6c0`  
		Last Modified: Wed, 14 Jul 2021 00:18:07 GMT  
		Size: 498.3 MB (498252316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c1d5eca3d063ae7effcc02e063c12fba349a3397808320570881e1cd400c468`  
		Last Modified: Wed, 14 Jul 2021 00:17:11 GMT  
		Size: 191.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63d346d7d3d4c52f9398df214716d61690c11261de8d80fdf0667a891d03f975`  
		Last Modified: Wed, 14 Jul 2021 00:17:11 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d45857737224785a1eab0c64e68eca963845fc8c29ba24f0f31cca91f9f73a4c`  
		Last Modified: Wed, 14 Jul 2021 00:17:09 GMT  
		Size: 281.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cce5e9dc1794cbdc1c5c738f15081bcfd141e67f3bea239ac3c2550551d5e76`  
		Last Modified: Wed, 14 Jul 2021 00:17:10 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:823f3f5bd72eb157355adc6d50c5df0e37548878cbad7b1ce94a902b039d5c61`  
		Last Modified: Wed, 14 Jul 2021 00:17:09 GMT  
		Size: 216.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ded2b29872fe46b0fdbeae64bbbbfdda02d84267a7b46538e6b749ce296fd3ce`  
		Last Modified: Wed, 14 Jul 2021 00:17:09 GMT  
		Size: 125.9 KB (125895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79733ad7ecdd3e0dc809f52676d3c3468febbb8306ca93d20ff073847c2f50ea`  
		Last Modified: Wed, 14 Jul 2021 00:17:09 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchbase:7.0.0-beta`

```console
$ docker pull couchbase@sha256:d1688941d858881861c60fb674f37ec439f098035f00d682710ee0d06ef18799
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `couchbase:7.0.0-beta` - linux; amd64

```console
$ docker pull couchbase@sha256:7fc24a15658a601982c5e1832db2189ea949aabbe7b86e2e4b37c2510583a047
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **628.1 MB (628096335 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b754d7f1774a0d94e1402b2a26d3cdf7cc241a468e6b53d7d6c3a2191cf094f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Tue, 13 Jul 2021 22:29:34 GMT
ADD file:5c3d9d2597e01d1cee8513ff0e1344e7791e6f582be2cbd1d5777dd204780f1c in / 
# Tue, 13 Jul 2021 22:29:34 GMT
CMD ["bash"]
# Tue, 13 Jul 2021 23:50:49 GMT
LABEL maintainer=docker@couchbase.com
# Tue, 13 Jul 2021 23:51:15 GMT
RUN set -x &&     apt-get update &&     apt-get install -yq runit wget chrpath tzdata man     lsof lshw sysstat net-tools numactl bzip2 &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Tue, 13 Jul 2021 23:51:16 GMT
RUN if [ ! -x /usr/sbin/runsvdir-start ]; then         cp -a /etc/runit/2 /usr/sbin/runsvdir-start;     fi
# Tue, 13 Jul 2021 23:51:16 GMT
ARG CB_VERSION=7.0.0-beta
# Tue, 13 Jul 2021 23:51:17 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.0-beta
# Tue, 13 Jul 2021 23:51:17 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_7.0.0-beta-ubuntu20.04_amd64.deb
# Tue, 13 Jul 2021 23:51:17 GMT
ARG CB_SHA256=e24be4f765eafbfbfdd5f7eddb780006084e3bd01cbcb3d3880dd9be48b955f6
# Tue, 13 Jul 2021 23:51:17 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Tue, 13 Jul 2021 23:51:18 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.0-beta-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.0-beta CB_SHA256=e24be4f765eafbfbfdd5f7eddb780006084e3bd01cbcb3d3880dd9be48b955f6 CB_VERSION=7.0.0-beta
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Tue, 13 Jul 2021 23:52:43 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.0-beta-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.0-beta CB_SHA256=e24be4f765eafbfbfdd5f7eddb780006084e3bd01cbcb3d3880dd9be48b955f6 CB_VERSION=7.0.0-beta
RUN set -x &&     export INSTALL_DONT_START_SERVER=1 &&     wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE &&     echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - &&     apt-get update &&     apt-get install -y ./$CB_PACKAGE &&     rm -f ./$CB_PACKAGE &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Tue, 13 Jul 2021 23:52:50 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.0-beta-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.0-beta CB_SHA256=e24be4f765eafbfbfdd5f7eddb780006084e3bd01cbcb3d3880dd9be48b955f6 CB_VERSION=7.0.0-beta
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Tue, 13 Jul 2021 23:52:50 GMT
COPY file:d6a307209223b2df102f46f07fd186e09fac7114db2c965bb54097d3b4d3b989 in /etc/service/couchbase-server/run 
# Tue, 13 Jul 2021 23:52:52 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.0-beta-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.0-beta CB_SHA256=e24be4f765eafbfbfdd5f7eddb780006084e3bd01cbcb3d3880dd9be48b955f6 CB_VERSION=7.0.0-beta
RUN mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Tue, 13 Jul 2021 23:52:53 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Tue, 13 Jul 2021 23:52:55 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.0-beta-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.0-beta CB_SHA256=e24be4f765eafbfbfdd5f7eddb780006084e3bd01cbcb3d3880dd9be48b955f6 CB_VERSION=7.0.0-beta
RUN ln -s dummy.sh /usr/local/bin/iptables-save &&     ln -s dummy.sh /usr/local/bin/lvdisplay &&     ln -s dummy.sh /usr/local/bin/vgdisplay &&     ln -s dummy.sh /usr/local/bin/pvdisplay
# Tue, 13 Jul 2021 23:52:57 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.0-beta-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.0-beta CB_SHA256=e24be4f765eafbfbfdd5f7eddb780006084e3bd01cbcb3d3880dd9be48b955f6 CB_VERSION=7.0.0-beta
RUN chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl
# Tue, 13 Jul 2021 23:52:57 GMT
COPY file:d816a67f62bfba76d2812cefbe92252afa13f3852775c3e68599df7741e90cb7 in / 
# Tue, 13 Jul 2021 23:52:58 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 13 Jul 2021 23:52:58 GMT
CMD ["couchbase-server"]
# Tue, 13 Jul 2021 23:52:58 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Tue, 13 Jul 2021 23:52:59 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:a31c7b29f4ad2bd946738970f040825704a523ded1b9d6f9c7c7cafc6ab731df`  
		Last Modified: Tue, 13 Jul 2021 22:31:20 GMT  
		Size: 28.6 MB (28565863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27d820bb660a9b14c611213779ee0deee8781268242fd7d51bd43a6e638f6722`  
		Last Modified: Wed, 14 Jul 2021 00:14:56 GMT  
		Size: 8.3 MB (8286840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db40d5a53531bbb33b0d3feb0be6f6fd03a142fba87ac62d5487adf1928a6673`  
		Last Modified: Wed, 14 Jul 2021 00:14:50 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:875bb808e008cdde9ba4f2b7d35760e77f6a6a2e2db82c5e41e877fedd410d7d`  
		Last Modified: Wed, 14 Jul 2021 00:14:51 GMT  
		Size: 1.8 KB (1830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:855824ba8946788de53fb20491f40faa224f2e5074bf3e8c3008c33fb81ff555`  
		Last Modified: Wed, 14 Jul 2021 00:15:57 GMT  
		Size: 591.1 MB (591113393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfc2a6dcc68d13067288c0300be7915f87fa22d599b8fb8a67bc3f2e194bf63e`  
		Last Modified: Wed, 14 Jul 2021 00:14:50 GMT  
		Size: 191.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c0d1e8645eda88311f73a402d5fc3541f22644726fc24084ba70ee986c42cbe`  
		Last Modified: Wed, 14 Jul 2021 00:14:50 GMT  
		Size: 472.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d9804d533cfe6215e476fd14d430e059f3998b5c7197b74b47dcb9da80b950f`  
		Last Modified: Wed, 14 Jul 2021 00:14:48 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10603d7e2729cb2b4acf00f32356c7545eac6748343669324c164bfc684e85c6`  
		Last Modified: Wed, 14 Jul 2021 00:14:48 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f959ad6bef002fb82a015a17c8f4e7a885ccc2bc9868147291a239165c43d39`  
		Last Modified: Wed, 14 Jul 2021 00:14:48 GMT  
		Size: 217.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21d42cd2ad5a7005696a4d7e2c1f84eafc57294b5cd3d4ee7a86cb41d4ed09fb`  
		Last Modified: Wed, 14 Jul 2021 00:14:48 GMT  
		Size: 125.9 KB (125893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0037a926b052a91e2453be04f4ae22cdfc4563cbc7536cb2d2bf0273afb8681`  
		Last Modified: Wed, 14 Jul 2021 00:14:48 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchbase:community`

```console
$ docker pull couchbase@sha256:a3b49c114e2c940ee412c4039120168389e52f4e351c81d2950f2e38f32fe7bf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `couchbase:community` - linux; amd64

```console
$ docker pull couchbase@sha256:cbc97df6300e0b0683dcb96a8439bd1c1f0d1016f2446e528e96f1486e10258c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **354.2 MB (354220927 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9188d75c56d46842d6a319020eb51f8383bc376b9b6d53eb8e120f9025e06f01`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Tue, 13 Jul 2021 22:29:15 GMT
ADD file:7274ece1917848683250bbeda9eacf6eb7510481cbaa177880e3a60b4133e35b in / 
# Tue, 13 Jul 2021 22:29:15 GMT
CMD ["bash"]
# Tue, 13 Jul 2021 23:56:52 GMT
LABEL maintainer=docker@couchbase.com
# Tue, 13 Jul 2021 23:57:29 GMT
RUN set -x &&     apt-get update &&     apt-get install -yq runit wget chrpath tzdata man     lsof lshw sysstat net-tools numactl bzip2 &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Tue, 13 Jul 2021 23:57:32 GMT
RUN if [ ! -x /usr/sbin/runsvdir-start ]; then         cp -a /etc/runit/2 /usr/sbin/runsvdir-start;     fi
# Tue, 13 Jul 2021 23:57:32 GMT
ARG CB_VERSION=6.6.0
# Tue, 13 Jul 2021 23:57:32 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0
# Tue, 13 Jul 2021 23:57:32 GMT
ARG CB_PACKAGE=couchbase-server-community_6.6.0-ubuntu18.04_amd64.deb
# Tue, 13 Jul 2021 23:57:33 GMT
ARG CB_SHA256=9b196cd7be81d7d6b179838e9d30164fdb7a1f27e96678e61e24e9fe5c93f559
# Tue, 13 Jul 2021 23:57:33 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Tue, 13 Jul 2021 23:57:35 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_6.6.0-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=9b196cd7be81d7d6b179838e9d30164fdb7a1f27e96678e61e24e9fe5c93f559 CB_VERSION=6.6.0
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Tue, 13 Jul 2021 23:58:37 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_6.6.0-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=9b196cd7be81d7d6b179838e9d30164fdb7a1f27e96678e61e24e9fe5c93f559 CB_VERSION=6.6.0
RUN set -x &&     export INSTALL_DONT_START_SERVER=1 &&     wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE &&     echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - &&     apt-get update &&     apt-get install -y ./$CB_PACKAGE &&     rm -f ./$CB_PACKAGE &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Tue, 13 Jul 2021 23:58:42 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_6.6.0-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=9b196cd7be81d7d6b179838e9d30164fdb7a1f27e96678e61e24e9fe5c93f559 CB_VERSION=6.6.0
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Tue, 13 Jul 2021 23:58:42 GMT
COPY file:d6a307209223b2df102f46f07fd186e09fac7114db2c965bb54097d3b4d3b989 in /etc/service/couchbase-server/run 
# Tue, 13 Jul 2021 23:58:44 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_6.6.0-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=9b196cd7be81d7d6b179838e9d30164fdb7a1f27e96678e61e24e9fe5c93f559 CB_VERSION=6.6.0
RUN mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Tue, 13 Jul 2021 23:58:44 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Tue, 13 Jul 2021 23:58:46 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_6.6.0-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=9b196cd7be81d7d6b179838e9d30164fdb7a1f27e96678e61e24e9fe5c93f559 CB_VERSION=6.6.0
RUN ln -s dummy.sh /usr/local/bin/iptables-save &&     ln -s dummy.sh /usr/local/bin/lvdisplay &&     ln -s dummy.sh /usr/local/bin/vgdisplay &&     ln -s dummy.sh /usr/local/bin/pvdisplay
# Tue, 13 Jul 2021 23:58:48 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_6.6.0-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=9b196cd7be81d7d6b179838e9d30164fdb7a1f27e96678e61e24e9fe5c93f559 CB_VERSION=6.6.0
RUN chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl
# Tue, 13 Jul 2021 23:58:48 GMT
COPY file:d816a67f62bfba76d2812cefbe92252afa13f3852775c3e68599df7741e90cb7 in / 
# Tue, 13 Jul 2021 23:58:48 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 13 Jul 2021 23:58:48 GMT
CMD ["couchbase-server"]
# Tue, 13 Jul 2021 23:58:49 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Tue, 13 Jul 2021 23:58:49 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:e7ae86ffe2df0787131a4c49ace1b018fd38d62929b007d86bdd1f825e56a852`  
		Last Modified: Tue, 13 Jul 2021 22:31:03 GMT  
		Size: 26.7 MB (26706145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f13c80c516e182839d6e6d6f7bc46ca9d41b722a2b3187d09071f91c78769b0e`  
		Last Modified: Wed, 14 Jul 2021 00:18:37 GMT  
		Size: 7.4 MB (7373539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fec6a0ae3c3d8baa9b4f7ebc733acffb0a42e2e7a0d032ceba2a7f11936f3e3`  
		Last Modified: Wed, 14 Jul 2021 00:18:32 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90b044bef35f71fc5ad909b9c120498dfcc56203b05466c42a9652aa7cfe76b7`  
		Last Modified: Wed, 14 Jul 2021 00:18:32 GMT  
		Size: 2.0 KB (1962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3533fd10906e91d51ac325e4b84d11198417748a608bfff173ffa3810057301a`  
		Last Modified: Wed, 14 Jul 2021 00:19:11 GMT  
		Size: 320.0 MB (320018573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60a370420cad28d201c6e76340ac6116eccac08d70000442c7bd76bb088f0b16`  
		Last Modified: Wed, 14 Jul 2021 00:18:32 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc17521d27f10560119aa2b999b4a33cfccad23b93b8bc8e10610d6edb89b0a2`  
		Last Modified: Wed, 14 Jul 2021 00:18:32 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5e4ec33c9da3da4066c087d543b96825b4684f158e879438b319baccf9fb81a`  
		Last Modified: Wed, 14 Jul 2021 00:18:30 GMT  
		Size: 279.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf8f3e5cbaba139c05a8c593cecf2b8248f37f5d88cca0f6ecf67300f34d00a0`  
		Last Modified: Wed, 14 Jul 2021 00:18:29 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e616737063650334ab279a00fe79613e34cd8cdac339085e854333779bd743fc`  
		Last Modified: Wed, 14 Jul 2021 00:18:30 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ddecd6c0f56654c2d2dc150ffce1983137207b7b7170fd1c2706d9619b2fcb6`  
		Last Modified: Wed, 14 Jul 2021 00:18:30 GMT  
		Size: 118.2 KB (118187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:587dcae06a9efe5aaccad9c7f80d654af05dad4f338ddf848becd288ca3e6363`  
		Last Modified: Wed, 14 Jul 2021 00:18:30 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchbase:community-6.5.0`

```console
$ docker pull couchbase@sha256:780920ed1462df52fe74af43df7c69ff91f20354802c2c135643254b7e6fe3f9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `couchbase:community-6.5.0` - linux; amd64

```console
$ docker pull couchbase@sha256:1e8d3f9934fbcfcb8f07957fcff53c263b1e1a4662b8e7efef29f44c6981fe4f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **351.6 MB (351613024 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:17a0a1ac8b418424cfc540f20dc8d03d0da7641cf3e67badf4413dcf852bdc77`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Tue, 13 Jul 2021 22:29:15 GMT
ADD file:7274ece1917848683250bbeda9eacf6eb7510481cbaa177880e3a60b4133e35b in / 
# Tue, 13 Jul 2021 22:29:15 GMT
CMD ["bash"]
# Tue, 13 Jul 2021 23:56:52 GMT
LABEL maintainer=docker@couchbase.com
# Tue, 13 Jul 2021 23:57:29 GMT
RUN set -x &&     apt-get update &&     apt-get install -yq runit wget chrpath tzdata man     lsof lshw sysstat net-tools numactl bzip2 &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Tue, 13 Jul 2021 23:57:32 GMT
RUN if [ ! -x /usr/sbin/runsvdir-start ]; then         cp -a /etc/runit/2 /usr/sbin/runsvdir-start;     fi
# Wed, 14 Jul 2021 00:04:52 GMT
ARG CB_VERSION=6.5.1
# Wed, 14 Jul 2021 00:04:52 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/6.5.1
# Wed, 14 Jul 2021 00:13:13 GMT
ARG CB_PACKAGE=couchbase-server-community_6.5.1-ubuntu18.04_amd64.deb
# Wed, 14 Jul 2021 00:13:13 GMT
ARG CB_SHA256=c4951cdab01759020444e4648023721ae3a333257591252475d34d5fc6ac8857
# Wed, 14 Jul 2021 00:13:14 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Wed, 14 Jul 2021 00:13:15 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_6.5.1-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.5.1 CB_SHA256=c4951cdab01759020444e4648023721ae3a333257591252475d34d5fc6ac8857 CB_VERSION=6.5.1
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Wed, 14 Jul 2021 00:13:59 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_6.5.1-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.5.1 CB_SHA256=c4951cdab01759020444e4648023721ae3a333257591252475d34d5fc6ac8857 CB_VERSION=6.5.1
RUN set -x &&     export INSTALL_DONT_START_SERVER=1 &&     wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE &&     echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - &&     apt-get update &&     apt-get install -y ./$CB_PACKAGE &&     rm -f ./$CB_PACKAGE &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Wed, 14 Jul 2021 00:14:02 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_6.5.1-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.5.1 CB_SHA256=c4951cdab01759020444e4648023721ae3a333257591252475d34d5fc6ac8857 CB_VERSION=6.5.1
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Wed, 14 Jul 2021 00:14:02 GMT
COPY file:d6a307209223b2df102f46f07fd186e09fac7114db2c965bb54097d3b4d3b989 in /etc/service/couchbase-server/run 
# Wed, 14 Jul 2021 00:14:03 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_6.5.1-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.5.1 CB_SHA256=c4951cdab01759020444e4648023721ae3a333257591252475d34d5fc6ac8857 CB_VERSION=6.5.1
RUN mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Wed, 14 Jul 2021 00:14:04 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Wed, 14 Jul 2021 00:14:05 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_6.5.1-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.5.1 CB_SHA256=c4951cdab01759020444e4648023721ae3a333257591252475d34d5fc6ac8857 CB_VERSION=6.5.1
RUN ln -s dummy.sh /usr/local/bin/iptables-save &&     ln -s dummy.sh /usr/local/bin/lvdisplay &&     ln -s dummy.sh /usr/local/bin/vgdisplay &&     ln -s dummy.sh /usr/local/bin/pvdisplay
# Wed, 14 Jul 2021 00:14:06 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_6.5.1-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.5.1 CB_SHA256=c4951cdab01759020444e4648023721ae3a333257591252475d34d5fc6ac8857 CB_VERSION=6.5.1
RUN chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl
# Wed, 14 Jul 2021 00:14:06 GMT
COPY file:d816a67f62bfba76d2812cefbe92252afa13f3852775c3e68599df7741e90cb7 in / 
# Wed, 14 Jul 2021 00:14:06 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 14 Jul 2021 00:14:06 GMT
CMD ["couchbase-server"]
# Wed, 14 Jul 2021 00:14:07 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Wed, 14 Jul 2021 00:14:07 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:e7ae86ffe2df0787131a4c49ace1b018fd38d62929b007d86bdd1f825e56a852`  
		Last Modified: Tue, 13 Jul 2021 22:31:03 GMT  
		Size: 26.7 MB (26706145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f13c80c516e182839d6e6d6f7bc46ca9d41b722a2b3187d09071f91c78769b0e`  
		Last Modified: Wed, 14 Jul 2021 00:18:37 GMT  
		Size: 7.4 MB (7373539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fec6a0ae3c3d8baa9b4f7ebc733acffb0a42e2e7a0d032ceba2a7f11936f3e3`  
		Last Modified: Wed, 14 Jul 2021 00:18:32 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5849cc4e97566fcca9e851b95d1b640d09c275a8f0de5ce9802b848505acc555`  
		Last Modified: Wed, 14 Jul 2021 00:28:44 GMT  
		Size: 2.0 KB (1968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b8c2626047f93096c08a5f89e8c06dc4769acba0b713530650f3b4046b155f2`  
		Last Modified: Wed, 14 Jul 2021 00:29:23 GMT  
		Size: 317.4 MB (317410654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1df0798bfad73262ab0c435b407b0a9f7541567a893fc51283ec6e625b495705`  
		Last Modified: Wed, 14 Jul 2021 00:28:44 GMT  
		Size: 190.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfd0e5737fd92c009d64dfdfc591c68587f699d1d8519d38ddea7c78bc3d3019`  
		Last Modified: Wed, 14 Jul 2021 00:28:44 GMT  
		Size: 479.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ccd6c507f746b7c9ddde98c68b2ecfa57c13b52bf19eee5748112cec6548b15`  
		Last Modified: Wed, 14 Jul 2021 00:28:42 GMT  
		Size: 281.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:250fd5006e469efcb2e420ed91b7797fcb761103a67f5ce7149ddc8cbbed53ae`  
		Last Modified: Wed, 14 Jul 2021 00:28:42 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5604e56d06aa7943574e9ad1a59bebe3db535a58b6ed03769b1f8e8522d2b5bd`  
		Last Modified: Wed, 14 Jul 2021 00:28:42 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:328539dacd95cce1cf6b6a90b051555f82bfa116940cbc06c1a90d26c7e8b027`  
		Last Modified: Wed, 14 Jul 2021 00:28:42 GMT  
		Size: 118.2 KB (118189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eba78f163397b863b311b9bb613a0366738840b73052c2106aae53624390da41`  
		Last Modified: Wed, 14 Jul 2021 00:28:41 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchbase:community-6.5.1`

```console
$ docker pull couchbase@sha256:780920ed1462df52fe74af43df7c69ff91f20354802c2c135643254b7e6fe3f9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `couchbase:community-6.5.1` - linux; amd64

```console
$ docker pull couchbase@sha256:1e8d3f9934fbcfcb8f07957fcff53c263b1e1a4662b8e7efef29f44c6981fe4f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **351.6 MB (351613024 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:17a0a1ac8b418424cfc540f20dc8d03d0da7641cf3e67badf4413dcf852bdc77`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Tue, 13 Jul 2021 22:29:15 GMT
ADD file:7274ece1917848683250bbeda9eacf6eb7510481cbaa177880e3a60b4133e35b in / 
# Tue, 13 Jul 2021 22:29:15 GMT
CMD ["bash"]
# Tue, 13 Jul 2021 23:56:52 GMT
LABEL maintainer=docker@couchbase.com
# Tue, 13 Jul 2021 23:57:29 GMT
RUN set -x &&     apt-get update &&     apt-get install -yq runit wget chrpath tzdata man     lsof lshw sysstat net-tools numactl bzip2 &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Tue, 13 Jul 2021 23:57:32 GMT
RUN if [ ! -x /usr/sbin/runsvdir-start ]; then         cp -a /etc/runit/2 /usr/sbin/runsvdir-start;     fi
# Wed, 14 Jul 2021 00:04:52 GMT
ARG CB_VERSION=6.5.1
# Wed, 14 Jul 2021 00:04:52 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/6.5.1
# Wed, 14 Jul 2021 00:13:13 GMT
ARG CB_PACKAGE=couchbase-server-community_6.5.1-ubuntu18.04_amd64.deb
# Wed, 14 Jul 2021 00:13:13 GMT
ARG CB_SHA256=c4951cdab01759020444e4648023721ae3a333257591252475d34d5fc6ac8857
# Wed, 14 Jul 2021 00:13:14 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Wed, 14 Jul 2021 00:13:15 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_6.5.1-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.5.1 CB_SHA256=c4951cdab01759020444e4648023721ae3a333257591252475d34d5fc6ac8857 CB_VERSION=6.5.1
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Wed, 14 Jul 2021 00:13:59 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_6.5.1-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.5.1 CB_SHA256=c4951cdab01759020444e4648023721ae3a333257591252475d34d5fc6ac8857 CB_VERSION=6.5.1
RUN set -x &&     export INSTALL_DONT_START_SERVER=1 &&     wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE &&     echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - &&     apt-get update &&     apt-get install -y ./$CB_PACKAGE &&     rm -f ./$CB_PACKAGE &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Wed, 14 Jul 2021 00:14:02 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_6.5.1-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.5.1 CB_SHA256=c4951cdab01759020444e4648023721ae3a333257591252475d34d5fc6ac8857 CB_VERSION=6.5.1
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Wed, 14 Jul 2021 00:14:02 GMT
COPY file:d6a307209223b2df102f46f07fd186e09fac7114db2c965bb54097d3b4d3b989 in /etc/service/couchbase-server/run 
# Wed, 14 Jul 2021 00:14:03 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_6.5.1-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.5.1 CB_SHA256=c4951cdab01759020444e4648023721ae3a333257591252475d34d5fc6ac8857 CB_VERSION=6.5.1
RUN mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Wed, 14 Jul 2021 00:14:04 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Wed, 14 Jul 2021 00:14:05 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_6.5.1-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.5.1 CB_SHA256=c4951cdab01759020444e4648023721ae3a333257591252475d34d5fc6ac8857 CB_VERSION=6.5.1
RUN ln -s dummy.sh /usr/local/bin/iptables-save &&     ln -s dummy.sh /usr/local/bin/lvdisplay &&     ln -s dummy.sh /usr/local/bin/vgdisplay &&     ln -s dummy.sh /usr/local/bin/pvdisplay
# Wed, 14 Jul 2021 00:14:06 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_6.5.1-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.5.1 CB_SHA256=c4951cdab01759020444e4648023721ae3a333257591252475d34d5fc6ac8857 CB_VERSION=6.5.1
RUN chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl
# Wed, 14 Jul 2021 00:14:06 GMT
COPY file:d816a67f62bfba76d2812cefbe92252afa13f3852775c3e68599df7741e90cb7 in / 
# Wed, 14 Jul 2021 00:14:06 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 14 Jul 2021 00:14:06 GMT
CMD ["couchbase-server"]
# Wed, 14 Jul 2021 00:14:07 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Wed, 14 Jul 2021 00:14:07 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:e7ae86ffe2df0787131a4c49ace1b018fd38d62929b007d86bdd1f825e56a852`  
		Last Modified: Tue, 13 Jul 2021 22:31:03 GMT  
		Size: 26.7 MB (26706145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f13c80c516e182839d6e6d6f7bc46ca9d41b722a2b3187d09071f91c78769b0e`  
		Last Modified: Wed, 14 Jul 2021 00:18:37 GMT  
		Size: 7.4 MB (7373539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fec6a0ae3c3d8baa9b4f7ebc733acffb0a42e2e7a0d032ceba2a7f11936f3e3`  
		Last Modified: Wed, 14 Jul 2021 00:18:32 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5849cc4e97566fcca9e851b95d1b640d09c275a8f0de5ce9802b848505acc555`  
		Last Modified: Wed, 14 Jul 2021 00:28:44 GMT  
		Size: 2.0 KB (1968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b8c2626047f93096c08a5f89e8c06dc4769acba0b713530650f3b4046b155f2`  
		Last Modified: Wed, 14 Jul 2021 00:29:23 GMT  
		Size: 317.4 MB (317410654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1df0798bfad73262ab0c435b407b0a9f7541567a893fc51283ec6e625b495705`  
		Last Modified: Wed, 14 Jul 2021 00:28:44 GMT  
		Size: 190.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfd0e5737fd92c009d64dfdfc591c68587f699d1d8519d38ddea7c78bc3d3019`  
		Last Modified: Wed, 14 Jul 2021 00:28:44 GMT  
		Size: 479.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ccd6c507f746b7c9ddde98c68b2ecfa57c13b52bf19eee5748112cec6548b15`  
		Last Modified: Wed, 14 Jul 2021 00:28:42 GMT  
		Size: 281.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:250fd5006e469efcb2e420ed91b7797fcb761103a67f5ce7149ddc8cbbed53ae`  
		Last Modified: Wed, 14 Jul 2021 00:28:42 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5604e56d06aa7943574e9ad1a59bebe3db535a58b6ed03769b1f8e8522d2b5bd`  
		Last Modified: Wed, 14 Jul 2021 00:28:42 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:328539dacd95cce1cf6b6a90b051555f82bfa116940cbc06c1a90d26c7e8b027`  
		Last Modified: Wed, 14 Jul 2021 00:28:42 GMT  
		Size: 118.2 KB (118189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eba78f163397b863b311b9bb613a0366738840b73052c2106aae53624390da41`  
		Last Modified: Wed, 14 Jul 2021 00:28:41 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchbase:community-6.6.0`

```console
$ docker pull couchbase@sha256:a3b49c114e2c940ee412c4039120168389e52f4e351c81d2950f2e38f32fe7bf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `couchbase:community-6.6.0` - linux; amd64

```console
$ docker pull couchbase@sha256:cbc97df6300e0b0683dcb96a8439bd1c1f0d1016f2446e528e96f1486e10258c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **354.2 MB (354220927 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9188d75c56d46842d6a319020eb51f8383bc376b9b6d53eb8e120f9025e06f01`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Tue, 13 Jul 2021 22:29:15 GMT
ADD file:7274ece1917848683250bbeda9eacf6eb7510481cbaa177880e3a60b4133e35b in / 
# Tue, 13 Jul 2021 22:29:15 GMT
CMD ["bash"]
# Tue, 13 Jul 2021 23:56:52 GMT
LABEL maintainer=docker@couchbase.com
# Tue, 13 Jul 2021 23:57:29 GMT
RUN set -x &&     apt-get update &&     apt-get install -yq runit wget chrpath tzdata man     lsof lshw sysstat net-tools numactl bzip2 &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Tue, 13 Jul 2021 23:57:32 GMT
RUN if [ ! -x /usr/sbin/runsvdir-start ]; then         cp -a /etc/runit/2 /usr/sbin/runsvdir-start;     fi
# Tue, 13 Jul 2021 23:57:32 GMT
ARG CB_VERSION=6.6.0
# Tue, 13 Jul 2021 23:57:32 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0
# Tue, 13 Jul 2021 23:57:32 GMT
ARG CB_PACKAGE=couchbase-server-community_6.6.0-ubuntu18.04_amd64.deb
# Tue, 13 Jul 2021 23:57:33 GMT
ARG CB_SHA256=9b196cd7be81d7d6b179838e9d30164fdb7a1f27e96678e61e24e9fe5c93f559
# Tue, 13 Jul 2021 23:57:33 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Tue, 13 Jul 2021 23:57:35 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_6.6.0-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=9b196cd7be81d7d6b179838e9d30164fdb7a1f27e96678e61e24e9fe5c93f559 CB_VERSION=6.6.0
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Tue, 13 Jul 2021 23:58:37 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_6.6.0-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=9b196cd7be81d7d6b179838e9d30164fdb7a1f27e96678e61e24e9fe5c93f559 CB_VERSION=6.6.0
RUN set -x &&     export INSTALL_DONT_START_SERVER=1 &&     wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE &&     echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - &&     apt-get update &&     apt-get install -y ./$CB_PACKAGE &&     rm -f ./$CB_PACKAGE &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Tue, 13 Jul 2021 23:58:42 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_6.6.0-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=9b196cd7be81d7d6b179838e9d30164fdb7a1f27e96678e61e24e9fe5c93f559 CB_VERSION=6.6.0
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Tue, 13 Jul 2021 23:58:42 GMT
COPY file:d6a307209223b2df102f46f07fd186e09fac7114db2c965bb54097d3b4d3b989 in /etc/service/couchbase-server/run 
# Tue, 13 Jul 2021 23:58:44 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_6.6.0-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=9b196cd7be81d7d6b179838e9d30164fdb7a1f27e96678e61e24e9fe5c93f559 CB_VERSION=6.6.0
RUN mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Tue, 13 Jul 2021 23:58:44 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Tue, 13 Jul 2021 23:58:46 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_6.6.0-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=9b196cd7be81d7d6b179838e9d30164fdb7a1f27e96678e61e24e9fe5c93f559 CB_VERSION=6.6.0
RUN ln -s dummy.sh /usr/local/bin/iptables-save &&     ln -s dummy.sh /usr/local/bin/lvdisplay &&     ln -s dummy.sh /usr/local/bin/vgdisplay &&     ln -s dummy.sh /usr/local/bin/pvdisplay
# Tue, 13 Jul 2021 23:58:48 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_6.6.0-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=9b196cd7be81d7d6b179838e9d30164fdb7a1f27e96678e61e24e9fe5c93f559 CB_VERSION=6.6.0
RUN chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl
# Tue, 13 Jul 2021 23:58:48 GMT
COPY file:d816a67f62bfba76d2812cefbe92252afa13f3852775c3e68599df7741e90cb7 in / 
# Tue, 13 Jul 2021 23:58:48 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 13 Jul 2021 23:58:48 GMT
CMD ["couchbase-server"]
# Tue, 13 Jul 2021 23:58:49 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Tue, 13 Jul 2021 23:58:49 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:e7ae86ffe2df0787131a4c49ace1b018fd38d62929b007d86bdd1f825e56a852`  
		Last Modified: Tue, 13 Jul 2021 22:31:03 GMT  
		Size: 26.7 MB (26706145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f13c80c516e182839d6e6d6f7bc46ca9d41b722a2b3187d09071f91c78769b0e`  
		Last Modified: Wed, 14 Jul 2021 00:18:37 GMT  
		Size: 7.4 MB (7373539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fec6a0ae3c3d8baa9b4f7ebc733acffb0a42e2e7a0d032ceba2a7f11936f3e3`  
		Last Modified: Wed, 14 Jul 2021 00:18:32 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90b044bef35f71fc5ad909b9c120498dfcc56203b05466c42a9652aa7cfe76b7`  
		Last Modified: Wed, 14 Jul 2021 00:18:32 GMT  
		Size: 2.0 KB (1962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3533fd10906e91d51ac325e4b84d11198417748a608bfff173ffa3810057301a`  
		Last Modified: Wed, 14 Jul 2021 00:19:11 GMT  
		Size: 320.0 MB (320018573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60a370420cad28d201c6e76340ac6116eccac08d70000442c7bd76bb088f0b16`  
		Last Modified: Wed, 14 Jul 2021 00:18:32 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc17521d27f10560119aa2b999b4a33cfccad23b93b8bc8e10610d6edb89b0a2`  
		Last Modified: Wed, 14 Jul 2021 00:18:32 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5e4ec33c9da3da4066c087d543b96825b4684f158e879438b319baccf9fb81a`  
		Last Modified: Wed, 14 Jul 2021 00:18:30 GMT  
		Size: 279.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf8f3e5cbaba139c05a8c593cecf2b8248f37f5d88cca0f6ecf67300f34d00a0`  
		Last Modified: Wed, 14 Jul 2021 00:18:29 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e616737063650334ab279a00fe79613e34cd8cdac339085e854333779bd743fc`  
		Last Modified: Wed, 14 Jul 2021 00:18:30 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ddecd6c0f56654c2d2dc150ffce1983137207b7b7170fd1c2706d9619b2fcb6`  
		Last Modified: Wed, 14 Jul 2021 00:18:30 GMT  
		Size: 118.2 KB (118187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:587dcae06a9efe5aaccad9c7f80d654af05dad4f338ddf848becd288ca3e6363`  
		Last Modified: Wed, 14 Jul 2021 00:18:30 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchbase:community-7.0.0-beta`

```console
$ docker pull couchbase@sha256:5d0008523237a9302b6484725bdf8e14857a9ce15545317d88e49862b578da6e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `couchbase:community-7.0.0-beta` - linux; amd64

```console
$ docker pull couchbase@sha256:3b9810afe75f424a49322720be3a18d0b26b20cb8103ec8da32765bb99ae42e0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **434.0 MB (434032981 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:acb5a98d6d2a0c5a4af192f658a49de5c09c55c0e6e6d1df643a0ad4cdcf650f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Tue, 13 Jul 2021 22:29:34 GMT
ADD file:5c3d9d2597e01d1cee8513ff0e1344e7791e6f582be2cbd1d5777dd204780f1c in / 
# Tue, 13 Jul 2021 22:29:34 GMT
CMD ["bash"]
# Tue, 13 Jul 2021 23:50:49 GMT
LABEL maintainer=docker@couchbase.com
# Tue, 13 Jul 2021 23:51:15 GMT
RUN set -x &&     apt-get update &&     apt-get install -yq runit wget chrpath tzdata man     lsof lshw sysstat net-tools numactl bzip2 &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Tue, 13 Jul 2021 23:51:16 GMT
RUN if [ ! -x /usr/sbin/runsvdir-start ]; then         cp -a /etc/runit/2 /usr/sbin/runsvdir-start;     fi
# Tue, 13 Jul 2021 23:51:16 GMT
ARG CB_VERSION=7.0.0-beta
# Tue, 13 Jul 2021 23:51:17 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.0-beta
# Tue, 13 Jul 2021 23:53:16 GMT
ARG CB_PACKAGE=couchbase-server-community_7.0.0-beta-ubuntu20.04_amd64.deb
# Tue, 13 Jul 2021 23:53:16 GMT
ARG CB_SHA256=51e843e9d2b5ef746353d79c044f17e4f9be0866673bd6fda01da27a0edf9fc9
# Tue, 13 Jul 2021 23:53:17 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Tue, 13 Jul 2021 23:53:19 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.0.0-beta-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.0-beta CB_SHA256=51e843e9d2b5ef746353d79c044f17e4f9be0866673bd6fda01da27a0edf9fc9 CB_VERSION=7.0.0-beta
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Tue, 13 Jul 2021 23:54:19 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.0.0-beta-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.0-beta CB_SHA256=51e843e9d2b5ef746353d79c044f17e4f9be0866673bd6fda01da27a0edf9fc9 CB_VERSION=7.0.0-beta
RUN set -x &&     export INSTALL_DONT_START_SERVER=1 &&     wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE &&     echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - &&     apt-get update &&     apt-get install -y ./$CB_PACKAGE &&     rm -f ./$CB_PACKAGE &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Tue, 13 Jul 2021 23:54:22 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.0.0-beta-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.0-beta CB_SHA256=51e843e9d2b5ef746353d79c044f17e4f9be0866673bd6fda01da27a0edf9fc9 CB_VERSION=7.0.0-beta
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Tue, 13 Jul 2021 23:54:23 GMT
COPY file:d6a307209223b2df102f46f07fd186e09fac7114db2c965bb54097d3b4d3b989 in /etc/service/couchbase-server/run 
# Tue, 13 Jul 2021 23:54:24 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.0.0-beta-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.0-beta CB_SHA256=51e843e9d2b5ef746353d79c044f17e4f9be0866673bd6fda01da27a0edf9fc9 CB_VERSION=7.0.0-beta
RUN mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Tue, 13 Jul 2021 23:54:24 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Tue, 13 Jul 2021 23:54:25 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.0.0-beta-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.0-beta CB_SHA256=51e843e9d2b5ef746353d79c044f17e4f9be0866673bd6fda01da27a0edf9fc9 CB_VERSION=7.0.0-beta
RUN ln -s dummy.sh /usr/local/bin/iptables-save &&     ln -s dummy.sh /usr/local/bin/lvdisplay &&     ln -s dummy.sh /usr/local/bin/vgdisplay &&     ln -s dummy.sh /usr/local/bin/pvdisplay
# Tue, 13 Jul 2021 23:54:26 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.0.0-beta-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.0-beta CB_SHA256=51e843e9d2b5ef746353d79c044f17e4f9be0866673bd6fda01da27a0edf9fc9 CB_VERSION=7.0.0-beta
RUN chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl
# Tue, 13 Jul 2021 23:54:26 GMT
COPY file:d816a67f62bfba76d2812cefbe92252afa13f3852775c3e68599df7741e90cb7 in / 
# Tue, 13 Jul 2021 23:54:26 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 13 Jul 2021 23:54:27 GMT
CMD ["couchbase-server"]
# Tue, 13 Jul 2021 23:54:27 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Tue, 13 Jul 2021 23:54:27 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:a31c7b29f4ad2bd946738970f040825704a523ded1b9d6f9c7c7cafc6ab731df`  
		Last Modified: Tue, 13 Jul 2021 22:31:20 GMT  
		Size: 28.6 MB (28565863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27d820bb660a9b14c611213779ee0deee8781268242fd7d51bd43a6e638f6722`  
		Last Modified: Wed, 14 Jul 2021 00:14:56 GMT  
		Size: 8.3 MB (8286840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db40d5a53531bbb33b0d3feb0be6f6fd03a142fba87ac62d5487adf1928a6673`  
		Last Modified: Wed, 14 Jul 2021 00:14:50 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3896078d2dbca6a7536e29984383c46920bf7cd3141ea6cac17ba8e4299977c`  
		Last Modified: Wed, 14 Jul 2021 00:16:12 GMT  
		Size: 1.8 KB (1832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97842510154b16a7c5dbf2edac08fdc41c1e0c2d8e7ac46439fd9f47ef9f8256`  
		Last Modified: Wed, 14 Jul 2021 00:17:01 GMT  
		Size: 397.1 MB (397050034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a7f231548a787819c593246d5329e54c2ad5668fdd4f614129d3ff3f8b3eb2c`  
		Last Modified: Wed, 14 Jul 2021 00:16:12 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a8ed4e7f75eaa7ac8762e88f9b40be057826f25ee8060e5252874de967ce267`  
		Last Modified: Wed, 14 Jul 2021 00:16:12 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4378de9caaedf7a35ab05134cd9b174422ed1096c37b87b1018cfa0eea2b0994`  
		Last Modified: Wed, 14 Jul 2021 00:16:10 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bca8b4c46801d47f5dfae3f3408f245f6b64d2da9c71dbadfb66a2eb8200704`  
		Last Modified: Wed, 14 Jul 2021 00:16:10 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61c26a2366d66674c927eaa6f700b9781176042547dcd91b0a0aca9baae54684`  
		Last Modified: Wed, 14 Jul 2021 00:16:10 GMT  
		Size: 217.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18f56fadf88bc02d02c5d7361306d960fd3a49320bff1a645af18ae5bd0c0d70`  
		Last Modified: Wed, 14 Jul 2021 00:16:10 GMT  
		Size: 125.9 KB (125892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c819ee4ae2da728f31bf6f58740f18fe23ac33976bc62eb5d3ff41ea20d69ab`  
		Last Modified: Wed, 14 Jul 2021 00:16:10 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchbase:enterprise`

```console
$ docker pull couchbase@sha256:f81f332a99b86514042eaf1194603d65c37404c2686d1ae3ec3855056247be5c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `couchbase:enterprise` - linux; amd64

```console
$ docker pull couchbase@sha256:512ce0c9f998819d6e59f576cb24bc258775dfcfd52eee616427a5dec207eac3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **533.2 MB (533221032 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:00cc1f1af822aeda54b4e7859f621aaab1b8ac5a0eb0a97e0e89fdbdd7a005b1`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Tue, 13 Jul 2021 22:29:34 GMT
ADD file:5c3d9d2597e01d1cee8513ff0e1344e7791e6f582be2cbd1d5777dd204780f1c in / 
# Tue, 13 Jul 2021 22:29:34 GMT
CMD ["bash"]
# Tue, 13 Jul 2021 23:50:49 GMT
LABEL maintainer=docker@couchbase.com
# Tue, 13 Jul 2021 23:55:02 GMT
RUN set -x &&     apt-get update &&     apt-get install -yq runit wget chrpath tzdata     lsof lshw sysstat net-tools numactl bzip2 &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Tue, 13 Jul 2021 23:55:04 GMT
RUN if [ ! -x /usr/sbin/runsvdir-start ]; then         cp -a /etc/runit/2 /usr/sbin/runsvdir-start;     fi
# Tue, 13 Jul 2021 23:55:05 GMT
ARG CB_VERSION=6.6.2
# Tue, 13 Jul 2021 23:55:05 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.2
# Tue, 13 Jul 2021 23:55:06 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_6.6.2-ubuntu20.04_amd64.deb
# Tue, 13 Jul 2021 23:55:06 GMT
ARG CB_SHA256=41c033e6c1e98b0844a5cb5768e3769e7012d8374a6bd235c86e10db33b17afc
# Tue, 13 Jul 2021 23:55:06 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Tue, 13 Jul 2021 23:55:08 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.2-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.2 CB_SHA256=41c033e6c1e98b0844a5cb5768e3769e7012d8374a6bd235c86e10db33b17afc CB_VERSION=6.6.2
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Tue, 13 Jul 2021 23:56:27 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.2-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.2 CB_SHA256=41c033e6c1e98b0844a5cb5768e3769e7012d8374a6bd235c86e10db33b17afc CB_VERSION=6.6.2
RUN set -x &&     export INSTALL_DONT_START_SERVER=1 &&     wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE &&     echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - &&     apt-get update &&     apt-get install -y ./$CB_PACKAGE &&     rm -f ./$CB_PACKAGE &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Tue, 13 Jul 2021 23:56:32 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.2-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.2 CB_SHA256=41c033e6c1e98b0844a5cb5768e3769e7012d8374a6bd235c86e10db33b17afc CB_VERSION=6.6.2
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Tue, 13 Jul 2021 23:56:32 GMT
COPY file:d6a307209223b2df102f46f07fd186e09fac7114db2c965bb54097d3b4d3b989 in /etc/service/couchbase-server/run 
# Tue, 13 Jul 2021 23:56:34 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.2-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.2 CB_SHA256=41c033e6c1e98b0844a5cb5768e3769e7012d8374a6bd235c86e10db33b17afc CB_VERSION=6.6.2
RUN mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Tue, 13 Jul 2021 23:56:34 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Tue, 13 Jul 2021 23:56:36 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.2-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.2 CB_SHA256=41c033e6c1e98b0844a5cb5768e3769e7012d8374a6bd235c86e10db33b17afc CB_VERSION=6.6.2
RUN ln -s dummy.sh /usr/local/bin/iptables-save &&     ln -s dummy.sh /usr/local/bin/lvdisplay &&     ln -s dummy.sh /usr/local/bin/vgdisplay &&     ln -s dummy.sh /usr/local/bin/pvdisplay
# Tue, 13 Jul 2021 23:56:37 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.2-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.2 CB_SHA256=41c033e6c1e98b0844a5cb5768e3769e7012d8374a6bd235c86e10db33b17afc CB_VERSION=6.6.2
RUN chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl
# Tue, 13 Jul 2021 23:56:37 GMT
COPY file:d816a67f62bfba76d2812cefbe92252afa13f3852775c3e68599df7741e90cb7 in / 
# Tue, 13 Jul 2021 23:56:37 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 13 Jul 2021 23:56:38 GMT
CMD ["couchbase-server"]
# Tue, 13 Jul 2021 23:56:38 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Tue, 13 Jul 2021 23:56:38 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:a31c7b29f4ad2bd946738970f040825704a523ded1b9d6f9c7c7cafc6ab731df`  
		Last Modified: Tue, 13 Jul 2021 22:31:20 GMT  
		Size: 28.6 MB (28565863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f926d574d0b4b28f1f76deaa9aff956ebd84fca4c28ae00cb2342e321657edf3`  
		Last Modified: Wed, 14 Jul 2021 00:17:16 GMT  
		Size: 6.3 MB (6272606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ad3c9266985cc6da988565a76f19e617642668ced44547bb0e3b11af0301a00`  
		Last Modified: Wed, 14 Jul 2021 00:17:13 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23d163e5c68bca024eec49616679790ec8960fcde31526d8e29b5b1c38a9e872`  
		Last Modified: Wed, 14 Jul 2021 00:17:12 GMT  
		Size: 1.8 KB (1830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef2f5d79c085803411789e047e9ac102f5b17b68e9cffdcf72c199cabae6f6c0`  
		Last Modified: Wed, 14 Jul 2021 00:18:07 GMT  
		Size: 498.3 MB (498252316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c1d5eca3d063ae7effcc02e063c12fba349a3397808320570881e1cd400c468`  
		Last Modified: Wed, 14 Jul 2021 00:17:11 GMT  
		Size: 191.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63d346d7d3d4c52f9398df214716d61690c11261de8d80fdf0667a891d03f975`  
		Last Modified: Wed, 14 Jul 2021 00:17:11 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d45857737224785a1eab0c64e68eca963845fc8c29ba24f0f31cca91f9f73a4c`  
		Last Modified: Wed, 14 Jul 2021 00:17:09 GMT  
		Size: 281.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cce5e9dc1794cbdc1c5c738f15081bcfd141e67f3bea239ac3c2550551d5e76`  
		Last Modified: Wed, 14 Jul 2021 00:17:10 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:823f3f5bd72eb157355adc6d50c5df0e37548878cbad7b1ce94a902b039d5c61`  
		Last Modified: Wed, 14 Jul 2021 00:17:09 GMT  
		Size: 216.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ded2b29872fe46b0fdbeae64bbbbfdda02d84267a7b46538e6b749ce296fd3ce`  
		Last Modified: Wed, 14 Jul 2021 00:17:09 GMT  
		Size: 125.9 KB (125895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79733ad7ecdd3e0dc809f52676d3c3468febbb8306ca93d20ff073847c2f50ea`  
		Last Modified: Wed, 14 Jul 2021 00:17:09 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchbase:enterprise-6.0.1`

```console
$ docker pull couchbase@sha256:8a8ff02997140ad599d86bdda34d3850b70e8ae4c5bbd16ad3ccbd74d6f28f1c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `couchbase:enterprise-6.0.1` - linux; amd64

```console
$ docker pull couchbase@sha256:c43f4fb868048e12d20013e12446753da51bb2f9fb3175b303ac67a017569c7b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **455.2 MB (455212187 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4640a8f2c7d8cbfe809363c1881b4ed21c91deeb471fea7f15cbbb82a2bd7678`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Tue, 13 Jul 2021 22:29:15 GMT
ADD file:7274ece1917848683250bbeda9eacf6eb7510481cbaa177880e3a60b4133e35b in / 
# Tue, 13 Jul 2021 22:29:15 GMT
CMD ["bash"]
# Tue, 13 Jul 2021 23:56:52 GMT
LABEL maintainer=docker@couchbase.com
# Tue, 13 Jul 2021 23:59:19 GMT
RUN set -x &&     apt-get update &&     apt-get install -yq runit wget chrpath tzdata man     lsof lshw sysstat net-tools numactl python-httplib2 &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Tue, 13 Jul 2021 23:59:21 GMT
RUN if [ ! -x /usr/sbin/runsvdir-start ]; then         cp -a /etc/runit/2 /usr/sbin/runsvdir-start;     fi
# Wed, 14 Jul 2021 00:12:02 GMT
ARG CB_VERSION=6.0.1
# Wed, 14 Jul 2021 00:12:02 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.1
# Wed, 14 Jul 2021 00:12:02 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_6.0.1-ubuntu18.04_amd64.deb
# Wed, 14 Jul 2021 00:12:02 GMT
ARG CB_SHA256=68deed9ba855e2a84500ae99a787c415fc85b4d4dc1140be28ae6f56662bafea
# Wed, 14 Jul 2021 00:12:02 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Wed, 14 Jul 2021 00:12:03 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.1-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.1 CB_SHA256=68deed9ba855e2a84500ae99a787c415fc85b4d4dc1140be28ae6f56662bafea CB_VERSION=6.0.1
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Wed, 14 Jul 2021 00:12:58 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.1-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.1 CB_SHA256=68deed9ba855e2a84500ae99a787c415fc85b4d4dc1140be28ae6f56662bafea CB_VERSION=6.0.1
RUN set -x &&     export INSTALL_DONT_START_SERVER=1 &&     wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE &&     echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - &&     apt-get update &&     apt-get install -y ./$CB_PACKAGE &&     rm -f ./$CB_PACKAGE &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Wed, 14 Jul 2021 00:13:01 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.1-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.1 CB_SHA256=68deed9ba855e2a84500ae99a787c415fc85b4d4dc1140be28ae6f56662bafea CB_VERSION=6.0.1
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Wed, 14 Jul 2021 00:13:02 GMT
COPY file:d6a307209223b2df102f46f07fd186e09fac7114db2c965bb54097d3b4d3b989 in /etc/service/couchbase-server/run 
# Wed, 14 Jul 2021 00:13:03 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.1-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.1 CB_SHA256=68deed9ba855e2a84500ae99a787c415fc85b4d4dc1140be28ae6f56662bafea CB_VERSION=6.0.1
RUN mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Wed, 14 Jul 2021 00:13:03 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Wed, 14 Jul 2021 00:13:04 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.1-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.1 CB_SHA256=68deed9ba855e2a84500ae99a787c415fc85b4d4dc1140be28ae6f56662bafea CB_VERSION=6.0.1
RUN ln -s dummy.sh /usr/local/bin/iptables-save &&     ln -s dummy.sh /usr/local/bin/lvdisplay &&     ln -s dummy.sh /usr/local/bin/vgdisplay &&     ln -s dummy.sh /usr/local/bin/pvdisplay
# Wed, 14 Jul 2021 00:13:05 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.1-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.1 CB_SHA256=68deed9ba855e2a84500ae99a787c415fc85b4d4dc1140be28ae6f56662bafea CB_VERSION=6.0.1
RUN chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl
# Wed, 14 Jul 2021 00:13:05 GMT
COPY file:d816a67f62bfba76d2812cefbe92252afa13f3852775c3e68599df7741e90cb7 in / 
# Wed, 14 Jul 2021 00:13:05 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 14 Jul 2021 00:13:06 GMT
CMD ["couchbase-server"]
# Wed, 14 Jul 2021 00:13:06 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Wed, 14 Jul 2021 00:13:06 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:e7ae86ffe2df0787131a4c49ace1b018fd38d62929b007d86bdd1f825e56a852`  
		Last Modified: Tue, 13 Jul 2021 22:31:03 GMT  
		Size: 26.7 MB (26706145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31fa1d32440e9d869ef3438e5bfc1ad70daed7feb9b3a6d493072814a7eeea31`  
		Last Modified: Wed, 14 Jul 2021 00:19:32 GMT  
		Size: 15.9 MB (15922983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d3525b15f6ce5dff724448cd14b2fc3b4cff8ed696b456b2adf085528b5b2a2`  
		Last Modified: Wed, 14 Jul 2021 00:19:25 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72469b72d916f06e1121875a4727378ce8e398344dd61e579da3d0022b4f1cfe`  
		Last Modified: Wed, 14 Jul 2021 00:27:45 GMT  
		Size: 2.0 KB (1967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e74faa62fbf1d0b232e99e243790e3d245175d846416cc1ec738bce2039b01b6`  
		Last Modified: Wed, 14 Jul 2021 00:28:30 GMT  
		Size: 412.5 MB (412453000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3beaaa08e768bed1f2afbe8bbfa872cbdada91cfcf137379493ffefdcf01d2ad`  
		Last Modified: Wed, 14 Jul 2021 00:27:45 GMT  
		Size: 192.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3514b1349e8e01bb0852f5b739ad43c39ca84603a7ed474d3b0f2d42cc0c56ba`  
		Last Modified: Wed, 14 Jul 2021 00:27:45 GMT  
		Size: 482.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22667dd57035a153fc93b73e7620cd2d4a3d93b4dfaf27fd18fa4420e51d4839`  
		Last Modified: Wed, 14 Jul 2021 00:27:43 GMT  
		Size: 279.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4acae565a322b393595022ffd46a892c759fb8bff66f336be20a85859eb69d1`  
		Last Modified: Wed, 14 Jul 2021 00:27:43 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca61a2cf9c63ee0d58f811dedfcdc21b1450a7300912c4f39623bc94d29ccfdb`  
		Last Modified: Wed, 14 Jul 2021 00:27:43 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38fb7c3ce891142743af0f1d199837fea51349a8e0c0dc97a8ca6e1ff8e1ac68`  
		Last Modified: Wed, 14 Jul 2021 00:27:43 GMT  
		Size: 125.6 KB (125561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7607bacfa9601b6de1181ce26531001ed4e89ffcc99715593147ff8e34bca9f6`  
		Last Modified: Wed, 14 Jul 2021 00:27:43 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchbase:enterprise-6.0.2`

```console
$ docker pull couchbase@sha256:de9b5c24c995523a83b7dac6f8bfd73ff9a076f9a2f8722eb4d757368718eb25
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `couchbase:enterprise-6.0.2` - linux; amd64

```console
$ docker pull couchbase@sha256:8e02ada2704dcb26338bb9676552bae57a134806f8498eb6183e5506ba3e037d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **463.4 MB (463382896 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3447021d7164a497e86563e16ad4820b4fea2b0497b535f71b74e15f6cd1cac0`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Tue, 13 Jul 2021 22:29:15 GMT
ADD file:7274ece1917848683250bbeda9eacf6eb7510481cbaa177880e3a60b4133e35b in / 
# Tue, 13 Jul 2021 22:29:15 GMT
CMD ["bash"]
# Tue, 13 Jul 2021 23:56:52 GMT
LABEL maintainer=docker@couchbase.com
# Tue, 13 Jul 2021 23:59:19 GMT
RUN set -x &&     apt-get update &&     apt-get install -yq runit wget chrpath tzdata man     lsof lshw sysstat net-tools numactl python-httplib2 &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Tue, 13 Jul 2021 23:59:21 GMT
RUN if [ ! -x /usr/sbin/runsvdir-start ]; then         cp -a /etc/runit/2 /usr/sbin/runsvdir-start;     fi
# Wed, 14 Jul 2021 00:10:21 GMT
ARG CB_VERSION=6.0.2
# Wed, 14 Jul 2021 00:10:21 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.2
# Wed, 14 Jul 2021 00:10:21 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_6.0.2-ubuntu18.04_amd64.deb
# Wed, 14 Jul 2021 00:10:22 GMT
ARG CB_SHA256=5410a56cefd7a9c624a2d64e474058b43a90e8d66c73fea6b2a8b16a4f6fe14d
# Wed, 14 Jul 2021 00:10:22 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Wed, 14 Jul 2021 00:10:23 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.2-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.2 CB_SHA256=5410a56cefd7a9c624a2d64e474058b43a90e8d66c73fea6b2a8b16a4f6fe14d CB_VERSION=6.0.2
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Wed, 14 Jul 2021 00:11:22 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.2-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.2 CB_SHA256=5410a56cefd7a9c624a2d64e474058b43a90e8d66c73fea6b2a8b16a4f6fe14d CB_VERSION=6.0.2
RUN set -x &&     export INSTALL_DONT_START_SERVER=1 &&     wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE &&     echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - &&     apt-get update &&     apt-get install -y ./$CB_PACKAGE &&     rm -f ./$CB_PACKAGE &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Wed, 14 Jul 2021 00:11:44 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.2-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.2 CB_SHA256=5410a56cefd7a9c624a2d64e474058b43a90e8d66c73fea6b2a8b16a4f6fe14d CB_VERSION=6.0.2
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Wed, 14 Jul 2021 00:11:45 GMT
COPY file:d6a307209223b2df102f46f07fd186e09fac7114db2c965bb54097d3b4d3b989 in /etc/service/couchbase-server/run 
# Wed, 14 Jul 2021 00:11:46 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.2-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.2 CB_SHA256=5410a56cefd7a9c624a2d64e474058b43a90e8d66c73fea6b2a8b16a4f6fe14d CB_VERSION=6.0.2
RUN mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Wed, 14 Jul 2021 00:11:46 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Wed, 14 Jul 2021 00:11:47 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.2-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.2 CB_SHA256=5410a56cefd7a9c624a2d64e474058b43a90e8d66c73fea6b2a8b16a4f6fe14d CB_VERSION=6.0.2
RUN ln -s dummy.sh /usr/local/bin/iptables-save &&     ln -s dummy.sh /usr/local/bin/lvdisplay &&     ln -s dummy.sh /usr/local/bin/vgdisplay &&     ln -s dummy.sh /usr/local/bin/pvdisplay
# Wed, 14 Jul 2021 00:11:48 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.2-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.2 CB_SHA256=5410a56cefd7a9c624a2d64e474058b43a90e8d66c73fea6b2a8b16a4f6fe14d CB_VERSION=6.0.2
RUN chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl
# Wed, 14 Jul 2021 00:11:48 GMT
COPY file:d816a67f62bfba76d2812cefbe92252afa13f3852775c3e68599df7741e90cb7 in / 
# Wed, 14 Jul 2021 00:11:48 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 14 Jul 2021 00:11:48 GMT
CMD ["couchbase-server"]
# Wed, 14 Jul 2021 00:11:49 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Wed, 14 Jul 2021 00:11:49 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:e7ae86ffe2df0787131a4c49ace1b018fd38d62929b007d86bdd1f825e56a852`  
		Last Modified: Tue, 13 Jul 2021 22:31:03 GMT  
		Size: 26.7 MB (26706145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31fa1d32440e9d869ef3438e5bfc1ad70daed7feb9b3a6d493072814a7eeea31`  
		Last Modified: Wed, 14 Jul 2021 00:19:32 GMT  
		Size: 15.9 MB (15922983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d3525b15f6ce5dff724448cd14b2fc3b4cff8ed696b456b2adf085528b5b2a2`  
		Last Modified: Wed, 14 Jul 2021 00:19:25 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:603249a8f1cf0ebf8e676e6ef0d97a7b00c518fe588dc65c9f16b286de5d3b36`  
		Last Modified: Wed, 14 Jul 2021 00:26:49 GMT  
		Size: 2.0 KB (1969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2d9534b3cb8baf23f515c8f4b7762851a6f2e2df6e333c9401160236fa48652`  
		Last Modified: Wed, 14 Jul 2021 00:27:30 GMT  
		Size: 420.6 MB (420623712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8283ee9491704f4dae8db18fcb0eda7f2a3af0fd8514d793d9e217559047cec`  
		Last Modified: Wed, 14 Jul 2021 00:26:48 GMT  
		Size: 192.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20342722cce538c85079a8afa2a8f5a029ae981ec1a690f5ed86b8c2b8af0342`  
		Last Modified: Wed, 14 Jul 2021 00:26:48 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4afda51548d5dc06330535b173566c9209c2c3f0c6d7e43b6ae194f5bfe71253`  
		Last Modified: Wed, 14 Jul 2021 00:26:46 GMT  
		Size: 279.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0989364a544fa2d17eb0cf25aca82520310b7579e1156302d1d658d392a52f7`  
		Last Modified: Wed, 14 Jul 2021 00:26:46 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:061c137e4d88835c0cb2dd20e925a1b684f62e175d060d5ec379619f3409740f`  
		Last Modified: Wed, 14 Jul 2021 00:26:46 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05303718e4140b55b907377dfeba8672fd0ca32a0139a191030d221f374aa84f`  
		Last Modified: Wed, 14 Jul 2021 00:26:46 GMT  
		Size: 125.6 KB (125561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9eb0f57abd2ba900921d5e40f9576d7e21f0a593e230604d7de7dcce7088837`  
		Last Modified: Wed, 14 Jul 2021 00:26:46 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchbase:enterprise-6.0.3`

```console
$ docker pull couchbase@sha256:2ca33951fcd428a03147f116657c80f76dc896bf5a50d905343da158440aa8fc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `couchbase:enterprise-6.0.3` - linux; amd64

```console
$ docker pull couchbase@sha256:324edff57c7aee2a917507acbdbc43474bbb02dbfea393467fae937cafe810bf
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **465.9 MB (465906748 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c47f7d8e17933f975153e288308212811e5463ecef3aed61207441a5aff8a1fd`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Tue, 13 Jul 2021 22:29:15 GMT
ADD file:7274ece1917848683250bbeda9eacf6eb7510481cbaa177880e3a60b4133e35b in / 
# Tue, 13 Jul 2021 22:29:15 GMT
CMD ["bash"]
# Tue, 13 Jul 2021 23:56:52 GMT
LABEL maintainer=docker@couchbase.com
# Tue, 13 Jul 2021 23:59:19 GMT
RUN set -x &&     apt-get update &&     apt-get install -yq runit wget chrpath tzdata man     lsof lshw sysstat net-tools numactl python-httplib2 &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Tue, 13 Jul 2021 23:59:21 GMT
RUN if [ ! -x /usr/sbin/runsvdir-start ]; then         cp -a /etc/runit/2 /usr/sbin/runsvdir-start;     fi
# Wed, 14 Jul 2021 00:09:09 GMT
ARG CB_VERSION=6.0.3
# Wed, 14 Jul 2021 00:09:10 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.3
# Wed, 14 Jul 2021 00:09:10 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_6.0.3-ubuntu18.04_amd64.deb
# Wed, 14 Jul 2021 00:09:10 GMT
ARG CB_SHA256=8ee814ea8d99141de5493a6a24423c6a5dc4e01b8393dce87ca1639630315382
# Wed, 14 Jul 2021 00:09:10 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Wed, 14 Jul 2021 00:09:11 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.3-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.3 CB_SHA256=8ee814ea8d99141de5493a6a24423c6a5dc4e01b8393dce87ca1639630315382 CB_VERSION=6.0.3
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Wed, 14 Jul 2021 00:10:10 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.3-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.3 CB_SHA256=8ee814ea8d99141de5493a6a24423c6a5dc4e01b8393dce87ca1639630315382 CB_VERSION=6.0.3
RUN set -x &&     export INSTALL_DONT_START_SERVER=1 &&     wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE &&     echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - &&     apt-get update &&     apt-get install -y ./$CB_PACKAGE &&     rm -f ./$CB_PACKAGE &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Wed, 14 Jul 2021 00:10:13 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.3-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.3 CB_SHA256=8ee814ea8d99141de5493a6a24423c6a5dc4e01b8393dce87ca1639630315382 CB_VERSION=6.0.3
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Wed, 14 Jul 2021 00:10:14 GMT
COPY file:d6a307209223b2df102f46f07fd186e09fac7114db2c965bb54097d3b4d3b989 in /etc/service/couchbase-server/run 
# Wed, 14 Jul 2021 00:10:15 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.3-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.3 CB_SHA256=8ee814ea8d99141de5493a6a24423c6a5dc4e01b8393dce87ca1639630315382 CB_VERSION=6.0.3
RUN mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Wed, 14 Jul 2021 00:10:15 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Wed, 14 Jul 2021 00:10:16 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.3-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.3 CB_SHA256=8ee814ea8d99141de5493a6a24423c6a5dc4e01b8393dce87ca1639630315382 CB_VERSION=6.0.3
RUN ln -s dummy.sh /usr/local/bin/iptables-save &&     ln -s dummy.sh /usr/local/bin/lvdisplay &&     ln -s dummy.sh /usr/local/bin/vgdisplay &&     ln -s dummy.sh /usr/local/bin/pvdisplay
# Wed, 14 Jul 2021 00:10:17 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.3-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.3 CB_SHA256=8ee814ea8d99141de5493a6a24423c6a5dc4e01b8393dce87ca1639630315382 CB_VERSION=6.0.3
RUN chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl
# Wed, 14 Jul 2021 00:10:17 GMT
COPY file:d816a67f62bfba76d2812cefbe92252afa13f3852775c3e68599df7741e90cb7 in / 
# Wed, 14 Jul 2021 00:10:17 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 14 Jul 2021 00:10:17 GMT
CMD ["couchbase-server"]
# Wed, 14 Jul 2021 00:10:18 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Wed, 14 Jul 2021 00:10:18 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:e7ae86ffe2df0787131a4c49ace1b018fd38d62929b007d86bdd1f825e56a852`  
		Last Modified: Tue, 13 Jul 2021 22:31:03 GMT  
		Size: 26.7 MB (26706145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31fa1d32440e9d869ef3438e5bfc1ad70daed7feb9b3a6d493072814a7eeea31`  
		Last Modified: Wed, 14 Jul 2021 00:19:32 GMT  
		Size: 15.9 MB (15922983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d3525b15f6ce5dff724448cd14b2fc3b4cff8ed696b456b2adf085528b5b2a2`  
		Last Modified: Wed, 14 Jul 2021 00:19:25 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a87df52b5ea3cc49700b53c210b5ebe99ddf87056405f040593913d9f8c47599`  
		Last Modified: Wed, 14 Jul 2021 00:25:53 GMT  
		Size: 2.0 KB (1971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efe050fd8c96c1333e825325cf2a385fb2249e29d2a86295a8e44fd26e78dd1e`  
		Last Modified: Wed, 14 Jul 2021 00:26:34 GMT  
		Size: 423.1 MB (423147566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8af8a25dfae3cd32c9b437073247d6a3f79fc9f14a2c35adb730a5503f9e60c9`  
		Last Modified: Wed, 14 Jul 2021 00:25:53 GMT  
		Size: 191.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02bc5e818d0b081fb9790b5b3167453695cd69f167069b9b06ca6d70bfab8cf7`  
		Last Modified: Wed, 14 Jul 2021 00:25:53 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ccf28a52d832dcbb2337c7c99775f02c93935a45ce1dea2ec475bd16c435a5f`  
		Last Modified: Wed, 14 Jul 2021 00:25:51 GMT  
		Size: 279.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cd5d7cd6e13a56c0d0b842454f92f5cc3dd403a7291e11f4cbf93ff55ec0ab1`  
		Last Modified: Wed, 14 Jul 2021 00:25:51 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afa89f6d24da70e562ae6fe8dfcc487049d11f579e6030507ec9c9f5a424be6c`  
		Last Modified: Wed, 14 Jul 2021 00:25:51 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c9a21894ad164f0f760611f64405966f7ae780078ca8608fe9ae565cf566550`  
		Last Modified: Wed, 14 Jul 2021 00:25:51 GMT  
		Size: 125.6 KB (125558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90487eb210f8d4f901f84dc0b9e61ccd2137b3c9d647fa38d7b708b44591b958`  
		Last Modified: Wed, 14 Jul 2021 00:25:51 GMT  
		Size: 858.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchbase:enterprise-6.0.4`

```console
$ docker pull couchbase@sha256:b9898e94785b49ddba89e600193dde03e616a41e01676a743dbfb57f4c4d8110
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `couchbase:enterprise-6.0.4` - linux; amd64

```console
$ docker pull couchbase@sha256:96f5f253b16b7bfef403f349c39c890efb991a3c76c53b8ff5df4e4554b8adc9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **467.2 MB (467173553 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3618f344592fa4de4ecc882a29a993cf8b8b094c2fb7f67ccf477d57095635b4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Tue, 13 Jul 2021 22:29:15 GMT
ADD file:7274ece1917848683250bbeda9eacf6eb7510481cbaa177880e3a60b4133e35b in / 
# Tue, 13 Jul 2021 22:29:15 GMT
CMD ["bash"]
# Tue, 13 Jul 2021 23:56:52 GMT
LABEL maintainer=docker@couchbase.com
# Tue, 13 Jul 2021 23:59:19 GMT
RUN set -x &&     apt-get update &&     apt-get install -yq runit wget chrpath tzdata man     lsof lshw sysstat net-tools numactl python-httplib2 &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Tue, 13 Jul 2021 23:59:21 GMT
RUN if [ ! -x /usr/sbin/runsvdir-start ]; then         cp -a /etc/runit/2 /usr/sbin/runsvdir-start;     fi
# Wed, 14 Jul 2021 00:07:57 GMT
ARG CB_VERSION=6.0.4
# Wed, 14 Jul 2021 00:07:58 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.4
# Wed, 14 Jul 2021 00:07:58 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_6.0.4-ubuntu18.04_amd64.deb
# Wed, 14 Jul 2021 00:07:58 GMT
ARG CB_SHA256=7dbe8dd074f9cabea69468ea488f9ffc19c04dab8fc2e98c937fa32704982aff
# Wed, 14 Jul 2021 00:07:58 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Wed, 14 Jul 2021 00:07:59 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.4-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.4 CB_SHA256=7dbe8dd074f9cabea69468ea488f9ffc19c04dab8fc2e98c937fa32704982aff CB_VERSION=6.0.4
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Wed, 14 Jul 2021 00:08:57 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.4-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.4 CB_SHA256=7dbe8dd074f9cabea69468ea488f9ffc19c04dab8fc2e98c937fa32704982aff CB_VERSION=6.0.4
RUN set -x &&     export INSTALL_DONT_START_SERVER=1 &&     wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE &&     echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - &&     apt-get update &&     apt-get install -y ./$CB_PACKAGE &&     rm -f ./$CB_PACKAGE &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Wed, 14 Jul 2021 00:09:01 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.4-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.4 CB_SHA256=7dbe8dd074f9cabea69468ea488f9ffc19c04dab8fc2e98c937fa32704982aff CB_VERSION=6.0.4
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Wed, 14 Jul 2021 00:09:01 GMT
COPY file:d6a307209223b2df102f46f07fd186e09fac7114db2c965bb54097d3b4d3b989 in /etc/service/couchbase-server/run 
# Wed, 14 Jul 2021 00:09:02 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.4-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.4 CB_SHA256=7dbe8dd074f9cabea69468ea488f9ffc19c04dab8fc2e98c937fa32704982aff CB_VERSION=6.0.4
RUN mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Wed, 14 Jul 2021 00:09:02 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Wed, 14 Jul 2021 00:09:03 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.4-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.4 CB_SHA256=7dbe8dd074f9cabea69468ea488f9ffc19c04dab8fc2e98c937fa32704982aff CB_VERSION=6.0.4
RUN ln -s dummy.sh /usr/local/bin/iptables-save &&     ln -s dummy.sh /usr/local/bin/lvdisplay &&     ln -s dummy.sh /usr/local/bin/vgdisplay &&     ln -s dummy.sh /usr/local/bin/pvdisplay
# Wed, 14 Jul 2021 00:09:04 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.4-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.4 CB_SHA256=7dbe8dd074f9cabea69468ea488f9ffc19c04dab8fc2e98c937fa32704982aff CB_VERSION=6.0.4
RUN chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl
# Wed, 14 Jul 2021 00:09:04 GMT
COPY file:d816a67f62bfba76d2812cefbe92252afa13f3852775c3e68599df7741e90cb7 in / 
# Wed, 14 Jul 2021 00:09:05 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 14 Jul 2021 00:09:05 GMT
CMD ["couchbase-server"]
# Wed, 14 Jul 2021 00:09:05 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Wed, 14 Jul 2021 00:09:05 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:e7ae86ffe2df0787131a4c49ace1b018fd38d62929b007d86bdd1f825e56a852`  
		Last Modified: Tue, 13 Jul 2021 22:31:03 GMT  
		Size: 26.7 MB (26706145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31fa1d32440e9d869ef3438e5bfc1ad70daed7feb9b3a6d493072814a7eeea31`  
		Last Modified: Wed, 14 Jul 2021 00:19:32 GMT  
		Size: 15.9 MB (15922983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d3525b15f6ce5dff724448cd14b2fc3b4cff8ed696b456b2adf085528b5b2a2`  
		Last Modified: Wed, 14 Jul 2021 00:19:25 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf3a3b7c6bc46ae495064fe52418dd279fc078f7a5b5559856421ec70a8ad99a`  
		Last Modified: Wed, 14 Jul 2021 00:24:58 GMT  
		Size: 2.0 KB (1967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba1cb08d8fd0ea9125e7f2d87cf3bd3f1ee8e2eb8785405e904163c7af85c13d`  
		Last Modified: Wed, 14 Jul 2021 00:25:39 GMT  
		Size: 424.4 MB (424414373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64dbdc5cb335c4fa20a1529faa766256f539e06f80663d2c3c6ac8d2e4e36379`  
		Last Modified: Wed, 14 Jul 2021 00:24:58 GMT  
		Size: 191.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f865105c048695dd483dfceb73c7027a13cc43c5b67a71ec9ce517ad7e869c8`  
		Last Modified: Wed, 14 Jul 2021 00:24:58 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fc175912ab464cab161e719cbcb7cad5f1ec658c6d06b6cf8690ba64eaf9368`  
		Last Modified: Wed, 14 Jul 2021 00:24:55 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc110d3d902ab016c5da32e4acf88ee20c51e7d5ae85b38d4199a74e6b673054`  
		Last Modified: Wed, 14 Jul 2021 00:24:56 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6ca51cc5fe51f0ca1792ce4e4a1e5d7ab3c454ecd5c8e94d6821cb50b08567b`  
		Last Modified: Wed, 14 Jul 2021 00:24:55 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fb188386e971655790488f4d29d36409eb1237a69784fe157f06cb6be00bbde`  
		Last Modified: Wed, 14 Jul 2021 00:24:56 GMT  
		Size: 125.6 KB (125563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57b04265b4d19130c58c8c2a29aa008d44939493416384508cee4656d92556c4`  
		Last Modified: Wed, 14 Jul 2021 00:24:55 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchbase:enterprise-6.0.5`

```console
$ docker pull couchbase@sha256:c2794e735530e77e4001b1743f4de9249140987d29aa27bd3208490b6148feac
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `couchbase:enterprise-6.0.5` - linux; amd64

```console
$ docker pull couchbase@sha256:6ac872346667262e6edc81280bd419cf62d39f56841fd5f984025003bfbeb4c9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **466.1 MB (466121401 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:75b0afca95bffb603ee6a94f16eb407d7d007aec985f78c3f19ca840f73039ae`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Tue, 13 Jul 2021 22:29:15 GMT
ADD file:7274ece1917848683250bbeda9eacf6eb7510481cbaa177880e3a60b4133e35b in / 
# Tue, 13 Jul 2021 22:29:15 GMT
CMD ["bash"]
# Tue, 13 Jul 2021 23:56:52 GMT
LABEL maintainer=docker@couchbase.com
# Tue, 13 Jul 2021 23:59:19 GMT
RUN set -x &&     apt-get update &&     apt-get install -yq runit wget chrpath tzdata man     lsof lshw sysstat net-tools numactl python-httplib2 &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Tue, 13 Jul 2021 23:59:21 GMT
RUN if [ ! -x /usr/sbin/runsvdir-start ]; then         cp -a /etc/runit/2 /usr/sbin/runsvdir-start;     fi
# Tue, 13 Jul 2021 23:59:21 GMT
ARG CB_VERSION=6.0.5
# Tue, 13 Jul 2021 23:59:21 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.5
# Tue, 13 Jul 2021 23:59:21 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_6.0.5-ubuntu18.04_amd64.deb
# Tue, 13 Jul 2021 23:59:22 GMT
ARG CB_SHA256=6b152590867a58d771cffc22774d3cd66c916defcbeeeb339aca8d0a8e6d7f8d
# Tue, 13 Jul 2021 23:59:22 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Tue, 13 Jul 2021 23:59:23 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.5-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.5 CB_SHA256=6b152590867a58d771cffc22774d3cd66c916defcbeeeb339aca8d0a8e6d7f8d CB_VERSION=6.0.5
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Wed, 14 Jul 2021 00:00:43 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.5-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.5 CB_SHA256=6b152590867a58d771cffc22774d3cd66c916defcbeeeb339aca8d0a8e6d7f8d CB_VERSION=6.0.5
RUN set -x &&     export INSTALL_DONT_START_SERVER=1 &&     wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE &&     echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - &&     apt-get update &&     apt-get install -y ./$CB_PACKAGE &&     rm -f ./$CB_PACKAGE &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Wed, 14 Jul 2021 00:00:48 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.5-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.5 CB_SHA256=6b152590867a58d771cffc22774d3cd66c916defcbeeeb339aca8d0a8e6d7f8d CB_VERSION=6.0.5
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Wed, 14 Jul 2021 00:00:48 GMT
COPY file:d6a307209223b2df102f46f07fd186e09fac7114db2c965bb54097d3b4d3b989 in /etc/service/couchbase-server/run 
# Wed, 14 Jul 2021 00:00:51 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.5-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.5 CB_SHA256=6b152590867a58d771cffc22774d3cd66c916defcbeeeb339aca8d0a8e6d7f8d CB_VERSION=6.0.5
RUN mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Wed, 14 Jul 2021 00:00:51 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Wed, 14 Jul 2021 00:00:53 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.5-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.5 CB_SHA256=6b152590867a58d771cffc22774d3cd66c916defcbeeeb339aca8d0a8e6d7f8d CB_VERSION=6.0.5
RUN ln -s dummy.sh /usr/local/bin/iptables-save &&     ln -s dummy.sh /usr/local/bin/lvdisplay &&     ln -s dummy.sh /usr/local/bin/vgdisplay &&     ln -s dummy.sh /usr/local/bin/pvdisplay
# Wed, 14 Jul 2021 00:00:55 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.5-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.5 CB_SHA256=6b152590867a58d771cffc22774d3cd66c916defcbeeeb339aca8d0a8e6d7f8d CB_VERSION=6.0.5
RUN chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl
# Wed, 14 Jul 2021 00:00:56 GMT
COPY file:d816a67f62bfba76d2812cefbe92252afa13f3852775c3e68599df7741e90cb7 in / 
# Wed, 14 Jul 2021 00:00:56 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 14 Jul 2021 00:00:56 GMT
CMD ["couchbase-server"]
# Wed, 14 Jul 2021 00:00:57 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Wed, 14 Jul 2021 00:00:57 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:e7ae86ffe2df0787131a4c49ace1b018fd38d62929b007d86bdd1f825e56a852`  
		Last Modified: Tue, 13 Jul 2021 22:31:03 GMT  
		Size: 26.7 MB (26706145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31fa1d32440e9d869ef3438e5bfc1ad70daed7feb9b3a6d493072814a7eeea31`  
		Last Modified: Wed, 14 Jul 2021 00:19:32 GMT  
		Size: 15.9 MB (15922983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d3525b15f6ce5dff724448cd14b2fc3b4cff8ed696b456b2adf085528b5b2a2`  
		Last Modified: Wed, 14 Jul 2021 00:19:25 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5037ab8e061c8ac8dad72c6524e345936c64f4b921675a172bc0e5010f417518`  
		Last Modified: Wed, 14 Jul 2021 00:19:25 GMT  
		Size: 2.0 KB (1965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:135a2ec4d68ab3615eee5adf0ba4849c3acded84ea71e89f3c4f90f3f2b46000`  
		Last Modified: Wed, 14 Jul 2021 00:20:06 GMT  
		Size: 423.4 MB (423362229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6252f42dee8be81dbc56a7d42819069889a1b6f05ffc9c7ae2bfb0fc5a96d21e`  
		Last Modified: Wed, 14 Jul 2021 00:19:25 GMT  
		Size: 192.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:367d2d96dc36d6ec07050b65770fc6156bff82ccbc4ae7cdbc9f1da33cc4d7c6`  
		Last Modified: Wed, 14 Jul 2021 00:19:25 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25344e400b0d1939e6d3604c68eb98da50e8ec09ba94b679cb5371d705c7fcf6`  
		Last Modified: Wed, 14 Jul 2021 00:19:22 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:433d9be8d5ce4f880ffb7c99b47c03e88c5d03f00da401df464f2d6c1b2beb0e`  
		Last Modified: Wed, 14 Jul 2021 00:19:22 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3a01dae8f15dac3896e3330d6a1fbf8c72daf2f103a232c6f3980fcd8eebff8`  
		Last Modified: Wed, 14 Jul 2021 00:19:22 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12f0a82152aca4cbcba222cc0a294adfd643c40c83ba98369a78679d25e669db`  
		Last Modified: Wed, 14 Jul 2021 00:19:22 GMT  
		Size: 125.6 KB (125558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f758726bd5203a0462981dad419faed39c665522bdf6c589c50b0ab5de2f4fc`  
		Last Modified: Wed, 14 Jul 2021 00:19:22 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchbase:enterprise-6.5.0`

```console
$ docker pull couchbase@sha256:1c2654f480ef8427c0362829bdb0e6bda8645489ae87ddf0c7eb4424d43926de
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `couchbase:enterprise-6.5.0` - linux; amd64

```console
$ docker pull couchbase@sha256:0ba3a6d5d0b1f8b73573443c85cfb167c56d785e5939fdeb85e19bfe853f7a3d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **542.2 MB (542234395 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b9e0bc7184a3f3607e09fb1c6277bef11bb409d1102601eb2315679ea469fcda`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Tue, 13 Jul 2021 22:29:15 GMT
ADD file:7274ece1917848683250bbeda9eacf6eb7510481cbaa177880e3a60b4133e35b in / 
# Tue, 13 Jul 2021 22:29:15 GMT
CMD ["bash"]
# Tue, 13 Jul 2021 23:56:52 GMT
LABEL maintainer=docker@couchbase.com
# Tue, 13 Jul 2021 23:57:29 GMT
RUN set -x &&     apt-get update &&     apt-get install -yq runit wget chrpath tzdata man     lsof lshw sysstat net-tools numactl bzip2 &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Tue, 13 Jul 2021 23:57:32 GMT
RUN if [ ! -x /usr/sbin/runsvdir-start ]; then         cp -a /etc/runit/2 /usr/sbin/runsvdir-start;     fi
# Wed, 14 Jul 2021 00:06:32 GMT
ARG CB_VERSION=6.5.0
# Wed, 14 Jul 2021 00:06:32 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/6.5.0
# Wed, 14 Jul 2021 00:06:32 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_6.5.0-ubuntu18.04_amd64.deb
# Wed, 14 Jul 2021 00:06:33 GMT
ARG CB_SHA256=b4cafdc048b0caba85c24b90e6823e9ec2adc32061cafc527ddc99d706d6bc05
# Wed, 14 Jul 2021 00:06:33 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Wed, 14 Jul 2021 00:06:34 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.5.0-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.5.0 CB_SHA256=b4cafdc048b0caba85c24b90e6823e9ec2adc32061cafc527ddc99d706d6bc05 CB_VERSION=6.5.0
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Wed, 14 Jul 2021 00:07:40 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.5.0-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.5.0 CB_SHA256=b4cafdc048b0caba85c24b90e6823e9ec2adc32061cafc527ddc99d706d6bc05 CB_VERSION=6.5.0
RUN set -x &&     export INSTALL_DONT_START_SERVER=1 &&     wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE &&     echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - &&     apt-get update &&     apt-get install -y ./$CB_PACKAGE &&     rm -f ./$CB_PACKAGE &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Wed, 14 Jul 2021 00:07:44 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.5.0-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.5.0 CB_SHA256=b4cafdc048b0caba85c24b90e6823e9ec2adc32061cafc527ddc99d706d6bc05 CB_VERSION=6.5.0
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Wed, 14 Jul 2021 00:07:44 GMT
COPY file:d6a307209223b2df102f46f07fd186e09fac7114db2c965bb54097d3b4d3b989 in /etc/service/couchbase-server/run 
# Wed, 14 Jul 2021 00:07:45 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.5.0-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.5.0 CB_SHA256=b4cafdc048b0caba85c24b90e6823e9ec2adc32061cafc527ddc99d706d6bc05 CB_VERSION=6.5.0
RUN mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Wed, 14 Jul 2021 00:07:46 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Wed, 14 Jul 2021 00:07:47 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.5.0-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.5.0 CB_SHA256=b4cafdc048b0caba85c24b90e6823e9ec2adc32061cafc527ddc99d706d6bc05 CB_VERSION=6.5.0
RUN ln -s dummy.sh /usr/local/bin/iptables-save &&     ln -s dummy.sh /usr/local/bin/lvdisplay &&     ln -s dummy.sh /usr/local/bin/vgdisplay &&     ln -s dummy.sh /usr/local/bin/pvdisplay
# Wed, 14 Jul 2021 00:07:48 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.5.0-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.5.0 CB_SHA256=b4cafdc048b0caba85c24b90e6823e9ec2adc32061cafc527ddc99d706d6bc05 CB_VERSION=6.5.0
RUN chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl
# Wed, 14 Jul 2021 00:07:48 GMT
COPY file:d816a67f62bfba76d2812cefbe92252afa13f3852775c3e68599df7741e90cb7 in / 
# Wed, 14 Jul 2021 00:07:48 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 14 Jul 2021 00:07:49 GMT
CMD ["couchbase-server"]
# Wed, 14 Jul 2021 00:07:49 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Wed, 14 Jul 2021 00:07:49 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:e7ae86ffe2df0787131a4c49ace1b018fd38d62929b007d86bdd1f825e56a852`  
		Last Modified: Tue, 13 Jul 2021 22:31:03 GMT  
		Size: 26.7 MB (26706145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f13c80c516e182839d6e6d6f7bc46ca9d41b722a2b3187d09071f91c78769b0e`  
		Last Modified: Wed, 14 Jul 2021 00:18:37 GMT  
		Size: 7.4 MB (7373539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fec6a0ae3c3d8baa9b4f7ebc733acffb0a42e2e7a0d032ceba2a7f11936f3e3`  
		Last Modified: Wed, 14 Jul 2021 00:18:32 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac6ea85b7eae8b65ce8bf5a4eb8113662d048fe6e441bf9a4991e60bb7dd7885`  
		Last Modified: Wed, 14 Jul 2021 00:23:48 GMT  
		Size: 2.0 KB (1967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a8011aa8d5035f6fc3dbe7d7cb0b105c9b577965b9c71df01c62496289b2b10`  
		Last Modified: Wed, 14 Jul 2021 00:24:42 GMT  
		Size: 508.0 MB (508032027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02ff4341f265f333cc4ceb54256f2d610e00758f05d923a042917ee66ad70511`  
		Last Modified: Wed, 14 Jul 2021 00:23:48 GMT  
		Size: 190.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b658f87e1af28571f5360142615d3d834cb1522744e1b723fbaabfe422d6379`  
		Last Modified: Wed, 14 Jul 2021 00:23:48 GMT  
		Size: 480.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20d662cda6464532e5fb76a7e6360315fe834be02bd469181a85c415a5290f0d`  
		Last Modified: Wed, 14 Jul 2021 00:23:45 GMT  
		Size: 280.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7922c732bdc393a6987356e98912481476b4263fa2b1b28d8d7909f2449509d`  
		Last Modified: Wed, 14 Jul 2021 00:23:45 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6636355b99c052dac173273a1e5ee36763b074a24efbf5b29a671a74c3fd2ef`  
		Last Modified: Wed, 14 Jul 2021 00:23:45 GMT  
		Size: 217.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71b3aaa3c22f7b1f6f546d2d79ca875bbf38e4b50142dba6a3b2a81398b58ab6`  
		Last Modified: Wed, 14 Jul 2021 00:23:45 GMT  
		Size: 118.2 KB (118191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5b9899b2afec881cb60078d0c8957eb38376978a5458875a029f6073abeaca7`  
		Last Modified: Wed, 14 Jul 2021 00:23:45 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchbase:enterprise-6.5.1`

```console
$ docker pull couchbase@sha256:4d349e3b91534085e4b13c9b4e0ed589f522d756ee4d59d763fa55cb72e5e6dc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `couchbase:enterprise-6.5.1` - linux; amd64

```console
$ docker pull couchbase@sha256:cbfc1f569121926922fc536dd0bb9c6eb28fb22c8ff1ce60c28a35adf3a8122a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **501.5 MB (501508958 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8fd049d1538297e8768ff6ebd7a142eccc58415a7575324e34c3a44c38d57418`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Tue, 13 Jul 2021 22:29:15 GMT
ADD file:7274ece1917848683250bbeda9eacf6eb7510481cbaa177880e3a60b4133e35b in / 
# Tue, 13 Jul 2021 22:29:15 GMT
CMD ["bash"]
# Tue, 13 Jul 2021 23:56:52 GMT
LABEL maintainer=docker@couchbase.com
# Tue, 13 Jul 2021 23:57:29 GMT
RUN set -x &&     apt-get update &&     apt-get install -yq runit wget chrpath tzdata man     lsof lshw sysstat net-tools numactl bzip2 &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Tue, 13 Jul 2021 23:57:32 GMT
RUN if [ ! -x /usr/sbin/runsvdir-start ]; then         cp -a /etc/runit/2 /usr/sbin/runsvdir-start;     fi
# Wed, 14 Jul 2021 00:04:52 GMT
ARG CB_VERSION=6.5.1
# Wed, 14 Jul 2021 00:04:52 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/6.5.1
# Wed, 14 Jul 2021 00:04:52 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_6.5.1-ubuntu18.04_amd64.deb
# Wed, 14 Jul 2021 00:04:53 GMT
ARG CB_SHA256=992fc9aef85c210cc2d782a1726f2ef56ceb322fd67c2e95500e276ff106e6ff
# Wed, 14 Jul 2021 00:04:53 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Wed, 14 Jul 2021 00:04:55 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.5.1-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.5.1 CB_SHA256=992fc9aef85c210cc2d782a1726f2ef56ceb322fd67c2e95500e276ff106e6ff CB_VERSION=6.5.1
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Wed, 14 Jul 2021 00:06:19 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.5.1-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.5.1 CB_SHA256=992fc9aef85c210cc2d782a1726f2ef56ceb322fd67c2e95500e276ff106e6ff CB_VERSION=6.5.1
RUN set -x &&     export INSTALL_DONT_START_SERVER=1 &&     wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE &&     echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - &&     apt-get update &&     apt-get install -y ./$CB_PACKAGE &&     rm -f ./$CB_PACKAGE &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Wed, 14 Jul 2021 00:06:23 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.5.1-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.5.1 CB_SHA256=992fc9aef85c210cc2d782a1726f2ef56ceb322fd67c2e95500e276ff106e6ff CB_VERSION=6.5.1
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Wed, 14 Jul 2021 00:06:23 GMT
COPY file:d6a307209223b2df102f46f07fd186e09fac7114db2c965bb54097d3b4d3b989 in /etc/service/couchbase-server/run 
# Wed, 14 Jul 2021 00:06:25 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.5.1-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.5.1 CB_SHA256=992fc9aef85c210cc2d782a1726f2ef56ceb322fd67c2e95500e276ff106e6ff CB_VERSION=6.5.1
RUN mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Wed, 14 Jul 2021 00:06:25 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Wed, 14 Jul 2021 00:06:26 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.5.1-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.5.1 CB_SHA256=992fc9aef85c210cc2d782a1726f2ef56ceb322fd67c2e95500e276ff106e6ff CB_VERSION=6.5.1
RUN ln -s dummy.sh /usr/local/bin/iptables-save &&     ln -s dummy.sh /usr/local/bin/lvdisplay &&     ln -s dummy.sh /usr/local/bin/vgdisplay &&     ln -s dummy.sh /usr/local/bin/pvdisplay
# Wed, 14 Jul 2021 00:06:28 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.5.1-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.5.1 CB_SHA256=992fc9aef85c210cc2d782a1726f2ef56ceb322fd67c2e95500e276ff106e6ff CB_VERSION=6.5.1
RUN chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl
# Wed, 14 Jul 2021 00:06:28 GMT
COPY file:d816a67f62bfba76d2812cefbe92252afa13f3852775c3e68599df7741e90cb7 in / 
# Wed, 14 Jul 2021 00:06:28 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 14 Jul 2021 00:06:28 GMT
CMD ["couchbase-server"]
# Wed, 14 Jul 2021 00:06:29 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Wed, 14 Jul 2021 00:06:29 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:e7ae86ffe2df0787131a4c49ace1b018fd38d62929b007d86bdd1f825e56a852`  
		Last Modified: Tue, 13 Jul 2021 22:31:03 GMT  
		Size: 26.7 MB (26706145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f13c80c516e182839d6e6d6f7bc46ca9d41b722a2b3187d09071f91c78769b0e`  
		Last Modified: Wed, 14 Jul 2021 00:18:37 GMT  
		Size: 7.4 MB (7373539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fec6a0ae3c3d8baa9b4f7ebc733acffb0a42e2e7a0d032ceba2a7f11936f3e3`  
		Last Modified: Wed, 14 Jul 2021 00:18:32 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab5dee3151e8e70190b53a3a3bbc9200259eb35893c26bfebc01c368a6ace06f`  
		Last Modified: Wed, 14 Jul 2021 00:22:39 GMT  
		Size: 2.0 KB (1972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaf6bdafc3bdaf035f1502520973205992dd71544a8e8bf663761e6d90796dc4`  
		Last Modified: Wed, 14 Jul 2021 00:23:34 GMT  
		Size: 467.3 MB (467306581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c3098c61a8491b51e575498cdf6045b7324bd6c78629edb107d3bc845dabba1`  
		Last Modified: Wed, 14 Jul 2021 00:22:39 GMT  
		Size: 190.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0773ef54b733514ca4ebbc3dcbb80e174ac2fc8e8a2f0321bfc839f27047ae8`  
		Last Modified: Wed, 14 Jul 2021 00:22:39 GMT  
		Size: 480.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da37c896a9bb745bff6201e8d9623dfb15618f306dd094d8e1235004c6b1c545`  
		Last Modified: Wed, 14 Jul 2021 00:22:36 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f091525ff6ca545246cc550e088b4da9e978f179f87a21f9232fee45a563e40b`  
		Last Modified: Wed, 14 Jul 2021 00:22:36 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cfc56ee30aeb0a400dc9a1cc3f6a7303bc24da14ebd14e6e786d2c6b3616cc5`  
		Last Modified: Wed, 14 Jul 2021 00:22:36 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0478a678346ea57fb828351fa802dcbfe44b0490394f261354dbb4f95ae06b58`  
		Last Modified: Wed, 14 Jul 2021 00:22:37 GMT  
		Size: 118.2 KB (118190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9d175ba0da7224c3f91c98e765a46767a7ed9297a898b36c253b52928187b73`  
		Last Modified: Wed, 14 Jul 2021 00:22:36 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchbase:enterprise-6.6.0`

```console
$ docker pull couchbase@sha256:c63523e408d7fd3afc9471400ac47f738a895ca592daf543293393d5eccb1282
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `couchbase:enterprise-6.6.0` - linux; amd64

```console
$ docker pull couchbase@sha256:14f998618570e30d08415634308be14529f8e934b51ef1c561a238201a75f096
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **527.3 MB (527322653 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5065e29d7a87e48e3b2538d0f535a6b03886c5f9ccb09f6dfffd6b9163573f7d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Tue, 13 Jul 2021 22:29:15 GMT
ADD file:7274ece1917848683250bbeda9eacf6eb7510481cbaa177880e3a60b4133e35b in / 
# Tue, 13 Jul 2021 22:29:15 GMT
CMD ["bash"]
# Tue, 13 Jul 2021 23:56:52 GMT
LABEL maintainer=docker@couchbase.com
# Tue, 13 Jul 2021 23:57:29 GMT
RUN set -x &&     apt-get update &&     apt-get install -yq runit wget chrpath tzdata man     lsof lshw sysstat net-tools numactl bzip2 &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Tue, 13 Jul 2021 23:57:32 GMT
RUN if [ ! -x /usr/sbin/runsvdir-start ]; then         cp -a /etc/runit/2 /usr/sbin/runsvdir-start;     fi
# Tue, 13 Jul 2021 23:57:32 GMT
ARG CB_VERSION=6.6.0
# Tue, 13 Jul 2021 23:57:32 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0
# Wed, 14 Jul 2021 00:03:11 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_6.6.0-ubuntu18.04_amd64.deb
# Wed, 14 Jul 2021 00:03:11 GMT
ARG CB_SHA256=8e7fd5434537094be2fbdfedf3ab5005f0f7d5b9d0578f59ce540b424215b728
# Wed, 14 Jul 2021 00:03:12 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Wed, 14 Jul 2021 00:03:14 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.0-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=8e7fd5434537094be2fbdfedf3ab5005f0f7d5b9d0578f59ce540b424215b728 CB_VERSION=6.6.0
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Wed, 14 Jul 2021 00:04:23 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.0-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=8e7fd5434537094be2fbdfedf3ab5005f0f7d5b9d0578f59ce540b424215b728 CB_VERSION=6.6.0
RUN set -x &&     export INSTALL_DONT_START_SERVER=1 &&     wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE &&     echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - &&     apt-get update &&     apt-get install -y ./$CB_PACKAGE &&     rm -f ./$CB_PACKAGE &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Wed, 14 Jul 2021 00:04:29 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.0-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=8e7fd5434537094be2fbdfedf3ab5005f0f7d5b9d0578f59ce540b424215b728 CB_VERSION=6.6.0
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Wed, 14 Jul 2021 00:04:29 GMT
COPY file:d6a307209223b2df102f46f07fd186e09fac7114db2c965bb54097d3b4d3b989 in /etc/service/couchbase-server/run 
# Wed, 14 Jul 2021 00:04:31 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.0-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=8e7fd5434537094be2fbdfedf3ab5005f0f7d5b9d0578f59ce540b424215b728 CB_VERSION=6.6.0
RUN mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Wed, 14 Jul 2021 00:04:32 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Wed, 14 Jul 2021 00:04:34 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.0-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=8e7fd5434537094be2fbdfedf3ab5005f0f7d5b9d0578f59ce540b424215b728 CB_VERSION=6.6.0
RUN ln -s dummy.sh /usr/local/bin/iptables-save &&     ln -s dummy.sh /usr/local/bin/lvdisplay &&     ln -s dummy.sh /usr/local/bin/vgdisplay &&     ln -s dummy.sh /usr/local/bin/pvdisplay
# Wed, 14 Jul 2021 00:04:36 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.0-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=8e7fd5434537094be2fbdfedf3ab5005f0f7d5b9d0578f59ce540b424215b728 CB_VERSION=6.6.0
RUN chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl
# Wed, 14 Jul 2021 00:04:36 GMT
COPY file:d816a67f62bfba76d2812cefbe92252afa13f3852775c3e68599df7741e90cb7 in / 
# Wed, 14 Jul 2021 00:04:36 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 14 Jul 2021 00:04:37 GMT
CMD ["couchbase-server"]
# Wed, 14 Jul 2021 00:04:37 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Wed, 14 Jul 2021 00:04:37 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:e7ae86ffe2df0787131a4c49ace1b018fd38d62929b007d86bdd1f825e56a852`  
		Last Modified: Tue, 13 Jul 2021 22:31:03 GMT  
		Size: 26.7 MB (26706145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f13c80c516e182839d6e6d6f7bc46ca9d41b722a2b3187d09071f91c78769b0e`  
		Last Modified: Wed, 14 Jul 2021 00:18:37 GMT  
		Size: 7.4 MB (7373539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fec6a0ae3c3d8baa9b4f7ebc733acffb0a42e2e7a0d032ceba2a7f11936f3e3`  
		Last Modified: Wed, 14 Jul 2021 00:18:32 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:beff1fabd9cf83626d6441f27e38595e1a37e842ba062f25b094dae598fec8e9`  
		Last Modified: Wed, 14 Jul 2021 00:21:29 GMT  
		Size: 2.0 KB (1968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91f0c28648ffc3d7438a50edd26aa3e046b56497a8eff6cc962f7fb9b34893f0`  
		Last Modified: Wed, 14 Jul 2021 00:22:23 GMT  
		Size: 493.1 MB (493120282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d71d047bc6c5881d40b2338128dfe1f70c8c2a84cc05858bcdd7f1c528be6278`  
		Last Modified: Wed, 14 Jul 2021 00:21:29 GMT  
		Size: 190.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2c02e2f983881fdc342643c2a1960010fa65d78f4b5ab41371728dac97bd9db`  
		Last Modified: Wed, 14 Jul 2021 00:21:29 GMT  
		Size: 479.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b58b74c5013e779d82b12a7bebd5a6684161c2c54aed4fc5ab1d89e36975011`  
		Last Modified: Wed, 14 Jul 2021 00:21:26 GMT  
		Size: 280.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b1f6a851d29532a08ec1b8ae8f218a6b884e6e1c0894700ea8d67d1d8521e82`  
		Last Modified: Wed, 14 Jul 2021 00:21:26 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbfec9fa5f7320af7b34ea68e7a091df7773884c8491b01ce13cd74623adf692`  
		Last Modified: Wed, 14 Jul 2021 00:21:26 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a26f4d875683ac9ae45a8f9141852ec801ec35844858650109df21a64313c1b7`  
		Last Modified: Wed, 14 Jul 2021 00:21:26 GMT  
		Size: 118.2 KB (118192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f37c9aa96adac79e5a02cdd8ab85bc2f4537d7c1ce3e9e1a922a9851f388e9c`  
		Last Modified: Wed, 14 Jul 2021 00:21:26 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchbase:enterprise-6.6.1`

```console
$ docker pull couchbase@sha256:af6148a17dfdbfb30c187e7247fa5bff41f6a3dfe00b21e4fcf0a393d1e3cb3a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `couchbase:enterprise-6.6.1` - linux; amd64

```console
$ docker pull couchbase@sha256:b71d901bea6d20aeaf635993d07a5763c08c01500c0f257d80dee19a1b02242b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **528.5 MB (528524928 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:17fa76aff6698eef0b73a35d09436f4cd1af6964ed3a0456b045170d3d054ecb`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Tue, 13 Jul 2021 22:29:15 GMT
ADD file:7274ece1917848683250bbeda9eacf6eb7510481cbaa177880e3a60b4133e35b in / 
# Tue, 13 Jul 2021 22:29:15 GMT
CMD ["bash"]
# Tue, 13 Jul 2021 23:56:52 GMT
LABEL maintainer=docker@couchbase.com
# Tue, 13 Jul 2021 23:57:29 GMT
RUN set -x &&     apt-get update &&     apt-get install -yq runit wget chrpath tzdata man     lsof lshw sysstat net-tools numactl bzip2 &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Tue, 13 Jul 2021 23:57:32 GMT
RUN if [ ! -x /usr/sbin/runsvdir-start ]; then         cp -a /etc/runit/2 /usr/sbin/runsvdir-start;     fi
# Wed, 14 Jul 2021 00:01:14 GMT
ARG CB_VERSION=6.6.1
# Wed, 14 Jul 2021 00:01:15 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.1
# Wed, 14 Jul 2021 00:01:15 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_6.6.1-ubuntu18.04_amd64.deb
# Wed, 14 Jul 2021 00:01:15 GMT
ARG CB_SHA256=4bd8210458905a5801e98bda0663d1214f6743465843f49ef9a52212636b5e89
# Wed, 14 Jul 2021 00:01:16 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Wed, 14 Jul 2021 00:01:17 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.1-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.1 CB_SHA256=4bd8210458905a5801e98bda0663d1214f6743465843f49ef9a52212636b5e89 CB_VERSION=6.6.1
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Wed, 14 Jul 2021 00:02:39 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.1-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.1 CB_SHA256=4bd8210458905a5801e98bda0663d1214f6743465843f49ef9a52212636b5e89 CB_VERSION=6.6.1
RUN set -x &&     export INSTALL_DONT_START_SERVER=1 &&     wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE &&     echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - &&     apt-get update &&     apt-get install -y ./$CB_PACKAGE &&     rm -f ./$CB_PACKAGE &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Wed, 14 Jul 2021 00:02:44 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.1-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.1 CB_SHA256=4bd8210458905a5801e98bda0663d1214f6743465843f49ef9a52212636b5e89 CB_VERSION=6.6.1
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Wed, 14 Jul 2021 00:02:45 GMT
COPY file:d6a307209223b2df102f46f07fd186e09fac7114db2c965bb54097d3b4d3b989 in /etc/service/couchbase-server/run 
# Wed, 14 Jul 2021 00:02:46 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.1-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.1 CB_SHA256=4bd8210458905a5801e98bda0663d1214f6743465843f49ef9a52212636b5e89 CB_VERSION=6.6.1
RUN mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Wed, 14 Jul 2021 00:02:47 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Wed, 14 Jul 2021 00:02:49 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.1-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.1 CB_SHA256=4bd8210458905a5801e98bda0663d1214f6743465843f49ef9a52212636b5e89 CB_VERSION=6.6.1
RUN ln -s dummy.sh /usr/local/bin/iptables-save &&     ln -s dummy.sh /usr/local/bin/lvdisplay &&     ln -s dummy.sh /usr/local/bin/vgdisplay &&     ln -s dummy.sh /usr/local/bin/pvdisplay
# Wed, 14 Jul 2021 00:02:51 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.1-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.1 CB_SHA256=4bd8210458905a5801e98bda0663d1214f6743465843f49ef9a52212636b5e89 CB_VERSION=6.6.1
RUN chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl
# Wed, 14 Jul 2021 00:02:51 GMT
COPY file:d816a67f62bfba76d2812cefbe92252afa13f3852775c3e68599df7741e90cb7 in / 
# Wed, 14 Jul 2021 00:02:52 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 14 Jul 2021 00:02:52 GMT
CMD ["couchbase-server"]
# Wed, 14 Jul 2021 00:02:52 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Wed, 14 Jul 2021 00:02:53 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:e7ae86ffe2df0787131a4c49ace1b018fd38d62929b007d86bdd1f825e56a852`  
		Last Modified: Tue, 13 Jul 2021 22:31:03 GMT  
		Size: 26.7 MB (26706145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f13c80c516e182839d6e6d6f7bc46ca9d41b722a2b3187d09071f91c78769b0e`  
		Last Modified: Wed, 14 Jul 2021 00:18:37 GMT  
		Size: 7.4 MB (7373539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fec6a0ae3c3d8baa9b4f7ebc733acffb0a42e2e7a0d032ceba2a7f11936f3e3`  
		Last Modified: Wed, 14 Jul 2021 00:18:32 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9286972580e33b72ccf9c3fce3fe227c9d6625574bf6787bf2d489723c906538`  
		Last Modified: Wed, 14 Jul 2021 00:20:19 GMT  
		Size: 2.0 KB (1963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1687b69a86447feeab1eb31298e4fb3b13c191ee68e30fa0a097164b9580893`  
		Last Modified: Wed, 14 Jul 2021 00:21:14 GMT  
		Size: 494.3 MB (494322565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1ba863fe24827037c66b30eddf1f16af20ea3e786b84e6e7850f1131b7ffd02`  
		Last Modified: Wed, 14 Jul 2021 00:20:19 GMT  
		Size: 190.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e747f934c61fd217d3d09b8b8b6213d8cf601b008e3c9033ec8e2ccfb56fc931`  
		Last Modified: Wed, 14 Jul 2021 00:20:19 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6342fbc05e2e7d8a699270d543c3e0da4bb5f587f8c43a6f491424bcb60e9304`  
		Last Modified: Wed, 14 Jul 2021 00:20:17 GMT  
		Size: 282.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a1f233d6e7725d9fa0bf5328e7c8b80e7efc71112be7507cb7a7bc06149f1b3`  
		Last Modified: Wed, 14 Jul 2021 00:20:17 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8081b1aafdb161c6c8f0021ee61ac6bfe1371824658432201dc2a3e59aa3a26b`  
		Last Modified: Wed, 14 Jul 2021 00:20:17 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1727ebe294a93614fb6a2674332ac66d4ac849581f75da275adb6abefb6b2746`  
		Last Modified: Wed, 14 Jul 2021 00:20:17 GMT  
		Size: 118.2 KB (118190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a64e65e5fc46d51deb08bee39f530bc2e4029b8b543da18e751fed8b428811aa`  
		Last Modified: Wed, 14 Jul 2021 00:20:17 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchbase:enterprise-6.6.2`

```console
$ docker pull couchbase@sha256:f81f332a99b86514042eaf1194603d65c37404c2686d1ae3ec3855056247be5c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `couchbase:enterprise-6.6.2` - linux; amd64

```console
$ docker pull couchbase@sha256:512ce0c9f998819d6e59f576cb24bc258775dfcfd52eee616427a5dec207eac3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **533.2 MB (533221032 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:00cc1f1af822aeda54b4e7859f621aaab1b8ac5a0eb0a97e0e89fdbdd7a005b1`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Tue, 13 Jul 2021 22:29:34 GMT
ADD file:5c3d9d2597e01d1cee8513ff0e1344e7791e6f582be2cbd1d5777dd204780f1c in / 
# Tue, 13 Jul 2021 22:29:34 GMT
CMD ["bash"]
# Tue, 13 Jul 2021 23:50:49 GMT
LABEL maintainer=docker@couchbase.com
# Tue, 13 Jul 2021 23:55:02 GMT
RUN set -x &&     apt-get update &&     apt-get install -yq runit wget chrpath tzdata     lsof lshw sysstat net-tools numactl bzip2 &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Tue, 13 Jul 2021 23:55:04 GMT
RUN if [ ! -x /usr/sbin/runsvdir-start ]; then         cp -a /etc/runit/2 /usr/sbin/runsvdir-start;     fi
# Tue, 13 Jul 2021 23:55:05 GMT
ARG CB_VERSION=6.6.2
# Tue, 13 Jul 2021 23:55:05 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.2
# Tue, 13 Jul 2021 23:55:06 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_6.6.2-ubuntu20.04_amd64.deb
# Tue, 13 Jul 2021 23:55:06 GMT
ARG CB_SHA256=41c033e6c1e98b0844a5cb5768e3769e7012d8374a6bd235c86e10db33b17afc
# Tue, 13 Jul 2021 23:55:06 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Tue, 13 Jul 2021 23:55:08 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.2-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.2 CB_SHA256=41c033e6c1e98b0844a5cb5768e3769e7012d8374a6bd235c86e10db33b17afc CB_VERSION=6.6.2
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Tue, 13 Jul 2021 23:56:27 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.2-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.2 CB_SHA256=41c033e6c1e98b0844a5cb5768e3769e7012d8374a6bd235c86e10db33b17afc CB_VERSION=6.6.2
RUN set -x &&     export INSTALL_DONT_START_SERVER=1 &&     wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE &&     echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - &&     apt-get update &&     apt-get install -y ./$CB_PACKAGE &&     rm -f ./$CB_PACKAGE &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Tue, 13 Jul 2021 23:56:32 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.2-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.2 CB_SHA256=41c033e6c1e98b0844a5cb5768e3769e7012d8374a6bd235c86e10db33b17afc CB_VERSION=6.6.2
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Tue, 13 Jul 2021 23:56:32 GMT
COPY file:d6a307209223b2df102f46f07fd186e09fac7114db2c965bb54097d3b4d3b989 in /etc/service/couchbase-server/run 
# Tue, 13 Jul 2021 23:56:34 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.2-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.2 CB_SHA256=41c033e6c1e98b0844a5cb5768e3769e7012d8374a6bd235c86e10db33b17afc CB_VERSION=6.6.2
RUN mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Tue, 13 Jul 2021 23:56:34 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Tue, 13 Jul 2021 23:56:36 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.2-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.2 CB_SHA256=41c033e6c1e98b0844a5cb5768e3769e7012d8374a6bd235c86e10db33b17afc CB_VERSION=6.6.2
RUN ln -s dummy.sh /usr/local/bin/iptables-save &&     ln -s dummy.sh /usr/local/bin/lvdisplay &&     ln -s dummy.sh /usr/local/bin/vgdisplay &&     ln -s dummy.sh /usr/local/bin/pvdisplay
# Tue, 13 Jul 2021 23:56:37 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.2-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.2 CB_SHA256=41c033e6c1e98b0844a5cb5768e3769e7012d8374a6bd235c86e10db33b17afc CB_VERSION=6.6.2
RUN chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl
# Tue, 13 Jul 2021 23:56:37 GMT
COPY file:d816a67f62bfba76d2812cefbe92252afa13f3852775c3e68599df7741e90cb7 in / 
# Tue, 13 Jul 2021 23:56:37 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 13 Jul 2021 23:56:38 GMT
CMD ["couchbase-server"]
# Tue, 13 Jul 2021 23:56:38 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Tue, 13 Jul 2021 23:56:38 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:a31c7b29f4ad2bd946738970f040825704a523ded1b9d6f9c7c7cafc6ab731df`  
		Last Modified: Tue, 13 Jul 2021 22:31:20 GMT  
		Size: 28.6 MB (28565863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f926d574d0b4b28f1f76deaa9aff956ebd84fca4c28ae00cb2342e321657edf3`  
		Last Modified: Wed, 14 Jul 2021 00:17:16 GMT  
		Size: 6.3 MB (6272606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ad3c9266985cc6da988565a76f19e617642668ced44547bb0e3b11af0301a00`  
		Last Modified: Wed, 14 Jul 2021 00:17:13 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23d163e5c68bca024eec49616679790ec8960fcde31526d8e29b5b1c38a9e872`  
		Last Modified: Wed, 14 Jul 2021 00:17:12 GMT  
		Size: 1.8 KB (1830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef2f5d79c085803411789e047e9ac102f5b17b68e9cffdcf72c199cabae6f6c0`  
		Last Modified: Wed, 14 Jul 2021 00:18:07 GMT  
		Size: 498.3 MB (498252316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c1d5eca3d063ae7effcc02e063c12fba349a3397808320570881e1cd400c468`  
		Last Modified: Wed, 14 Jul 2021 00:17:11 GMT  
		Size: 191.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63d346d7d3d4c52f9398df214716d61690c11261de8d80fdf0667a891d03f975`  
		Last Modified: Wed, 14 Jul 2021 00:17:11 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d45857737224785a1eab0c64e68eca963845fc8c29ba24f0f31cca91f9f73a4c`  
		Last Modified: Wed, 14 Jul 2021 00:17:09 GMT  
		Size: 281.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cce5e9dc1794cbdc1c5c738f15081bcfd141e67f3bea239ac3c2550551d5e76`  
		Last Modified: Wed, 14 Jul 2021 00:17:10 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:823f3f5bd72eb157355adc6d50c5df0e37548878cbad7b1ce94a902b039d5c61`  
		Last Modified: Wed, 14 Jul 2021 00:17:09 GMT  
		Size: 216.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ded2b29872fe46b0fdbeae64bbbbfdda02d84267a7b46538e6b749ce296fd3ce`  
		Last Modified: Wed, 14 Jul 2021 00:17:09 GMT  
		Size: 125.9 KB (125895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79733ad7ecdd3e0dc809f52676d3c3468febbb8306ca93d20ff073847c2f50ea`  
		Last Modified: Wed, 14 Jul 2021 00:17:09 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchbase:enterprise-7.0.0-beta`

```console
$ docker pull couchbase@sha256:d1688941d858881861c60fb674f37ec439f098035f00d682710ee0d06ef18799
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `couchbase:enterprise-7.0.0-beta` - linux; amd64

```console
$ docker pull couchbase@sha256:7fc24a15658a601982c5e1832db2189ea949aabbe7b86e2e4b37c2510583a047
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **628.1 MB (628096335 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b754d7f1774a0d94e1402b2a26d3cdf7cc241a468e6b53d7d6c3a2191cf094f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Tue, 13 Jul 2021 22:29:34 GMT
ADD file:5c3d9d2597e01d1cee8513ff0e1344e7791e6f582be2cbd1d5777dd204780f1c in / 
# Tue, 13 Jul 2021 22:29:34 GMT
CMD ["bash"]
# Tue, 13 Jul 2021 23:50:49 GMT
LABEL maintainer=docker@couchbase.com
# Tue, 13 Jul 2021 23:51:15 GMT
RUN set -x &&     apt-get update &&     apt-get install -yq runit wget chrpath tzdata man     lsof lshw sysstat net-tools numactl bzip2 &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Tue, 13 Jul 2021 23:51:16 GMT
RUN if [ ! -x /usr/sbin/runsvdir-start ]; then         cp -a /etc/runit/2 /usr/sbin/runsvdir-start;     fi
# Tue, 13 Jul 2021 23:51:16 GMT
ARG CB_VERSION=7.0.0-beta
# Tue, 13 Jul 2021 23:51:17 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.0-beta
# Tue, 13 Jul 2021 23:51:17 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_7.0.0-beta-ubuntu20.04_amd64.deb
# Tue, 13 Jul 2021 23:51:17 GMT
ARG CB_SHA256=e24be4f765eafbfbfdd5f7eddb780006084e3bd01cbcb3d3880dd9be48b955f6
# Tue, 13 Jul 2021 23:51:17 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Tue, 13 Jul 2021 23:51:18 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.0-beta-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.0-beta CB_SHA256=e24be4f765eafbfbfdd5f7eddb780006084e3bd01cbcb3d3880dd9be48b955f6 CB_VERSION=7.0.0-beta
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Tue, 13 Jul 2021 23:52:43 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.0-beta-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.0-beta CB_SHA256=e24be4f765eafbfbfdd5f7eddb780006084e3bd01cbcb3d3880dd9be48b955f6 CB_VERSION=7.0.0-beta
RUN set -x &&     export INSTALL_DONT_START_SERVER=1 &&     wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE &&     echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - &&     apt-get update &&     apt-get install -y ./$CB_PACKAGE &&     rm -f ./$CB_PACKAGE &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Tue, 13 Jul 2021 23:52:50 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.0-beta-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.0-beta CB_SHA256=e24be4f765eafbfbfdd5f7eddb780006084e3bd01cbcb3d3880dd9be48b955f6 CB_VERSION=7.0.0-beta
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Tue, 13 Jul 2021 23:52:50 GMT
COPY file:d6a307209223b2df102f46f07fd186e09fac7114db2c965bb54097d3b4d3b989 in /etc/service/couchbase-server/run 
# Tue, 13 Jul 2021 23:52:52 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.0-beta-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.0-beta CB_SHA256=e24be4f765eafbfbfdd5f7eddb780006084e3bd01cbcb3d3880dd9be48b955f6 CB_VERSION=7.0.0-beta
RUN mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Tue, 13 Jul 2021 23:52:53 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Tue, 13 Jul 2021 23:52:55 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.0-beta-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.0-beta CB_SHA256=e24be4f765eafbfbfdd5f7eddb780006084e3bd01cbcb3d3880dd9be48b955f6 CB_VERSION=7.0.0-beta
RUN ln -s dummy.sh /usr/local/bin/iptables-save &&     ln -s dummy.sh /usr/local/bin/lvdisplay &&     ln -s dummy.sh /usr/local/bin/vgdisplay &&     ln -s dummy.sh /usr/local/bin/pvdisplay
# Tue, 13 Jul 2021 23:52:57 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.0-beta-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.0-beta CB_SHA256=e24be4f765eafbfbfdd5f7eddb780006084e3bd01cbcb3d3880dd9be48b955f6 CB_VERSION=7.0.0-beta
RUN chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl
# Tue, 13 Jul 2021 23:52:57 GMT
COPY file:d816a67f62bfba76d2812cefbe92252afa13f3852775c3e68599df7741e90cb7 in / 
# Tue, 13 Jul 2021 23:52:58 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 13 Jul 2021 23:52:58 GMT
CMD ["couchbase-server"]
# Tue, 13 Jul 2021 23:52:58 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Tue, 13 Jul 2021 23:52:59 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:a31c7b29f4ad2bd946738970f040825704a523ded1b9d6f9c7c7cafc6ab731df`  
		Last Modified: Tue, 13 Jul 2021 22:31:20 GMT  
		Size: 28.6 MB (28565863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27d820bb660a9b14c611213779ee0deee8781268242fd7d51bd43a6e638f6722`  
		Last Modified: Wed, 14 Jul 2021 00:14:56 GMT  
		Size: 8.3 MB (8286840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db40d5a53531bbb33b0d3feb0be6f6fd03a142fba87ac62d5487adf1928a6673`  
		Last Modified: Wed, 14 Jul 2021 00:14:50 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:875bb808e008cdde9ba4f2b7d35760e77f6a6a2e2db82c5e41e877fedd410d7d`  
		Last Modified: Wed, 14 Jul 2021 00:14:51 GMT  
		Size: 1.8 KB (1830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:855824ba8946788de53fb20491f40faa224f2e5074bf3e8c3008c33fb81ff555`  
		Last Modified: Wed, 14 Jul 2021 00:15:57 GMT  
		Size: 591.1 MB (591113393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfc2a6dcc68d13067288c0300be7915f87fa22d599b8fb8a67bc3f2e194bf63e`  
		Last Modified: Wed, 14 Jul 2021 00:14:50 GMT  
		Size: 191.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c0d1e8645eda88311f73a402d5fc3541f22644726fc24084ba70ee986c42cbe`  
		Last Modified: Wed, 14 Jul 2021 00:14:50 GMT  
		Size: 472.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d9804d533cfe6215e476fd14d430e059f3998b5c7197b74b47dcb9da80b950f`  
		Last Modified: Wed, 14 Jul 2021 00:14:48 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10603d7e2729cb2b4acf00f32356c7545eac6748343669324c164bfc684e85c6`  
		Last Modified: Wed, 14 Jul 2021 00:14:48 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f959ad6bef002fb82a015a17c8f4e7a885ccc2bc9868147291a239165c43d39`  
		Last Modified: Wed, 14 Jul 2021 00:14:48 GMT  
		Size: 217.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21d42cd2ad5a7005696a4d7e2c1f84eafc57294b5cd3d4ee7a86cb41d4ed09fb`  
		Last Modified: Wed, 14 Jul 2021 00:14:48 GMT  
		Size: 125.9 KB (125893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0037a926b052a91e2453be04f4ae22cdfc4563cbc7536cb2d2bf0273afb8681`  
		Last Modified: Wed, 14 Jul 2021 00:14:48 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchbase:latest`

```console
$ docker pull couchbase@sha256:f81f332a99b86514042eaf1194603d65c37404c2686d1ae3ec3855056247be5c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `couchbase:latest` - linux; amd64

```console
$ docker pull couchbase@sha256:512ce0c9f998819d6e59f576cb24bc258775dfcfd52eee616427a5dec207eac3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **533.2 MB (533221032 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:00cc1f1af822aeda54b4e7859f621aaab1b8ac5a0eb0a97e0e89fdbdd7a005b1`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Tue, 13 Jul 2021 22:29:34 GMT
ADD file:5c3d9d2597e01d1cee8513ff0e1344e7791e6f582be2cbd1d5777dd204780f1c in / 
# Tue, 13 Jul 2021 22:29:34 GMT
CMD ["bash"]
# Tue, 13 Jul 2021 23:50:49 GMT
LABEL maintainer=docker@couchbase.com
# Tue, 13 Jul 2021 23:55:02 GMT
RUN set -x &&     apt-get update &&     apt-get install -yq runit wget chrpath tzdata     lsof lshw sysstat net-tools numactl bzip2 &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Tue, 13 Jul 2021 23:55:04 GMT
RUN if [ ! -x /usr/sbin/runsvdir-start ]; then         cp -a /etc/runit/2 /usr/sbin/runsvdir-start;     fi
# Tue, 13 Jul 2021 23:55:05 GMT
ARG CB_VERSION=6.6.2
# Tue, 13 Jul 2021 23:55:05 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.2
# Tue, 13 Jul 2021 23:55:06 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_6.6.2-ubuntu20.04_amd64.deb
# Tue, 13 Jul 2021 23:55:06 GMT
ARG CB_SHA256=41c033e6c1e98b0844a5cb5768e3769e7012d8374a6bd235c86e10db33b17afc
# Tue, 13 Jul 2021 23:55:06 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Tue, 13 Jul 2021 23:55:08 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.2-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.2 CB_SHA256=41c033e6c1e98b0844a5cb5768e3769e7012d8374a6bd235c86e10db33b17afc CB_VERSION=6.6.2
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Tue, 13 Jul 2021 23:56:27 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.2-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.2 CB_SHA256=41c033e6c1e98b0844a5cb5768e3769e7012d8374a6bd235c86e10db33b17afc CB_VERSION=6.6.2
RUN set -x &&     export INSTALL_DONT_START_SERVER=1 &&     wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE &&     echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - &&     apt-get update &&     apt-get install -y ./$CB_PACKAGE &&     rm -f ./$CB_PACKAGE &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Tue, 13 Jul 2021 23:56:32 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.2-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.2 CB_SHA256=41c033e6c1e98b0844a5cb5768e3769e7012d8374a6bd235c86e10db33b17afc CB_VERSION=6.6.2
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Tue, 13 Jul 2021 23:56:32 GMT
COPY file:d6a307209223b2df102f46f07fd186e09fac7114db2c965bb54097d3b4d3b989 in /etc/service/couchbase-server/run 
# Tue, 13 Jul 2021 23:56:34 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.2-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.2 CB_SHA256=41c033e6c1e98b0844a5cb5768e3769e7012d8374a6bd235c86e10db33b17afc CB_VERSION=6.6.2
RUN mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Tue, 13 Jul 2021 23:56:34 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Tue, 13 Jul 2021 23:56:36 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.2-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.2 CB_SHA256=41c033e6c1e98b0844a5cb5768e3769e7012d8374a6bd235c86e10db33b17afc CB_VERSION=6.6.2
RUN ln -s dummy.sh /usr/local/bin/iptables-save &&     ln -s dummy.sh /usr/local/bin/lvdisplay &&     ln -s dummy.sh /usr/local/bin/vgdisplay &&     ln -s dummy.sh /usr/local/bin/pvdisplay
# Tue, 13 Jul 2021 23:56:37 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.2-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.2 CB_SHA256=41c033e6c1e98b0844a5cb5768e3769e7012d8374a6bd235c86e10db33b17afc CB_VERSION=6.6.2
RUN chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl
# Tue, 13 Jul 2021 23:56:37 GMT
COPY file:d816a67f62bfba76d2812cefbe92252afa13f3852775c3e68599df7741e90cb7 in / 
# Tue, 13 Jul 2021 23:56:37 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 13 Jul 2021 23:56:38 GMT
CMD ["couchbase-server"]
# Tue, 13 Jul 2021 23:56:38 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Tue, 13 Jul 2021 23:56:38 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:a31c7b29f4ad2bd946738970f040825704a523ded1b9d6f9c7c7cafc6ab731df`  
		Last Modified: Tue, 13 Jul 2021 22:31:20 GMT  
		Size: 28.6 MB (28565863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f926d574d0b4b28f1f76deaa9aff956ebd84fca4c28ae00cb2342e321657edf3`  
		Last Modified: Wed, 14 Jul 2021 00:17:16 GMT  
		Size: 6.3 MB (6272606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ad3c9266985cc6da988565a76f19e617642668ced44547bb0e3b11af0301a00`  
		Last Modified: Wed, 14 Jul 2021 00:17:13 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23d163e5c68bca024eec49616679790ec8960fcde31526d8e29b5b1c38a9e872`  
		Last Modified: Wed, 14 Jul 2021 00:17:12 GMT  
		Size: 1.8 KB (1830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef2f5d79c085803411789e047e9ac102f5b17b68e9cffdcf72c199cabae6f6c0`  
		Last Modified: Wed, 14 Jul 2021 00:18:07 GMT  
		Size: 498.3 MB (498252316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c1d5eca3d063ae7effcc02e063c12fba349a3397808320570881e1cd400c468`  
		Last Modified: Wed, 14 Jul 2021 00:17:11 GMT  
		Size: 191.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63d346d7d3d4c52f9398df214716d61690c11261de8d80fdf0667a891d03f975`  
		Last Modified: Wed, 14 Jul 2021 00:17:11 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d45857737224785a1eab0c64e68eca963845fc8c29ba24f0f31cca91f9f73a4c`  
		Last Modified: Wed, 14 Jul 2021 00:17:09 GMT  
		Size: 281.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cce5e9dc1794cbdc1c5c738f15081bcfd141e67f3bea239ac3c2550551d5e76`  
		Last Modified: Wed, 14 Jul 2021 00:17:10 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:823f3f5bd72eb157355adc6d50c5df0e37548878cbad7b1ce94a902b039d5c61`  
		Last Modified: Wed, 14 Jul 2021 00:17:09 GMT  
		Size: 216.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ded2b29872fe46b0fdbeae64bbbbfdda02d84267a7b46538e6b749ce296fd3ce`  
		Last Modified: Wed, 14 Jul 2021 00:17:09 GMT  
		Size: 125.9 KB (125895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79733ad7ecdd3e0dc809f52676d3c3468febbb8306ca93d20ff073847c2f50ea`  
		Last Modified: Wed, 14 Jul 2021 00:17:09 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
