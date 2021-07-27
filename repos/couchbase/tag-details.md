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
$ docker pull couchbase@sha256:59357050ffc9245a673bb94cf7f473afa8793efe831f8eb43b34cd6c864cf0b1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `couchbase:6.0.4` - linux; amd64

```console
$ docker pull couchbase@sha256:2072d81f3b5f827d376965a1cea84f0bffa52384003b6e4f8165c4374341d35f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **467.2 MB (467176565 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92694534bfffd286b6c35bbc4783b3a87fbb8e902d6b070561842970528c5a3d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Mon, 26 Jul 2021 21:21:30 GMT
ADD file:e729fb032bd2f7cde20fb343da0cd358447e8b23028422c123944e8d0be660fa in / 
# Mon, 26 Jul 2021 21:21:31 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 22:21:49 GMT
LABEL maintainer=docker@couchbase.com
# Mon, 26 Jul 2021 22:23:55 GMT
RUN set -x &&     apt-get update &&     apt-get install -yq runit wget chrpath tzdata man     lsof lshw sysstat net-tools numactl python-httplib2 &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Mon, 26 Jul 2021 22:23:56 GMT
RUN if [ ! -x /usr/sbin/runsvdir-start ]; then         cp -a /etc/runit/2 /usr/sbin/runsvdir-start;     fi
# Mon, 26 Jul 2021 22:30:52 GMT
ARG CB_VERSION=6.0.4
# Mon, 26 Jul 2021 22:30:52 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.4
# Mon, 26 Jul 2021 22:30:52 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_6.0.4-ubuntu18.04_amd64.deb
# Mon, 26 Jul 2021 22:30:52 GMT
ARG CB_SHA256=7dbe8dd074f9cabea69468ea488f9ffc19c04dab8fc2e98c937fa32704982aff
# Mon, 26 Jul 2021 22:30:53 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Mon, 26 Jul 2021 22:30:53 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.4-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.4 CB_SHA256=7dbe8dd074f9cabea69468ea488f9ffc19c04dab8fc2e98c937fa32704982aff CB_VERSION=6.0.4
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Mon, 26 Jul 2021 22:31:51 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.4-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.4 CB_SHA256=7dbe8dd074f9cabea69468ea488f9ffc19c04dab8fc2e98c937fa32704982aff CB_VERSION=6.0.4
RUN set -x &&     export INSTALL_DONT_START_SERVER=1 &&     wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE &&     echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - &&     apt-get update &&     apt-get install -y ./$CB_PACKAGE &&     rm -f ./$CB_PACKAGE &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Mon, 26 Jul 2021 22:31:55 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.4-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.4 CB_SHA256=7dbe8dd074f9cabea69468ea488f9ffc19c04dab8fc2e98c937fa32704982aff CB_VERSION=6.0.4
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Mon, 26 Jul 2021 22:31:55 GMT
COPY file:d6a307209223b2df102f46f07fd186e09fac7114db2c965bb54097d3b4d3b989 in /etc/service/couchbase-server/run 
# Mon, 26 Jul 2021 22:31:56 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.4-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.4 CB_SHA256=7dbe8dd074f9cabea69468ea488f9ffc19c04dab8fc2e98c937fa32704982aff CB_VERSION=6.0.4
RUN mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Mon, 26 Jul 2021 22:31:56 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Mon, 26 Jul 2021 22:31:57 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.4-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.4 CB_SHA256=7dbe8dd074f9cabea69468ea488f9ffc19c04dab8fc2e98c937fa32704982aff CB_VERSION=6.0.4
RUN ln -s dummy.sh /usr/local/bin/iptables-save &&     ln -s dummy.sh /usr/local/bin/lvdisplay &&     ln -s dummy.sh /usr/local/bin/vgdisplay &&     ln -s dummy.sh /usr/local/bin/pvdisplay
# Mon, 26 Jul 2021 22:31:57 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.4-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.4 CB_SHA256=7dbe8dd074f9cabea69468ea488f9ffc19c04dab8fc2e98c937fa32704982aff CB_VERSION=6.0.4
RUN chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl
# Mon, 26 Jul 2021 22:31:58 GMT
COPY file:d816a67f62bfba76d2812cefbe92252afa13f3852775c3e68599df7741e90cb7 in / 
# Mon, 26 Jul 2021 22:31:58 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 26 Jul 2021 22:31:58 GMT
CMD ["couchbase-server"]
# Mon, 26 Jul 2021 22:31:58 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Mon, 26 Jul 2021 22:31:59 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:feac5306138255e28a9862d3f3d29025d0a4d0648855afe1acd6131af07138ac`  
		Last Modified: Mon, 26 Jul 2021 21:22:52 GMT  
		Size: 26.7 MB (26709039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d34675e7dacc0ce319b39b9ea2535f805fa959a52abc54f87cc0a227b97902ca`  
		Last Modified: Mon, 26 Jul 2021 22:42:05 GMT  
		Size: 15.9 MB (15922947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:889c4fafca81882f6937a23d718195844112f8f700b2bbf19b2fed74fb78653f`  
		Last Modified: Mon, 26 Jul 2021 22:42:00 GMT  
		Size: 266.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e574c78a46b41674f9a3261a0f0c68f76abd0af29aa26a2362df38dbcb6d3330`  
		Last Modified: Mon, 26 Jul 2021 22:47:59 GMT  
		Size: 2.0 KB (1968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14eb1008642f2ce7d352468ddc36a6f68069d11a44a253a029bfd0c2d1261c9a`  
		Last Modified: Mon, 26 Jul 2021 22:48:57 GMT  
		Size: 424.4 MB (424414525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f1e38580af5926287c75c797617759c89a0d42fc97c3aa2c0c4fe882e99c2b4`  
		Last Modified: Mon, 26 Jul 2021 22:47:59 GMT  
		Size: 191.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5ed61202651841bbbfe7ba1edd60b48fce04ad1b3aeb89a7d52e3b16a7c537c`  
		Last Modified: Mon, 26 Jul 2021 22:47:59 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:821f18160c226c642f0e30b158c5b1f1dc3c62470b537b709873f6c7a476dd33`  
		Last Modified: Mon, 26 Jul 2021 22:47:57 GMT  
		Size: 279.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bfd07498e11d153cd5fded3de1535089da489d5592399519f7b7290c183d61d`  
		Last Modified: Mon, 26 Jul 2021 22:47:57 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2432caa6ca57817ccc6feb3a8338adabb9a699a72a7c14080667989c2da7dd3`  
		Last Modified: Mon, 26 Jul 2021 22:47:57 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:882cf855fdcaee36f9707e3f2fa50e58a7c933e2b3a5f270152a180d5f3b9f4d`  
		Last Modified: Mon, 26 Jul 2021 22:47:57 GMT  
		Size: 125.6 KB (125559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99d9886ac4a5adeee111246e59b940f93799770342238916bfd704a9111e322f`  
		Last Modified: Mon, 26 Jul 2021 22:47:57 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchbase:6.0.5`

```console
$ docker pull couchbase@sha256:4076897f81ab96c69d27f42accb996d141dbd3a2e9023579841b2361597553c1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `couchbase:6.0.5` - linux; amd64

```console
$ docker pull couchbase@sha256:3a8ee070210558c8a7b4f42d1cef3d608db79a83510927b40eec0423ccbd23d5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **466.1 MB (466124028 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e8db7615f18de1e06f508993a9d442ce0eafcea50895d938de595152a2123121`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Mon, 26 Jul 2021 21:21:30 GMT
ADD file:e729fb032bd2f7cde20fb343da0cd358447e8b23028422c123944e8d0be660fa in / 
# Mon, 26 Jul 2021 21:21:31 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 22:21:49 GMT
LABEL maintainer=docker@couchbase.com
# Mon, 26 Jul 2021 22:23:55 GMT
RUN set -x &&     apt-get update &&     apt-get install -yq runit wget chrpath tzdata man     lsof lshw sysstat net-tools numactl python-httplib2 &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Mon, 26 Jul 2021 22:23:56 GMT
RUN if [ ! -x /usr/sbin/runsvdir-start ]; then         cp -a /etc/runit/2 /usr/sbin/runsvdir-start;     fi
# Mon, 26 Jul 2021 22:23:56 GMT
ARG CB_VERSION=6.0.5
# Mon, 26 Jul 2021 22:23:56 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.5
# Mon, 26 Jul 2021 22:23:56 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_6.0.5-ubuntu18.04_amd64.deb
# Mon, 26 Jul 2021 22:23:57 GMT
ARG CB_SHA256=6b152590867a58d771cffc22774d3cd66c916defcbeeeb339aca8d0a8e6d7f8d
# Mon, 26 Jul 2021 22:23:57 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Mon, 26 Jul 2021 22:23:58 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.5-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.5 CB_SHA256=6b152590867a58d771cffc22774d3cd66c916defcbeeeb339aca8d0a8e6d7f8d CB_VERSION=6.0.5
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Mon, 26 Jul 2021 22:24:57 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.5-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.5 CB_SHA256=6b152590867a58d771cffc22774d3cd66c916defcbeeeb339aca8d0a8e6d7f8d CB_VERSION=6.0.5
RUN set -x &&     export INSTALL_DONT_START_SERVER=1 &&     wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE &&     echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - &&     apt-get update &&     apt-get install -y ./$CB_PACKAGE &&     rm -f ./$CB_PACKAGE &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Mon, 26 Jul 2021 22:25:00 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.5-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.5 CB_SHA256=6b152590867a58d771cffc22774d3cd66c916defcbeeeb339aca8d0a8e6d7f8d CB_VERSION=6.0.5
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Mon, 26 Jul 2021 22:25:00 GMT
COPY file:d6a307209223b2df102f46f07fd186e09fac7114db2c965bb54097d3b4d3b989 in /etc/service/couchbase-server/run 
# Mon, 26 Jul 2021 22:25:01 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.5-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.5 CB_SHA256=6b152590867a58d771cffc22774d3cd66c916defcbeeeb339aca8d0a8e6d7f8d CB_VERSION=6.0.5
RUN mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Mon, 26 Jul 2021 22:25:01 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Mon, 26 Jul 2021 22:25:02 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.5-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.5 CB_SHA256=6b152590867a58d771cffc22774d3cd66c916defcbeeeb339aca8d0a8e6d7f8d CB_VERSION=6.0.5
RUN ln -s dummy.sh /usr/local/bin/iptables-save &&     ln -s dummy.sh /usr/local/bin/lvdisplay &&     ln -s dummy.sh /usr/local/bin/vgdisplay &&     ln -s dummy.sh /usr/local/bin/pvdisplay
# Mon, 26 Jul 2021 22:25:03 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.5-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.5 CB_SHA256=6b152590867a58d771cffc22774d3cd66c916defcbeeeb339aca8d0a8e6d7f8d CB_VERSION=6.0.5
RUN chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl
# Mon, 26 Jul 2021 22:25:03 GMT
COPY file:d816a67f62bfba76d2812cefbe92252afa13f3852775c3e68599df7741e90cb7 in / 
# Mon, 26 Jul 2021 22:25:04 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 26 Jul 2021 22:25:04 GMT
CMD ["couchbase-server"]
# Mon, 26 Jul 2021 22:25:04 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Mon, 26 Jul 2021 22:25:04 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:feac5306138255e28a9862d3f3d29025d0a4d0648855afe1acd6131af07138ac`  
		Last Modified: Mon, 26 Jul 2021 21:22:52 GMT  
		Size: 26.7 MB (26709039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d34675e7dacc0ce319b39b9ea2535f805fa959a52abc54f87cc0a227b97902ca`  
		Last Modified: Mon, 26 Jul 2021 22:42:05 GMT  
		Size: 15.9 MB (15922947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:889c4fafca81882f6937a23d718195844112f8f700b2bbf19b2fed74fb78653f`  
		Last Modified: Mon, 26 Jul 2021 22:42:00 GMT  
		Size: 266.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70f22272715b7ac39bdeb72247eb7c9d676e111cb87f716a6b7d9a3699677895`  
		Last Modified: Mon, 26 Jul 2021 22:41:58 GMT  
		Size: 2.0 KB (1969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6272140edf88cd01360aac5bddc2d13a011276f72173b6d9ae176fe243afbcbe`  
		Last Modified: Mon, 26 Jul 2021 22:42:41 GMT  
		Size: 423.4 MB (423361988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d78863e03e170d48a06840a1f3c0af08fc6a03998bd8b2cc5bd9d42146459335`  
		Last Modified: Mon, 26 Jul 2021 22:41:58 GMT  
		Size: 191.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce9c75079115b27ecc729a3d9a6ea34ffbbf322b75074b937b0a88b311b44e09`  
		Last Modified: Mon, 26 Jul 2021 22:41:58 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8be88b035f8327fce982f782ee4d4f158a491292ab1a83ea9bec04510e2eeedf`  
		Last Modified: Mon, 26 Jul 2021 22:41:55 GMT  
		Size: 280.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93191caa985b907966beca25f0640d7f64475b6f2662beaa3e13685df8684139`  
		Last Modified: Mon, 26 Jul 2021 22:41:58 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab9a7069e44f4669174a2e317fd06732143189d95777bc146d3897c070d52028`  
		Last Modified: Mon, 26 Jul 2021 22:41:55 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3d37421dd736067d67fc2e040630fd1bc247c1f2cfc75354428c93d6ace6ba3`  
		Last Modified: Mon, 26 Jul 2021 22:41:55 GMT  
		Size: 125.6 KB (125559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa4704f88c75024de08db79dc6908a3dc28f99ca5b88bb3d403b7410161fc66d`  
		Last Modified: Mon, 26 Jul 2021 22:41:55 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchbase:6.5.0`

```console
$ docker pull couchbase@sha256:9387c6f85e86c0fd1d17503901d7736ef79666d3ee434a05d77cab05eb82944f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `couchbase:6.5.0` - linux; amd64

```console
$ docker pull couchbase@sha256:2965cc1703c7207d7c0ab985d3b1d17527ce2b1ed4194c2e94ce4404ab4b7b70
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **542.2 MB (542236366 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:347b738ae0432bd3d41b32b59f1f101c8af3fce36f8aff0db87481fd4b6aa534`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Mon, 26 Jul 2021 21:21:30 GMT
ADD file:e729fb032bd2f7cde20fb343da0cd358447e8b23028422c123944e8d0be660fa in / 
# Mon, 26 Jul 2021 21:21:31 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 22:21:49 GMT
LABEL maintainer=docker@couchbase.com
# Mon, 26 Jul 2021 22:22:25 GMT
RUN set -x &&     apt-get update &&     apt-get install -yq runit wget chrpath tzdata man     lsof lshw sysstat net-tools numactl bzip2 &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Mon, 26 Jul 2021 22:22:26 GMT
RUN if [ ! -x /usr/sbin/runsvdir-start ]; then         cp -a /etc/runit/2 /usr/sbin/runsvdir-start;     fi
# Mon, 26 Jul 2021 22:29:26 GMT
ARG CB_VERSION=6.5.0
# Mon, 26 Jul 2021 22:29:26 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/6.5.0
# Mon, 26 Jul 2021 22:29:27 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_6.5.0-ubuntu18.04_amd64.deb
# Mon, 26 Jul 2021 22:29:27 GMT
ARG CB_SHA256=b4cafdc048b0caba85c24b90e6823e9ec2adc32061cafc527ddc99d706d6bc05
# Mon, 26 Jul 2021 22:29:27 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Mon, 26 Jul 2021 22:29:28 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.5.0-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.5.0 CB_SHA256=b4cafdc048b0caba85c24b90e6823e9ec2adc32061cafc527ddc99d706d6bc05 CB_VERSION=6.5.0
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Mon, 26 Jul 2021 22:30:36 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.5.0-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.5.0 CB_SHA256=b4cafdc048b0caba85c24b90e6823e9ec2adc32061cafc527ddc99d706d6bc05 CB_VERSION=6.5.0
RUN set -x &&     export INSTALL_DONT_START_SERVER=1 &&     wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE &&     echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - &&     apt-get update &&     apt-get install -y ./$CB_PACKAGE &&     rm -f ./$CB_PACKAGE &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Mon, 26 Jul 2021 22:30:40 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.5.0-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.5.0 CB_SHA256=b4cafdc048b0caba85c24b90e6823e9ec2adc32061cafc527ddc99d706d6bc05 CB_VERSION=6.5.0
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Mon, 26 Jul 2021 22:30:40 GMT
COPY file:d6a307209223b2df102f46f07fd186e09fac7114db2c965bb54097d3b4d3b989 in /etc/service/couchbase-server/run 
# Mon, 26 Jul 2021 22:30:41 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.5.0-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.5.0 CB_SHA256=b4cafdc048b0caba85c24b90e6823e9ec2adc32061cafc527ddc99d706d6bc05 CB_VERSION=6.5.0
RUN mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Mon, 26 Jul 2021 22:30:41 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Mon, 26 Jul 2021 22:30:42 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.5.0-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.5.0 CB_SHA256=b4cafdc048b0caba85c24b90e6823e9ec2adc32061cafc527ddc99d706d6bc05 CB_VERSION=6.5.0
RUN ln -s dummy.sh /usr/local/bin/iptables-save &&     ln -s dummy.sh /usr/local/bin/lvdisplay &&     ln -s dummy.sh /usr/local/bin/vgdisplay &&     ln -s dummy.sh /usr/local/bin/pvdisplay
# Mon, 26 Jul 2021 22:30:43 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.5.0-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.5.0 CB_SHA256=b4cafdc048b0caba85c24b90e6823e9ec2adc32061cafc527ddc99d706d6bc05 CB_VERSION=6.5.0
RUN chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl
# Mon, 26 Jul 2021 22:30:43 GMT
COPY file:d816a67f62bfba76d2812cefbe92252afa13f3852775c3e68599df7741e90cb7 in / 
# Mon, 26 Jul 2021 22:30:43 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 26 Jul 2021 22:30:44 GMT
CMD ["couchbase-server"]
# Mon, 26 Jul 2021 22:30:44 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Mon, 26 Jul 2021 22:30:44 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:feac5306138255e28a9862d3f3d29025d0a4d0648855afe1acd6131af07138ac`  
		Last Modified: Mon, 26 Jul 2021 21:22:52 GMT  
		Size: 26.7 MB (26709039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2a4e30704289595ec4268563ba339f4be2e264b88e79d255b680ccc550789ba`  
		Last Modified: Mon, 26 Jul 2021 22:41:09 GMT  
		Size: 7.4 MB (7373152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61d99bab81201d5c70f8e51f9f400575173f81ff7b28365411dc726bd35ec58d`  
		Last Modified: Mon, 26 Jul 2021 22:41:05 GMT  
		Size: 266.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b3f669ec644d0fc9e7ccde33439c5b7d2bbb56bc2ffde1565fdcb2313ffb018`  
		Last Modified: Mon, 26 Jul 2021 22:46:47 GMT  
		Size: 2.0 KB (1968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bad7d2497294635cf86849061925f4f120c3aa5d1f0b2d42ad8676ff616c4f8e`  
		Last Modified: Mon, 26 Jul 2021 22:47:44 GMT  
		Size: 508.0 MB (508031490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:740d72f0611aefdbcbfbab07c53099d044a0588e4316bf4ccd968818aefbd819`  
		Last Modified: Mon, 26 Jul 2021 22:46:46 GMT  
		Size: 191.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f6a2df8e1ea242f8693607bebe20f2a6ab4a568fdf1e6f61228fade370ac06e`  
		Last Modified: Mon, 26 Jul 2021 22:46:46 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0457572c00706de1d6e9522a5f0d2028fefaf79f16be1eb56cbaf6e99847089`  
		Last Modified: Mon, 26 Jul 2021 22:46:44 GMT  
		Size: 281.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9f2e39afe2424c9b028592e19e443ed2f0027473240cc14fdb0b59d093b43c0`  
		Last Modified: Mon, 26 Jul 2021 22:46:44 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d3ab6e813da57c9c0300bce664c95c9915a442625363458afc273024570886c`  
		Last Modified: Mon, 26 Jul 2021 22:46:44 GMT  
		Size: 217.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73f1e5798c71eda8b93bcc34c342819e6549ff71f3a52f972d1cbe39916ce41a`  
		Last Modified: Mon, 26 Jul 2021 22:46:44 GMT  
		Size: 118.2 KB (118191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b285cea2534462bf1b30a6c0fa6e4cab474972698b161529d550b92c8200200`  
		Last Modified: Mon, 26 Jul 2021 22:46:44 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchbase:6.5.1`

```console
$ docker pull couchbase@sha256:0254bc931089c931928c7928c76dffbb0e6039c59ae8f94dd5f113cc348700fc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `couchbase:6.5.1` - linux; amd64

```console
$ docker pull couchbase@sha256:56a7834eec771d194ef48a8c6c2df0a84c55be5556b2b30cff47bb46f7ef3fc0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **501.5 MB (501511512 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:83022788e529e8261037bba84084b8b245c561f826e586164f0c6ef351137f02`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Mon, 26 Jul 2021 21:21:30 GMT
ADD file:e729fb032bd2f7cde20fb343da0cd358447e8b23028422c123944e8d0be660fa in / 
# Mon, 26 Jul 2021 21:21:31 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 22:21:49 GMT
LABEL maintainer=docker@couchbase.com
# Mon, 26 Jul 2021 22:22:25 GMT
RUN set -x &&     apt-get update &&     apt-get install -yq runit wget chrpath tzdata man     lsof lshw sysstat net-tools numactl bzip2 &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Mon, 26 Jul 2021 22:22:26 GMT
RUN if [ ! -x /usr/sbin/runsvdir-start ]; then         cp -a /etc/runit/2 /usr/sbin/runsvdir-start;     fi
# Mon, 26 Jul 2021 22:28:01 GMT
ARG CB_VERSION=6.5.1
# Mon, 26 Jul 2021 22:28:01 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/6.5.1
# Mon, 26 Jul 2021 22:28:01 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_6.5.1-ubuntu18.04_amd64.deb
# Mon, 26 Jul 2021 22:28:01 GMT
ARG CB_SHA256=992fc9aef85c210cc2d782a1726f2ef56ceb322fd67c2e95500e276ff106e6ff
# Mon, 26 Jul 2021 22:28:02 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Mon, 26 Jul 2021 22:28:03 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.5.1-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.5.1 CB_SHA256=992fc9aef85c210cc2d782a1726f2ef56ceb322fd67c2e95500e276ff106e6ff CB_VERSION=6.5.1
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Mon, 26 Jul 2021 22:29:05 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.5.1-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.5.1 CB_SHA256=992fc9aef85c210cc2d782a1726f2ef56ceb322fd67c2e95500e276ff106e6ff CB_VERSION=6.5.1
RUN set -x &&     export INSTALL_DONT_START_SERVER=1 &&     wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE &&     echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - &&     apt-get update &&     apt-get install -y ./$CB_PACKAGE &&     rm -f ./$CB_PACKAGE &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Mon, 26 Jul 2021 22:29:07 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.5.1-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.5.1 CB_SHA256=992fc9aef85c210cc2d782a1726f2ef56ceb322fd67c2e95500e276ff106e6ff CB_VERSION=6.5.1
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Mon, 26 Jul 2021 22:29:08 GMT
COPY file:d6a307209223b2df102f46f07fd186e09fac7114db2c965bb54097d3b4d3b989 in /etc/service/couchbase-server/run 
# Mon, 26 Jul 2021 22:29:08 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.5.1-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.5.1 CB_SHA256=992fc9aef85c210cc2d782a1726f2ef56ceb322fd67c2e95500e276ff106e6ff CB_VERSION=6.5.1
RUN mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Mon, 26 Jul 2021 22:29:09 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Mon, 26 Jul 2021 22:29:09 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.5.1-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.5.1 CB_SHA256=992fc9aef85c210cc2d782a1726f2ef56ceb322fd67c2e95500e276ff106e6ff CB_VERSION=6.5.1
RUN ln -s dummy.sh /usr/local/bin/iptables-save &&     ln -s dummy.sh /usr/local/bin/lvdisplay &&     ln -s dummy.sh /usr/local/bin/vgdisplay &&     ln -s dummy.sh /usr/local/bin/pvdisplay
# Mon, 26 Jul 2021 22:29:10 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.5.1-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.5.1 CB_SHA256=992fc9aef85c210cc2d782a1726f2ef56ceb322fd67c2e95500e276ff106e6ff CB_VERSION=6.5.1
RUN chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl
# Mon, 26 Jul 2021 22:29:10 GMT
COPY file:d816a67f62bfba76d2812cefbe92252afa13f3852775c3e68599df7741e90cb7 in / 
# Mon, 26 Jul 2021 22:29:11 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 26 Jul 2021 22:29:11 GMT
CMD ["couchbase-server"]
# Mon, 26 Jul 2021 22:29:11 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Mon, 26 Jul 2021 22:29:11 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:feac5306138255e28a9862d3f3d29025d0a4d0648855afe1acd6131af07138ac`  
		Last Modified: Mon, 26 Jul 2021 21:22:52 GMT  
		Size: 26.7 MB (26709039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2a4e30704289595ec4268563ba339f4be2e264b88e79d255b680ccc550789ba`  
		Last Modified: Mon, 26 Jul 2021 22:41:09 GMT  
		Size: 7.4 MB (7373152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61d99bab81201d5c70f8e51f9f400575173f81ff7b28365411dc726bd35ec58d`  
		Last Modified: Mon, 26 Jul 2021 22:41:05 GMT  
		Size: 266.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:909345a645bc1c08329c7e80a3ff9fe1563ed753d2dc3e1eb03710bc35d44b40`  
		Last Modified: Mon, 26 Jul 2021 22:45:20 GMT  
		Size: 2.0 KB (1967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d855aad2e6af91ab6111b5826d3c1f948a6d3c6f173774756d73396793f5b89`  
		Last Modified: Mon, 26 Jul 2021 22:46:31 GMT  
		Size: 467.3 MB (467306639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68ea3f8ca21443b02bfba5a81304bfb1d7fe48119ff7bd55e285060b8c01bc68`  
		Last Modified: Mon, 26 Jul 2021 22:45:19 GMT  
		Size: 191.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a033f399787e6c32952c51add442bbd917a21958d0e4e59a4f3198a7b151205`  
		Last Modified: Mon, 26 Jul 2021 22:45:19 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b018f31e1c826afe291229aca140c54e623e1cfe7856459e93508a1d74799ac1`  
		Last Modified: Mon, 26 Jul 2021 22:45:17 GMT  
		Size: 281.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f041538ba3d0f3d11edbc9bdd75b7bfb070898fce64e34b08f3478780e1f08e`  
		Last Modified: Mon, 26 Jul 2021 22:45:16 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b72a132b7ddc7e6e2880deee77c218e55cc861c431858e464bdb154a2b7add1`  
		Last Modified: Mon, 26 Jul 2021 22:45:17 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ec6595ad3e89a6657440b99ffc0bfb797484e3e0ca28112fda1a4d062992dfc`  
		Last Modified: Mon, 26 Jul 2021 22:45:17 GMT  
		Size: 118.2 KB (118189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cd04f6da791cb9462e3e23cef1a4227594d77bbec153ae8c01cb59b152f3ace`  
		Last Modified: Mon, 26 Jul 2021 22:45:17 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchbase:6.6.0`

```console
$ docker pull couchbase@sha256:6b1d9cf03e16f6a4095c6ad367d0fa4e745e56825f794e3f0f6af9365f5eb01a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `couchbase:6.6.0` - linux; amd64

```console
$ docker pull couchbase@sha256:a2fc8cdd66c14a37b99b2494605e858bcb143cf9cdf376f3b7d1ec1acd66472e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **527.3 MB (527324890 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66d0f108e14b26d51dd738bb8af7e7f8e3779b0750eaa93ff9a2e3672499a0f6`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Mon, 26 Jul 2021 21:21:30 GMT
ADD file:e729fb032bd2f7cde20fb343da0cd358447e8b23028422c123944e8d0be660fa in / 
# Mon, 26 Jul 2021 21:21:31 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 22:21:49 GMT
LABEL maintainer=docker@couchbase.com
# Mon, 26 Jul 2021 22:22:25 GMT
RUN set -x &&     apt-get update &&     apt-get install -yq runit wget chrpath tzdata man     lsof lshw sysstat net-tools numactl bzip2 &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Mon, 26 Jul 2021 22:22:26 GMT
RUN if [ ! -x /usr/sbin/runsvdir-start ]; then         cp -a /etc/runit/2 /usr/sbin/runsvdir-start;     fi
# Mon, 26 Jul 2021 22:22:27 GMT
ARG CB_VERSION=6.6.0
# Mon, 26 Jul 2021 22:22:27 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0
# Mon, 26 Jul 2021 22:26:35 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_6.6.0-ubuntu18.04_amd64.deb
# Mon, 26 Jul 2021 22:26:36 GMT
ARG CB_SHA256=8e7fd5434537094be2fbdfedf3ab5005f0f7d5b9d0578f59ce540b424215b728
# Mon, 26 Jul 2021 22:26:36 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Mon, 26 Jul 2021 22:26:37 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.0-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=8e7fd5434537094be2fbdfedf3ab5005f0f7d5b9d0578f59ce540b424215b728 CB_VERSION=6.6.0
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Mon, 26 Jul 2021 22:27:43 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.0-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=8e7fd5434537094be2fbdfedf3ab5005f0f7d5b9d0578f59ce540b424215b728 CB_VERSION=6.6.0
RUN set -x &&     export INSTALL_DONT_START_SERVER=1 &&     wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE &&     echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - &&     apt-get update &&     apt-get install -y ./$CB_PACKAGE &&     rm -f ./$CB_PACKAGE &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Mon, 26 Jul 2021 22:27:47 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.0-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=8e7fd5434537094be2fbdfedf3ab5005f0f7d5b9d0578f59ce540b424215b728 CB_VERSION=6.6.0
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Mon, 26 Jul 2021 22:27:47 GMT
COPY file:d6a307209223b2df102f46f07fd186e09fac7114db2c965bb54097d3b4d3b989 in /etc/service/couchbase-server/run 
# Mon, 26 Jul 2021 22:27:48 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.0-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=8e7fd5434537094be2fbdfedf3ab5005f0f7d5b9d0578f59ce540b424215b728 CB_VERSION=6.6.0
RUN mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Mon, 26 Jul 2021 22:27:48 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Mon, 26 Jul 2021 22:27:49 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.0-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=8e7fd5434537094be2fbdfedf3ab5005f0f7d5b9d0578f59ce540b424215b728 CB_VERSION=6.6.0
RUN ln -s dummy.sh /usr/local/bin/iptables-save &&     ln -s dummy.sh /usr/local/bin/lvdisplay &&     ln -s dummy.sh /usr/local/bin/vgdisplay &&     ln -s dummy.sh /usr/local/bin/pvdisplay
# Mon, 26 Jul 2021 22:27:50 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.0-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=8e7fd5434537094be2fbdfedf3ab5005f0f7d5b9d0578f59ce540b424215b728 CB_VERSION=6.6.0
RUN chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl
# Mon, 26 Jul 2021 22:27:50 GMT
COPY file:d816a67f62bfba76d2812cefbe92252afa13f3852775c3e68599df7741e90cb7 in / 
# Mon, 26 Jul 2021 22:27:50 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 26 Jul 2021 22:27:50 GMT
CMD ["couchbase-server"]
# Mon, 26 Jul 2021 22:27:50 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Mon, 26 Jul 2021 22:27:51 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:feac5306138255e28a9862d3f3d29025d0a4d0648855afe1acd6131af07138ac`  
		Last Modified: Mon, 26 Jul 2021 21:22:52 GMT  
		Size: 26.7 MB (26709039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2a4e30704289595ec4268563ba339f4be2e264b88e79d255b680ccc550789ba`  
		Last Modified: Mon, 26 Jul 2021 22:41:09 GMT  
		Size: 7.4 MB (7373152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61d99bab81201d5c70f8e51f9f400575173f81ff7b28365411dc726bd35ec58d`  
		Last Modified: Mon, 26 Jul 2021 22:41:05 GMT  
		Size: 266.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c41056bf321c297635440676aa8845205766d98187c02bbb0a0a92dd844538c4`  
		Last Modified: Mon, 26 Jul 2021 22:44:07 GMT  
		Size: 2.0 KB (1966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1f4495478f55c2361512c14fd11182a2c4762b7dfa481381ad3133b3d9595dd`  
		Last Modified: Mon, 26 Jul 2021 22:45:03 GMT  
		Size: 493.1 MB (493120019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cf43d796878a1c1cbd05a076c43355bd3b70687d8bd28a1932468f2182eefce`  
		Last Modified: Mon, 26 Jul 2021 22:44:07 GMT  
		Size: 192.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af7fb99ce5d639f6830d982c769cde2d24eec0d1bcddb832c2bcee4b3d1f2c60`  
		Last Modified: Mon, 26 Jul 2021 22:44:07 GMT  
		Size: 479.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75040a6a6dac742b25c0f0fa89532c640f15591ec21af151eeafd6db74070c88`  
		Last Modified: Mon, 26 Jul 2021 22:44:04 GMT  
		Size: 280.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c0487699075b1f4c7b8cebd39a8d8973a207bac0c9b3717f95d8e83bd71fbb6`  
		Last Modified: Mon, 26 Jul 2021 22:44:04 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15756c2d9aecb2c909ac2b15a62c03f69345255bf9668f054e508d9c5a190ea1`  
		Last Modified: Mon, 26 Jul 2021 22:44:04 GMT  
		Size: 216.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a5b8651b569598c05e40067a744cc25f246fbce0a6ce50647dcbed6163a809a`  
		Last Modified: Mon, 26 Jul 2021 22:44:05 GMT  
		Size: 118.2 KB (118188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac7d1df271491a4d154090a38f26441d5575fa533057c224ced3295c0ff1871b`  
		Last Modified: Mon, 26 Jul 2021 22:44:04 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchbase:6.6.1`

```console
$ docker pull couchbase@sha256:ce27277fe7678f903b02438304ff57ff4455002bb9440844f2ff31a2eed2a2bd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `couchbase:6.6.1` - linux; amd64

```console
$ docker pull couchbase@sha256:8bae907adf53a82ae94c070752625dc94f9014807a26a232945d26eccdacbebb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **528.5 MB (528527045 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5b6f9c5715a276870475d948a55b433361fb63fab1c87dc085c57b563e089cda`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Mon, 26 Jul 2021 21:21:30 GMT
ADD file:e729fb032bd2f7cde20fb343da0cd358447e8b23028422c123944e8d0be660fa in / 
# Mon, 26 Jul 2021 21:21:31 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 22:21:49 GMT
LABEL maintainer=docker@couchbase.com
# Mon, 26 Jul 2021 22:22:25 GMT
RUN set -x &&     apt-get update &&     apt-get install -yq runit wget chrpath tzdata man     lsof lshw sysstat net-tools numactl bzip2 &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Mon, 26 Jul 2021 22:22:26 GMT
RUN if [ ! -x /usr/sbin/runsvdir-start ]; then         cp -a /etc/runit/2 /usr/sbin/runsvdir-start;     fi
# Mon, 26 Jul 2021 22:25:10 GMT
ARG CB_VERSION=6.6.1
# Mon, 26 Jul 2021 22:25:10 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.1
# Mon, 26 Jul 2021 22:25:10 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_6.6.1-ubuntu18.04_amd64.deb
# Mon, 26 Jul 2021 22:25:10 GMT
ARG CB_SHA256=4bd8210458905a5801e98bda0663d1214f6743465843f49ef9a52212636b5e89
# Mon, 26 Jul 2021 22:25:11 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Mon, 26 Jul 2021 22:25:11 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.1-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.1 CB_SHA256=4bd8210458905a5801e98bda0663d1214f6743465843f49ef9a52212636b5e89 CB_VERSION=6.6.1
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Mon, 26 Jul 2021 22:26:19 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.1-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.1 CB_SHA256=4bd8210458905a5801e98bda0663d1214f6743465843f49ef9a52212636b5e89 CB_VERSION=6.6.1
RUN set -x &&     export INSTALL_DONT_START_SERVER=1 &&     wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE &&     echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - &&     apt-get update &&     apt-get install -y ./$CB_PACKAGE &&     rm -f ./$CB_PACKAGE &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Mon, 26 Jul 2021 22:26:23 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.1-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.1 CB_SHA256=4bd8210458905a5801e98bda0663d1214f6743465843f49ef9a52212636b5e89 CB_VERSION=6.6.1
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Mon, 26 Jul 2021 22:26:23 GMT
COPY file:d6a307209223b2df102f46f07fd186e09fac7114db2c965bb54097d3b4d3b989 in /etc/service/couchbase-server/run 
# Mon, 26 Jul 2021 22:26:24 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.1-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.1 CB_SHA256=4bd8210458905a5801e98bda0663d1214f6743465843f49ef9a52212636b5e89 CB_VERSION=6.6.1
RUN mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Mon, 26 Jul 2021 22:26:24 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Mon, 26 Jul 2021 22:26:25 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.1-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.1 CB_SHA256=4bd8210458905a5801e98bda0663d1214f6743465843f49ef9a52212636b5e89 CB_VERSION=6.6.1
RUN ln -s dummy.sh /usr/local/bin/iptables-save &&     ln -s dummy.sh /usr/local/bin/lvdisplay &&     ln -s dummy.sh /usr/local/bin/vgdisplay &&     ln -s dummy.sh /usr/local/bin/pvdisplay
# Mon, 26 Jul 2021 22:26:26 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.1-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.1 CB_SHA256=4bd8210458905a5801e98bda0663d1214f6743465843f49ef9a52212636b5e89 CB_VERSION=6.6.1
RUN chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl
# Mon, 26 Jul 2021 22:26:26 GMT
COPY file:d816a67f62bfba76d2812cefbe92252afa13f3852775c3e68599df7741e90cb7 in / 
# Mon, 26 Jul 2021 22:26:26 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 26 Jul 2021 22:26:26 GMT
CMD ["couchbase-server"]
# Mon, 26 Jul 2021 22:26:27 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Mon, 26 Jul 2021 22:26:27 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:feac5306138255e28a9862d3f3d29025d0a4d0648855afe1acd6131af07138ac`  
		Last Modified: Mon, 26 Jul 2021 21:22:52 GMT  
		Size: 26.7 MB (26709039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2a4e30704289595ec4268563ba339f4be2e264b88e79d255b680ccc550789ba`  
		Last Modified: Mon, 26 Jul 2021 22:41:09 GMT  
		Size: 7.4 MB (7373152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61d99bab81201d5c70f8e51f9f400575173f81ff7b28365411dc726bd35ec58d`  
		Last Modified: Mon, 26 Jul 2021 22:41:05 GMT  
		Size: 266.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ab2f6ba05defbc278962d5c3675edb87a2a9aac298f764d149e8dfac6997210`  
		Last Modified: Mon, 26 Jul 2021 22:42:56 GMT  
		Size: 2.0 KB (1967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca281ad084b9caeb2bd4303f9ba708ebf5253a02428a14105ce61f4ad6c1649d`  
		Last Modified: Mon, 26 Jul 2021 22:43:52 GMT  
		Size: 494.3 MB (494322167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ee6152ff40f616ef043558d6c3bdb575595e9dcef1fdd0861342cf30cf9ad83`  
		Last Modified: Mon, 26 Jul 2021 22:42:56 GMT  
		Size: 191.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8076a41dccc574445e6fe0e1c3da4ac85e5d04a288a65f361e88bba93f8608aa`  
		Last Modified: Mon, 26 Jul 2021 22:42:57 GMT  
		Size: 479.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca6e027e9667d6d17e6ce6ac1a8893da041ed62683c31c582bdb8f1d738e50f8`  
		Last Modified: Mon, 26 Jul 2021 22:42:53 GMT  
		Size: 282.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fdbc0e5c5c39515362d1bb28bac1458a462fd9522995f866b1a24b4f5dd9063`  
		Last Modified: Mon, 26 Jul 2021 22:42:53 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4512e7ea1b1be5ec7744ca0b9d0e4c3c0720ed6fb5b2055b3c10f583b3ed25b3`  
		Last Modified: Mon, 26 Jul 2021 22:42:54 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ee32e5567f13959d200c1b58d732468142ea10d9e3e7a05bb249614074b6e05`  
		Last Modified: Mon, 26 Jul 2021 22:42:54 GMT  
		Size: 118.2 KB (118190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3cc78198ad3662750502dc48a81a466e27e0ad29b7f8970f2acfc87524c0d50`  
		Last Modified: Mon, 26 Jul 2021 22:42:53 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchbase:6.6.2`

```console
$ docker pull couchbase@sha256:9e6e9947a937f0e1d692deb0276131e10f0f12a8fd469e33d30fdd6b6a658c73
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `couchbase:6.6.2` - linux; amd64

```console
$ docker pull couchbase@sha256:2befadeed5bbfd07b657995c9432dad470840d4b32d8757c4de44f1f8bdb0bf6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **533.2 MB (533222654 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89c4c1a0b656b1893a5cc9277f0a39ac1771db24a19fcb5cd17e2c96f5b6f01d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Mon, 26 Jul 2021 21:21:39 GMT
ADD file:524e8d93ad65f08a0cb0d144268350186e36f508006b05b8faf2e1289499b59f in / 
# Mon, 26 Jul 2021 21:21:40 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 22:17:12 GMT
LABEL maintainer=docker@couchbase.com
# Mon, 26 Jul 2021 22:20:33 GMT
RUN set -x &&     apt-get update &&     apt-get install -yq runit wget chrpath tzdata     lsof lshw sysstat net-tools numactl bzip2 &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Mon, 26 Jul 2021 22:20:33 GMT
RUN if [ ! -x /usr/sbin/runsvdir-start ]; then         cp -a /etc/runit/2 /usr/sbin/runsvdir-start;     fi
# Mon, 26 Jul 2021 22:20:34 GMT
ARG CB_VERSION=6.6.2
# Mon, 26 Jul 2021 22:20:34 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.2
# Mon, 26 Jul 2021 22:20:34 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_6.6.2-ubuntu20.04_amd64.deb
# Mon, 26 Jul 2021 22:20:34 GMT
ARG CB_SHA256=41c033e6c1e98b0844a5cb5768e3769e7012d8374a6bd235c86e10db33b17afc
# Mon, 26 Jul 2021 22:20:34 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Mon, 26 Jul 2021 22:20:35 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.2-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.2 CB_SHA256=41c033e6c1e98b0844a5cb5768e3769e7012d8374a6bd235c86e10db33b17afc CB_VERSION=6.6.2
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Mon, 26 Jul 2021 22:21:31 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.2-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.2 CB_SHA256=41c033e6c1e98b0844a5cb5768e3769e7012d8374a6bd235c86e10db33b17afc CB_VERSION=6.6.2
RUN set -x &&     export INSTALL_DONT_START_SERVER=1 &&     wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE &&     echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - &&     apt-get update &&     apt-get install -y ./$CB_PACKAGE &&     rm -f ./$CB_PACKAGE &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Mon, 26 Jul 2021 22:21:35 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.2-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.2 CB_SHA256=41c033e6c1e98b0844a5cb5768e3769e7012d8374a6bd235c86e10db33b17afc CB_VERSION=6.6.2
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Mon, 26 Jul 2021 22:21:35 GMT
COPY file:d6a307209223b2df102f46f07fd186e09fac7114db2c965bb54097d3b4d3b989 in /etc/service/couchbase-server/run 
# Mon, 26 Jul 2021 22:21:36 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.2-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.2 CB_SHA256=41c033e6c1e98b0844a5cb5768e3769e7012d8374a6bd235c86e10db33b17afc CB_VERSION=6.6.2
RUN mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Mon, 26 Jul 2021 22:21:36 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Mon, 26 Jul 2021 22:21:37 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.2-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.2 CB_SHA256=41c033e6c1e98b0844a5cb5768e3769e7012d8374a6bd235c86e10db33b17afc CB_VERSION=6.6.2
RUN ln -s dummy.sh /usr/local/bin/iptables-save &&     ln -s dummy.sh /usr/local/bin/lvdisplay &&     ln -s dummy.sh /usr/local/bin/vgdisplay &&     ln -s dummy.sh /usr/local/bin/pvdisplay
# Mon, 26 Jul 2021 22:21:38 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.2-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.2 CB_SHA256=41c033e6c1e98b0844a5cb5768e3769e7012d8374a6bd235c86e10db33b17afc CB_VERSION=6.6.2
RUN chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl
# Mon, 26 Jul 2021 22:21:38 GMT
COPY file:d816a67f62bfba76d2812cefbe92252afa13f3852775c3e68599df7741e90cb7 in / 
# Mon, 26 Jul 2021 22:21:38 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 26 Jul 2021 22:21:38 GMT
CMD ["couchbase-server"]
# Mon, 26 Jul 2021 22:21:39 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Mon, 26 Jul 2021 22:21:39 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:16ec32c2132b43494832a05f2b02f7a822479f8250c173d0ab27b3de78b2f058`  
		Last Modified: Sun, 25 Jul 2021 03:03:29 GMT  
		Size: 28.6 MB (28567944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d887c602d6e2b416c36a7344e07f41278a46971fa08be0eeb2fc78a75d7013b`  
		Last Modified: Mon, 26 Jul 2021 22:39:49 GMT  
		Size: 6.3 MB (6272568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b219d16ecda3370190c17757e31f650c0b2db8a483364cebc0add69c976f1fa`  
		Last Modified: Mon, 26 Jul 2021 22:39:45 GMT  
		Size: 264.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:febb3fec572429eea18c02afb8a6c9879b303a8fe54f24c598d70e76284d2e50`  
		Last Modified: Mon, 26 Jul 2021 22:39:45 GMT  
		Size: 1.8 KB (1836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc966ce6300d6331c07980d729ddad541989a337e6eb174cab32a6da22196a4b`  
		Last Modified: Mon, 26 Jul 2021 22:40:42 GMT  
		Size: 498.3 MB (498251893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edb4c7a902a3d8673bde3e41bdcafb1f24b6bd970572a368d1d1c290bc0f0c5c`  
		Last Modified: Mon, 26 Jul 2021 22:39:45 GMT  
		Size: 191.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef06a70d616a9d9e24737530889d9744fa42fa92f9c293f9a47ab5046769e4e5`  
		Last Modified: Mon, 26 Jul 2021 22:39:45 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8a527aa307ea3cd1feffde8b7b71f90af3149dc21432afb9d9c9187c61017c5`  
		Last Modified: Mon, 26 Jul 2021 22:39:42 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4233c8f62d720537a74a69707dd1d651286d9bfab88848bb8d41445266481254`  
		Last Modified: Mon, 26 Jul 2021 22:39:42 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dda6ae4667566d063e0d185b915cc7fe3d16ea8dd7504aa48ae246e35db9d509`  
		Last Modified: Mon, 26 Jul 2021 22:39:42 GMT  
		Size: 217.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01243b96b0b7ddaf69634a7674356f0e483f5f24e91d57de48d161fcf28d65d0`  
		Last Modified: Mon, 26 Jul 2021 22:39:42 GMT  
		Size: 125.9 KB (125893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74aee4374d591a250acc5a5e8b2be6cacffceebba6ee89c2fe32ba3806144098`  
		Last Modified: Mon, 26 Jul 2021 22:39:42 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchbase:7.0.0-beta`

```console
$ docker pull couchbase@sha256:6e44fa2454163f3b8225d8c4e3e0dfe90b884b78a69c35a806661ce96864adcc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `couchbase:7.0.0-beta` - linux; amd64

```console
$ docker pull couchbase@sha256:9fe1cfbda9c8d987400c98872565178920a569c0c9fa50cb0b0e5b6bb40d248c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **628.1 MB (628099501 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f6a21205c8b00e182d981b8f3e6e3cfa85e3302d9ee85cc1c205da4f010f031d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Mon, 26 Jul 2021 21:21:39 GMT
ADD file:524e8d93ad65f08a0cb0d144268350186e36f508006b05b8faf2e1289499b59f in / 
# Mon, 26 Jul 2021 21:21:40 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 22:17:12 GMT
LABEL maintainer=docker@couchbase.com
# Mon, 26 Jul 2021 22:17:38 GMT
RUN set -x &&     apt-get update &&     apt-get install -yq runit wget chrpath tzdata man     lsof lshw sysstat net-tools numactl bzip2 &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Mon, 26 Jul 2021 22:17:39 GMT
RUN if [ ! -x /usr/sbin/runsvdir-start ]; then         cp -a /etc/runit/2 /usr/sbin/runsvdir-start;     fi
# Mon, 26 Jul 2021 22:17:39 GMT
ARG CB_VERSION=7.0.0-beta
# Mon, 26 Jul 2021 22:17:39 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.0-beta
# Mon, 26 Jul 2021 22:17:39 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_7.0.0-beta-ubuntu20.04_amd64.deb
# Mon, 26 Jul 2021 22:17:40 GMT
ARG CB_SHA256=e24be4f765eafbfbfdd5f7eddb780006084e3bd01cbcb3d3880dd9be48b955f6
# Mon, 26 Jul 2021 22:17:40 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Mon, 26 Jul 2021 22:17:41 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.0-beta-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.0-beta CB_SHA256=e24be4f765eafbfbfdd5f7eddb780006084e3bd01cbcb3d3880dd9be48b955f6 CB_VERSION=7.0.0-beta
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Mon, 26 Jul 2021 22:18:57 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.0-beta-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.0-beta CB_SHA256=e24be4f765eafbfbfdd5f7eddb780006084e3bd01cbcb3d3880dd9be48b955f6 CB_VERSION=7.0.0-beta
RUN set -x &&     export INSTALL_DONT_START_SERVER=1 &&     wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE &&     echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - &&     apt-get update &&     apt-get install -y ./$CB_PACKAGE &&     rm -f ./$CB_PACKAGE &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Mon, 26 Jul 2021 22:19:02 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.0-beta-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.0-beta CB_SHA256=e24be4f765eafbfbfdd5f7eddb780006084e3bd01cbcb3d3880dd9be48b955f6 CB_VERSION=7.0.0-beta
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Mon, 26 Jul 2021 22:19:02 GMT
COPY file:d6a307209223b2df102f46f07fd186e09fac7114db2c965bb54097d3b4d3b989 in /etc/service/couchbase-server/run 
# Mon, 26 Jul 2021 22:19:03 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.0-beta-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.0-beta CB_SHA256=e24be4f765eafbfbfdd5f7eddb780006084e3bd01cbcb3d3880dd9be48b955f6 CB_VERSION=7.0.0-beta
RUN mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Mon, 26 Jul 2021 22:19:03 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Mon, 26 Jul 2021 22:19:04 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.0-beta-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.0-beta CB_SHA256=e24be4f765eafbfbfdd5f7eddb780006084e3bd01cbcb3d3880dd9be48b955f6 CB_VERSION=7.0.0-beta
RUN ln -s dummy.sh /usr/local/bin/iptables-save &&     ln -s dummy.sh /usr/local/bin/lvdisplay &&     ln -s dummy.sh /usr/local/bin/vgdisplay &&     ln -s dummy.sh /usr/local/bin/pvdisplay
# Mon, 26 Jul 2021 22:19:05 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.0-beta-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.0-beta CB_SHA256=e24be4f765eafbfbfdd5f7eddb780006084e3bd01cbcb3d3880dd9be48b955f6 CB_VERSION=7.0.0-beta
RUN chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl
# Mon, 26 Jul 2021 22:19:05 GMT
COPY file:d816a67f62bfba76d2812cefbe92252afa13f3852775c3e68599df7741e90cb7 in / 
# Mon, 26 Jul 2021 22:19:05 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 26 Jul 2021 22:19:06 GMT
CMD ["couchbase-server"]
# Mon, 26 Jul 2021 22:19:06 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Mon, 26 Jul 2021 22:19:06 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:16ec32c2132b43494832a05f2b02f7a822479f8250c173d0ab27b3de78b2f058`  
		Last Modified: Sun, 25 Jul 2021 03:03:29 GMT  
		Size: 28.6 MB (28567944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0f4f47bb294f3f6f2dc58514a7dc33b42f8be77cfbbed0dbd1c8a49fca73899`  
		Last Modified: Mon, 26 Jul 2021 22:37:21 GMT  
		Size: 8.3 MB (8287040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e87aaeab53b206101d3fd9751a01810367e7cc684b3636f34e03abd4eec34d3`  
		Last Modified: Mon, 26 Jul 2021 22:37:16 GMT  
		Size: 264.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:417c7614b0fa37252a483308c9753ce5585933d987ea87961c5d9f55f79b720f`  
		Last Modified: Mon, 26 Jul 2021 22:37:16 GMT  
		Size: 1.8 KB (1837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2fde59718fdb413fa07cd7726e0c1f85f79c58d5ed1b201ac7e176d760bbb13`  
		Last Modified: Mon, 26 Jul 2021 22:38:28 GMT  
		Size: 591.1 MB (591114272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c2080252da7d35cf811f882d0f2a573fc3ea1a2c1b150c79368504002e92108`  
		Last Modified: Mon, 26 Jul 2021 22:37:16 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ad5beec000a75f8a1317b3a750fa17fa79638ed6a6fbb98dd91da2cd108a5bf`  
		Last Modified: Mon, 26 Jul 2021 22:37:16 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41bf72ef287f7997839083e39e4cadffa670e9cff91d572cbf064e7401a7bbd2`  
		Last Modified: Mon, 26 Jul 2021 22:37:13 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7973404887aa66902dd9a9e71fb076a67b3fac23ee1f3959be162f6f4bea088`  
		Last Modified: Mon, 26 Jul 2021 22:37:13 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da5872978d3451c5bf98a88425bcbaab9acd795c10fe9a46d5e416e0af549199`  
		Last Modified: Mon, 26 Jul 2021 22:37:13 GMT  
		Size: 217.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03667f47b7202daf73978394d95beca395bc90ecb6a0ff4f6f4e09cd442db30d`  
		Last Modified: Mon, 26 Jul 2021 22:37:14 GMT  
		Size: 125.9 KB (125894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83063b4e8c4354d6466cc2e72d4ec1ff97ff5f81bea8512990a6fa4d01f993e4`  
		Last Modified: Mon, 26 Jul 2021 22:37:14 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchbase:community`

```console
$ docker pull couchbase@sha256:b0baeef769e4ba8fab7ac8e0a78416a009de893fb3d6bf9c1dcbb75130fd004c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `couchbase:community` - linux; amd64

```console
$ docker pull couchbase@sha256:610c0d832bdb7e0144b88a509c9b857bf1551ae55572450dee2e2515eba3b313
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **354.2 MB (354223029 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b2ef0dbd9aca1cefb55ddecf92c830dda7d3d252e86f4a7511de382b757502e`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Mon, 26 Jul 2021 21:21:30 GMT
ADD file:e729fb032bd2f7cde20fb343da0cd358447e8b23028422c123944e8d0be660fa in / 
# Mon, 26 Jul 2021 21:21:31 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 22:21:49 GMT
LABEL maintainer=docker@couchbase.com
# Mon, 26 Jul 2021 22:22:25 GMT
RUN set -x &&     apt-get update &&     apt-get install -yq runit wget chrpath tzdata man     lsof lshw sysstat net-tools numactl bzip2 &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Mon, 26 Jul 2021 22:22:26 GMT
RUN if [ ! -x /usr/sbin/runsvdir-start ]; then         cp -a /etc/runit/2 /usr/sbin/runsvdir-start;     fi
# Mon, 26 Jul 2021 22:22:27 GMT
ARG CB_VERSION=6.6.0
# Mon, 26 Jul 2021 22:22:27 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0
# Mon, 26 Jul 2021 22:22:27 GMT
ARG CB_PACKAGE=couchbase-server-community_6.6.0-ubuntu18.04_amd64.deb
# Mon, 26 Jul 2021 22:22:27 GMT
ARG CB_SHA256=9b196cd7be81d7d6b179838e9d30164fdb7a1f27e96678e61e24e9fe5c93f559
# Mon, 26 Jul 2021 22:22:28 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Mon, 26 Jul 2021 22:22:28 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_6.6.0-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=9b196cd7be81d7d6b179838e9d30164fdb7a1f27e96678e61e24e9fe5c93f559 CB_VERSION=6.6.0
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Mon, 26 Jul 2021 22:23:07 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_6.6.0-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=9b196cd7be81d7d6b179838e9d30164fdb7a1f27e96678e61e24e9fe5c93f559 CB_VERSION=6.6.0
RUN set -x &&     export INSTALL_DONT_START_SERVER=1 &&     wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE &&     echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - &&     apt-get update &&     apt-get install -y ./$CB_PACKAGE &&     rm -f ./$CB_PACKAGE &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Mon, 26 Jul 2021 22:23:10 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_6.6.0-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=9b196cd7be81d7d6b179838e9d30164fdb7a1f27e96678e61e24e9fe5c93f559 CB_VERSION=6.6.0
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Mon, 26 Jul 2021 22:23:10 GMT
COPY file:d6a307209223b2df102f46f07fd186e09fac7114db2c965bb54097d3b4d3b989 in /etc/service/couchbase-server/run 
# Mon, 26 Jul 2021 22:23:11 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_6.6.0-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=9b196cd7be81d7d6b179838e9d30164fdb7a1f27e96678e61e24e9fe5c93f559 CB_VERSION=6.6.0
RUN mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Mon, 26 Jul 2021 22:23:11 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Mon, 26 Jul 2021 22:23:12 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_6.6.0-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=9b196cd7be81d7d6b179838e9d30164fdb7a1f27e96678e61e24e9fe5c93f559 CB_VERSION=6.6.0
RUN ln -s dummy.sh /usr/local/bin/iptables-save &&     ln -s dummy.sh /usr/local/bin/lvdisplay &&     ln -s dummy.sh /usr/local/bin/vgdisplay &&     ln -s dummy.sh /usr/local/bin/pvdisplay
# Mon, 26 Jul 2021 22:23:13 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_6.6.0-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=9b196cd7be81d7d6b179838e9d30164fdb7a1f27e96678e61e24e9fe5c93f559 CB_VERSION=6.6.0
RUN chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl
# Mon, 26 Jul 2021 22:23:13 GMT
COPY file:d816a67f62bfba76d2812cefbe92252afa13f3852775c3e68599df7741e90cb7 in / 
# Mon, 26 Jul 2021 22:23:13 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 26 Jul 2021 22:23:14 GMT
CMD ["couchbase-server"]
# Mon, 26 Jul 2021 22:23:14 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Mon, 26 Jul 2021 22:23:14 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:feac5306138255e28a9862d3f3d29025d0a4d0648855afe1acd6131af07138ac`  
		Last Modified: Mon, 26 Jul 2021 21:22:52 GMT  
		Size: 26.7 MB (26709039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2a4e30704289595ec4268563ba339f4be2e264b88e79d255b680ccc550789ba`  
		Last Modified: Mon, 26 Jul 2021 22:41:09 GMT  
		Size: 7.4 MB (7373152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61d99bab81201d5c70f8e51f9f400575173f81ff7b28365411dc726bd35ec58d`  
		Last Modified: Mon, 26 Jul 2021 22:41:05 GMT  
		Size: 266.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c19a3ff870dc5ba081bf7d1af748df9148879de3770eedbd347b181ba4418c79`  
		Last Modified: Mon, 26 Jul 2021 22:41:05 GMT  
		Size: 2.0 KB (1959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f382ce40a4c6276945dbeef635ef708db6059159d9cd4a3425a74b617526260`  
		Last Modified: Mon, 26 Jul 2021 22:41:43 GMT  
		Size: 320.0 MB (320018160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3c2b9b12ebfafd8910844e882c5402810c40d25ab0db6e3d5820fd0caf23ecd`  
		Last Modified: Mon, 26 Jul 2021 22:41:04 GMT  
		Size: 191.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a47da75ba54f0fd4481a18770a6976b47209fae9e9cfd864555a2cc9c008f14f`  
		Last Modified: Mon, 26 Jul 2021 22:41:04 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:279f16369c32576b89b9cb15e9bd6cdcae6e87c10488a78576e3aaebfbcc8a05`  
		Last Modified: Mon, 26 Jul 2021 22:41:02 GMT  
		Size: 281.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbc3de5a1ae1dcb40c884fe38811c4ddec5f9a69fc46ac0baa1600c5eddf1840`  
		Last Modified: Mon, 26 Jul 2021 22:41:02 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7af87bf9317c38c511c9e1d45f577b67286e9e32b9cf9e7f11477850fc3400c2`  
		Last Modified: Mon, 26 Jul 2021 22:41:02 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d103e2a72cbd3696decc19440714d165b3ba00fe9bb3b598d2f5ff90d8972a99`  
		Last Modified: Mon, 26 Jul 2021 22:41:02 GMT  
		Size: 118.2 KB (118192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b30a84cb279ced42a19136d7a67ce9cfa512a52dd859792f4d93e2c4b605d95a`  
		Last Modified: Mon, 26 Jul 2021 22:41:02 GMT  
		Size: 858.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchbase:community-6.5.0`

```console
$ docker pull couchbase@sha256:6996aaadfba2debfe1463348b8bc8bc089f31aa733e59822745cec88098ae290
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `couchbase:community-6.5.0` - linux; amd64

```console
$ docker pull couchbase@sha256:5bde6d71c2f2b5ea8b192e833dd73cb9bf582c2da6f4cc2ff6317d37890064ab
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **351.6 MB (351615437 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d5796eb2656031f98be50a78c78ed9f59f591997b9125171d032a21b481bd6bb`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Mon, 26 Jul 2021 21:21:30 GMT
ADD file:e729fb032bd2f7cde20fb343da0cd358447e8b23028422c123944e8d0be660fa in / 
# Mon, 26 Jul 2021 21:21:31 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 22:21:49 GMT
LABEL maintainer=docker@couchbase.com
# Mon, 26 Jul 2021 22:22:25 GMT
RUN set -x &&     apt-get update &&     apt-get install -yq runit wget chrpath tzdata man     lsof lshw sysstat net-tools numactl bzip2 &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Mon, 26 Jul 2021 22:22:26 GMT
RUN if [ ! -x /usr/sbin/runsvdir-start ]; then         cp -a /etc/runit/2 /usr/sbin/runsvdir-start;     fi
# Mon, 26 Jul 2021 22:28:01 GMT
ARG CB_VERSION=6.5.1
# Mon, 26 Jul 2021 22:28:01 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/6.5.1
# Mon, 26 Jul 2021 22:35:38 GMT
ARG CB_PACKAGE=couchbase-server-community_6.5.1-ubuntu18.04_amd64.deb
# Mon, 26 Jul 2021 22:35:38 GMT
ARG CB_SHA256=c4951cdab01759020444e4648023721ae3a333257591252475d34d5fc6ac8857
# Mon, 26 Jul 2021 22:35:39 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Mon, 26 Jul 2021 22:35:39 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_6.5.1-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.5.1 CB_SHA256=c4951cdab01759020444e4648023721ae3a333257591252475d34d5fc6ac8857 CB_VERSION=6.5.1
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Mon, 26 Jul 2021 22:36:24 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_6.5.1-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.5.1 CB_SHA256=c4951cdab01759020444e4648023721ae3a333257591252475d34d5fc6ac8857 CB_VERSION=6.5.1
RUN set -x &&     export INSTALL_DONT_START_SERVER=1 &&     wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE &&     echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - &&     apt-get update &&     apt-get install -y ./$CB_PACKAGE &&     rm -f ./$CB_PACKAGE &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Mon, 26 Jul 2021 22:36:27 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_6.5.1-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.5.1 CB_SHA256=c4951cdab01759020444e4648023721ae3a333257591252475d34d5fc6ac8857 CB_VERSION=6.5.1
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Mon, 26 Jul 2021 22:36:27 GMT
COPY file:d6a307209223b2df102f46f07fd186e09fac7114db2c965bb54097d3b4d3b989 in /etc/service/couchbase-server/run 
# Mon, 26 Jul 2021 22:36:28 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_6.5.1-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.5.1 CB_SHA256=c4951cdab01759020444e4648023721ae3a333257591252475d34d5fc6ac8857 CB_VERSION=6.5.1
RUN mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Mon, 26 Jul 2021 22:36:28 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Mon, 26 Jul 2021 22:36:29 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_6.5.1-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.5.1 CB_SHA256=c4951cdab01759020444e4648023721ae3a333257591252475d34d5fc6ac8857 CB_VERSION=6.5.1
RUN ln -s dummy.sh /usr/local/bin/iptables-save &&     ln -s dummy.sh /usr/local/bin/lvdisplay &&     ln -s dummy.sh /usr/local/bin/vgdisplay &&     ln -s dummy.sh /usr/local/bin/pvdisplay
# Mon, 26 Jul 2021 22:36:29 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_6.5.1-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.5.1 CB_SHA256=c4951cdab01759020444e4648023721ae3a333257591252475d34d5fc6ac8857 CB_VERSION=6.5.1
RUN chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl
# Mon, 26 Jul 2021 22:36:29 GMT
COPY file:d816a67f62bfba76d2812cefbe92252afa13f3852775c3e68599df7741e90cb7 in / 
# Mon, 26 Jul 2021 22:36:30 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 26 Jul 2021 22:36:30 GMT
CMD ["couchbase-server"]
# Mon, 26 Jul 2021 22:36:30 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Mon, 26 Jul 2021 22:36:30 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:feac5306138255e28a9862d3f3d29025d0a4d0648855afe1acd6131af07138ac`  
		Last Modified: Mon, 26 Jul 2021 21:22:52 GMT  
		Size: 26.7 MB (26709039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2a4e30704289595ec4268563ba339f4be2e264b88e79d255b680ccc550789ba`  
		Last Modified: Mon, 26 Jul 2021 22:41:09 GMT  
		Size: 7.4 MB (7373152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61d99bab81201d5c70f8e51f9f400575173f81ff7b28365411dc726bd35ec58d`  
		Last Modified: Mon, 26 Jul 2021 22:41:05 GMT  
		Size: 266.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30423f654cdfd5e40fb198ec2c0e911221bbeeb506af261abcd36b4a350e3af3`  
		Last Modified: Mon, 26 Jul 2021 22:52:35 GMT  
		Size: 2.0 KB (1964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce425e0082c261fae710fbf0ab2083a3c955eeb8aa13be6724e56bd5caa36499`  
		Last Modified: Mon, 26 Jul 2021 22:53:17 GMT  
		Size: 317.4 MB (317410567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d5c23528392bf6b7c935d1c19ef2f5d563e324a5ee42f47289fb6687332c2d3`  
		Last Modified: Mon, 26 Jul 2021 22:52:36 GMT  
		Size: 190.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a191b25677a9be068f9a59e3c3133ff85a14bea33e9d61eee2d35dca4f53e341`  
		Last Modified: Mon, 26 Jul 2021 22:52:35 GMT  
		Size: 480.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a72316fdb86b89d274d5cd1381e0bfe51af3473c2eea60110c7ef2f827587665`  
		Last Modified: Mon, 26 Jul 2021 22:52:33 GMT  
		Size: 279.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a4540266f8a024678919ed73b495f71768526a1be1d558ac7513965b1b3de47`  
		Last Modified: Mon, 26 Jul 2021 22:52:33 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8199cd188e19b9887a258dfe4f93e0851df20b086a29d36b5efc847eba11617`  
		Last Modified: Mon, 26 Jul 2021 22:52:33 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cba5b6cbf3404bb36c78fed1ef57673051054d74435976f18a9a31a69b4ae01`  
		Last Modified: Mon, 26 Jul 2021 22:52:33 GMT  
		Size: 118.2 KB (118188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8387f9b6be487cb23bf270882f73fa8950dab7fe973c07ff9e23eb516e034059`  
		Last Modified: Mon, 26 Jul 2021 22:52:33 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchbase:community-6.5.1`

```console
$ docker pull couchbase@sha256:6996aaadfba2debfe1463348b8bc8bc089f31aa733e59822745cec88098ae290
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `couchbase:community-6.5.1` - linux; amd64

```console
$ docker pull couchbase@sha256:5bde6d71c2f2b5ea8b192e833dd73cb9bf582c2da6f4cc2ff6317d37890064ab
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **351.6 MB (351615437 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d5796eb2656031f98be50a78c78ed9f59f591997b9125171d032a21b481bd6bb`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Mon, 26 Jul 2021 21:21:30 GMT
ADD file:e729fb032bd2f7cde20fb343da0cd358447e8b23028422c123944e8d0be660fa in / 
# Mon, 26 Jul 2021 21:21:31 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 22:21:49 GMT
LABEL maintainer=docker@couchbase.com
# Mon, 26 Jul 2021 22:22:25 GMT
RUN set -x &&     apt-get update &&     apt-get install -yq runit wget chrpath tzdata man     lsof lshw sysstat net-tools numactl bzip2 &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Mon, 26 Jul 2021 22:22:26 GMT
RUN if [ ! -x /usr/sbin/runsvdir-start ]; then         cp -a /etc/runit/2 /usr/sbin/runsvdir-start;     fi
# Mon, 26 Jul 2021 22:28:01 GMT
ARG CB_VERSION=6.5.1
# Mon, 26 Jul 2021 22:28:01 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/6.5.1
# Mon, 26 Jul 2021 22:35:38 GMT
ARG CB_PACKAGE=couchbase-server-community_6.5.1-ubuntu18.04_amd64.deb
# Mon, 26 Jul 2021 22:35:38 GMT
ARG CB_SHA256=c4951cdab01759020444e4648023721ae3a333257591252475d34d5fc6ac8857
# Mon, 26 Jul 2021 22:35:39 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Mon, 26 Jul 2021 22:35:39 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_6.5.1-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.5.1 CB_SHA256=c4951cdab01759020444e4648023721ae3a333257591252475d34d5fc6ac8857 CB_VERSION=6.5.1
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Mon, 26 Jul 2021 22:36:24 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_6.5.1-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.5.1 CB_SHA256=c4951cdab01759020444e4648023721ae3a333257591252475d34d5fc6ac8857 CB_VERSION=6.5.1
RUN set -x &&     export INSTALL_DONT_START_SERVER=1 &&     wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE &&     echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - &&     apt-get update &&     apt-get install -y ./$CB_PACKAGE &&     rm -f ./$CB_PACKAGE &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Mon, 26 Jul 2021 22:36:27 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_6.5.1-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.5.1 CB_SHA256=c4951cdab01759020444e4648023721ae3a333257591252475d34d5fc6ac8857 CB_VERSION=6.5.1
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Mon, 26 Jul 2021 22:36:27 GMT
COPY file:d6a307209223b2df102f46f07fd186e09fac7114db2c965bb54097d3b4d3b989 in /etc/service/couchbase-server/run 
# Mon, 26 Jul 2021 22:36:28 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_6.5.1-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.5.1 CB_SHA256=c4951cdab01759020444e4648023721ae3a333257591252475d34d5fc6ac8857 CB_VERSION=6.5.1
RUN mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Mon, 26 Jul 2021 22:36:28 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Mon, 26 Jul 2021 22:36:29 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_6.5.1-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.5.1 CB_SHA256=c4951cdab01759020444e4648023721ae3a333257591252475d34d5fc6ac8857 CB_VERSION=6.5.1
RUN ln -s dummy.sh /usr/local/bin/iptables-save &&     ln -s dummy.sh /usr/local/bin/lvdisplay &&     ln -s dummy.sh /usr/local/bin/vgdisplay &&     ln -s dummy.sh /usr/local/bin/pvdisplay
# Mon, 26 Jul 2021 22:36:29 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_6.5.1-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.5.1 CB_SHA256=c4951cdab01759020444e4648023721ae3a333257591252475d34d5fc6ac8857 CB_VERSION=6.5.1
RUN chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl
# Mon, 26 Jul 2021 22:36:29 GMT
COPY file:d816a67f62bfba76d2812cefbe92252afa13f3852775c3e68599df7741e90cb7 in / 
# Mon, 26 Jul 2021 22:36:30 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 26 Jul 2021 22:36:30 GMT
CMD ["couchbase-server"]
# Mon, 26 Jul 2021 22:36:30 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Mon, 26 Jul 2021 22:36:30 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:feac5306138255e28a9862d3f3d29025d0a4d0648855afe1acd6131af07138ac`  
		Last Modified: Mon, 26 Jul 2021 21:22:52 GMT  
		Size: 26.7 MB (26709039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2a4e30704289595ec4268563ba339f4be2e264b88e79d255b680ccc550789ba`  
		Last Modified: Mon, 26 Jul 2021 22:41:09 GMT  
		Size: 7.4 MB (7373152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61d99bab81201d5c70f8e51f9f400575173f81ff7b28365411dc726bd35ec58d`  
		Last Modified: Mon, 26 Jul 2021 22:41:05 GMT  
		Size: 266.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30423f654cdfd5e40fb198ec2c0e911221bbeeb506af261abcd36b4a350e3af3`  
		Last Modified: Mon, 26 Jul 2021 22:52:35 GMT  
		Size: 2.0 KB (1964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce425e0082c261fae710fbf0ab2083a3c955eeb8aa13be6724e56bd5caa36499`  
		Last Modified: Mon, 26 Jul 2021 22:53:17 GMT  
		Size: 317.4 MB (317410567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d5c23528392bf6b7c935d1c19ef2f5d563e324a5ee42f47289fb6687332c2d3`  
		Last Modified: Mon, 26 Jul 2021 22:52:36 GMT  
		Size: 190.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a191b25677a9be068f9a59e3c3133ff85a14bea33e9d61eee2d35dca4f53e341`  
		Last Modified: Mon, 26 Jul 2021 22:52:35 GMT  
		Size: 480.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a72316fdb86b89d274d5cd1381e0bfe51af3473c2eea60110c7ef2f827587665`  
		Last Modified: Mon, 26 Jul 2021 22:52:33 GMT  
		Size: 279.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a4540266f8a024678919ed73b495f71768526a1be1d558ac7513965b1b3de47`  
		Last Modified: Mon, 26 Jul 2021 22:52:33 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8199cd188e19b9887a258dfe4f93e0851df20b086a29d36b5efc847eba11617`  
		Last Modified: Mon, 26 Jul 2021 22:52:33 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cba5b6cbf3404bb36c78fed1ef57673051054d74435976f18a9a31a69b4ae01`  
		Last Modified: Mon, 26 Jul 2021 22:52:33 GMT  
		Size: 118.2 KB (118188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8387f9b6be487cb23bf270882f73fa8950dab7fe973c07ff9e23eb516e034059`  
		Last Modified: Mon, 26 Jul 2021 22:52:33 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchbase:community-6.6.0`

```console
$ docker pull couchbase@sha256:b0baeef769e4ba8fab7ac8e0a78416a009de893fb3d6bf9c1dcbb75130fd004c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `couchbase:community-6.6.0` - linux; amd64

```console
$ docker pull couchbase@sha256:610c0d832bdb7e0144b88a509c9b857bf1551ae55572450dee2e2515eba3b313
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **354.2 MB (354223029 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b2ef0dbd9aca1cefb55ddecf92c830dda7d3d252e86f4a7511de382b757502e`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Mon, 26 Jul 2021 21:21:30 GMT
ADD file:e729fb032bd2f7cde20fb343da0cd358447e8b23028422c123944e8d0be660fa in / 
# Mon, 26 Jul 2021 21:21:31 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 22:21:49 GMT
LABEL maintainer=docker@couchbase.com
# Mon, 26 Jul 2021 22:22:25 GMT
RUN set -x &&     apt-get update &&     apt-get install -yq runit wget chrpath tzdata man     lsof lshw sysstat net-tools numactl bzip2 &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Mon, 26 Jul 2021 22:22:26 GMT
RUN if [ ! -x /usr/sbin/runsvdir-start ]; then         cp -a /etc/runit/2 /usr/sbin/runsvdir-start;     fi
# Mon, 26 Jul 2021 22:22:27 GMT
ARG CB_VERSION=6.6.0
# Mon, 26 Jul 2021 22:22:27 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0
# Mon, 26 Jul 2021 22:22:27 GMT
ARG CB_PACKAGE=couchbase-server-community_6.6.0-ubuntu18.04_amd64.deb
# Mon, 26 Jul 2021 22:22:27 GMT
ARG CB_SHA256=9b196cd7be81d7d6b179838e9d30164fdb7a1f27e96678e61e24e9fe5c93f559
# Mon, 26 Jul 2021 22:22:28 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Mon, 26 Jul 2021 22:22:28 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_6.6.0-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=9b196cd7be81d7d6b179838e9d30164fdb7a1f27e96678e61e24e9fe5c93f559 CB_VERSION=6.6.0
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Mon, 26 Jul 2021 22:23:07 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_6.6.0-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=9b196cd7be81d7d6b179838e9d30164fdb7a1f27e96678e61e24e9fe5c93f559 CB_VERSION=6.6.0
RUN set -x &&     export INSTALL_DONT_START_SERVER=1 &&     wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE &&     echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - &&     apt-get update &&     apt-get install -y ./$CB_PACKAGE &&     rm -f ./$CB_PACKAGE &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Mon, 26 Jul 2021 22:23:10 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_6.6.0-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=9b196cd7be81d7d6b179838e9d30164fdb7a1f27e96678e61e24e9fe5c93f559 CB_VERSION=6.6.0
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Mon, 26 Jul 2021 22:23:10 GMT
COPY file:d6a307209223b2df102f46f07fd186e09fac7114db2c965bb54097d3b4d3b989 in /etc/service/couchbase-server/run 
# Mon, 26 Jul 2021 22:23:11 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_6.6.0-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=9b196cd7be81d7d6b179838e9d30164fdb7a1f27e96678e61e24e9fe5c93f559 CB_VERSION=6.6.0
RUN mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Mon, 26 Jul 2021 22:23:11 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Mon, 26 Jul 2021 22:23:12 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_6.6.0-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=9b196cd7be81d7d6b179838e9d30164fdb7a1f27e96678e61e24e9fe5c93f559 CB_VERSION=6.6.0
RUN ln -s dummy.sh /usr/local/bin/iptables-save &&     ln -s dummy.sh /usr/local/bin/lvdisplay &&     ln -s dummy.sh /usr/local/bin/vgdisplay &&     ln -s dummy.sh /usr/local/bin/pvdisplay
# Mon, 26 Jul 2021 22:23:13 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_6.6.0-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=9b196cd7be81d7d6b179838e9d30164fdb7a1f27e96678e61e24e9fe5c93f559 CB_VERSION=6.6.0
RUN chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl
# Mon, 26 Jul 2021 22:23:13 GMT
COPY file:d816a67f62bfba76d2812cefbe92252afa13f3852775c3e68599df7741e90cb7 in / 
# Mon, 26 Jul 2021 22:23:13 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 26 Jul 2021 22:23:14 GMT
CMD ["couchbase-server"]
# Mon, 26 Jul 2021 22:23:14 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Mon, 26 Jul 2021 22:23:14 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:feac5306138255e28a9862d3f3d29025d0a4d0648855afe1acd6131af07138ac`  
		Last Modified: Mon, 26 Jul 2021 21:22:52 GMT  
		Size: 26.7 MB (26709039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2a4e30704289595ec4268563ba339f4be2e264b88e79d255b680ccc550789ba`  
		Last Modified: Mon, 26 Jul 2021 22:41:09 GMT  
		Size: 7.4 MB (7373152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61d99bab81201d5c70f8e51f9f400575173f81ff7b28365411dc726bd35ec58d`  
		Last Modified: Mon, 26 Jul 2021 22:41:05 GMT  
		Size: 266.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c19a3ff870dc5ba081bf7d1af748df9148879de3770eedbd347b181ba4418c79`  
		Last Modified: Mon, 26 Jul 2021 22:41:05 GMT  
		Size: 2.0 KB (1959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f382ce40a4c6276945dbeef635ef708db6059159d9cd4a3425a74b617526260`  
		Last Modified: Mon, 26 Jul 2021 22:41:43 GMT  
		Size: 320.0 MB (320018160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3c2b9b12ebfafd8910844e882c5402810c40d25ab0db6e3d5820fd0caf23ecd`  
		Last Modified: Mon, 26 Jul 2021 22:41:04 GMT  
		Size: 191.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a47da75ba54f0fd4481a18770a6976b47209fae9e9cfd864555a2cc9c008f14f`  
		Last Modified: Mon, 26 Jul 2021 22:41:04 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:279f16369c32576b89b9cb15e9bd6cdcae6e87c10488a78576e3aaebfbcc8a05`  
		Last Modified: Mon, 26 Jul 2021 22:41:02 GMT  
		Size: 281.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbc3de5a1ae1dcb40c884fe38811c4ddec5f9a69fc46ac0baa1600c5eddf1840`  
		Last Modified: Mon, 26 Jul 2021 22:41:02 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7af87bf9317c38c511c9e1d45f577b67286e9e32b9cf9e7f11477850fc3400c2`  
		Last Modified: Mon, 26 Jul 2021 22:41:02 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d103e2a72cbd3696decc19440714d165b3ba00fe9bb3b598d2f5ff90d8972a99`  
		Last Modified: Mon, 26 Jul 2021 22:41:02 GMT  
		Size: 118.2 KB (118192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b30a84cb279ced42a19136d7a67ce9cfa512a52dd859792f4d93e2c4b605d95a`  
		Last Modified: Mon, 26 Jul 2021 22:41:02 GMT  
		Size: 858.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchbase:community-7.0.0-beta`

```console
$ docker pull couchbase@sha256:3d218fab74b022a627c3194f7d2115c1b71671743b0cd14fe397c0a90d778d74
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `couchbase:community-7.0.0-beta` - linux; amd64

```console
$ docker pull couchbase@sha256:750b7ca28f31e128470ccc511739d8b479a638ae2ed55223a26211b4c83800f1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **434.0 MB (434035245 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:35736c7516be0f482a3db69eca2529525732a0551479922b728f13b87e18d2b3`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Mon, 26 Jul 2021 21:21:39 GMT
ADD file:524e8d93ad65f08a0cb0d144268350186e36f508006b05b8faf2e1289499b59f in / 
# Mon, 26 Jul 2021 21:21:40 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 22:17:12 GMT
LABEL maintainer=docker@couchbase.com
# Mon, 26 Jul 2021 22:17:38 GMT
RUN set -x &&     apt-get update &&     apt-get install -yq runit wget chrpath tzdata man     lsof lshw sysstat net-tools numactl bzip2 &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Mon, 26 Jul 2021 22:17:39 GMT
RUN if [ ! -x /usr/sbin/runsvdir-start ]; then         cp -a /etc/runit/2 /usr/sbin/runsvdir-start;     fi
# Mon, 26 Jul 2021 22:17:39 GMT
ARG CB_VERSION=7.0.0-beta
# Mon, 26 Jul 2021 22:17:39 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.0-beta
# Mon, 26 Jul 2021 22:19:23 GMT
ARG CB_PACKAGE=couchbase-server-community_7.0.0-beta-ubuntu20.04_amd64.deb
# Mon, 26 Jul 2021 22:19:23 GMT
ARG CB_SHA256=51e843e9d2b5ef746353d79c044f17e4f9be0866673bd6fda01da27a0edf9fc9
# Mon, 26 Jul 2021 22:19:23 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Mon, 26 Jul 2021 22:19:24 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.0.0-beta-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.0-beta CB_SHA256=51e843e9d2b5ef746353d79c044f17e4f9be0866673bd6fda01da27a0edf9fc9 CB_VERSION=7.0.0-beta
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Mon, 26 Jul 2021 22:20:15 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.0.0-beta-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.0-beta CB_SHA256=51e843e9d2b5ef746353d79c044f17e4f9be0866673bd6fda01da27a0edf9fc9 CB_VERSION=7.0.0-beta
RUN set -x &&     export INSTALL_DONT_START_SERVER=1 &&     wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE &&     echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - &&     apt-get update &&     apt-get install -y ./$CB_PACKAGE &&     rm -f ./$CB_PACKAGE &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Mon, 26 Jul 2021 22:20:16 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.0.0-beta-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.0-beta CB_SHA256=51e843e9d2b5ef746353d79c044f17e4f9be0866673bd6fda01da27a0edf9fc9 CB_VERSION=7.0.0-beta
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Mon, 26 Jul 2021 22:20:17 GMT
COPY file:d6a307209223b2df102f46f07fd186e09fac7114db2c965bb54097d3b4d3b989 in /etc/service/couchbase-server/run 
# Mon, 26 Jul 2021 22:20:17 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.0.0-beta-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.0-beta CB_SHA256=51e843e9d2b5ef746353d79c044f17e4f9be0866673bd6fda01da27a0edf9fc9 CB_VERSION=7.0.0-beta
RUN mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Mon, 26 Jul 2021 22:20:18 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Mon, 26 Jul 2021 22:20:18 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.0.0-beta-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.0-beta CB_SHA256=51e843e9d2b5ef746353d79c044f17e4f9be0866673bd6fda01da27a0edf9fc9 CB_VERSION=7.0.0-beta
RUN ln -s dummy.sh /usr/local/bin/iptables-save &&     ln -s dummy.sh /usr/local/bin/lvdisplay &&     ln -s dummy.sh /usr/local/bin/vgdisplay &&     ln -s dummy.sh /usr/local/bin/pvdisplay
# Mon, 26 Jul 2021 22:20:19 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.0.0-beta-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.0-beta CB_SHA256=51e843e9d2b5ef746353d79c044f17e4f9be0866673bd6fda01da27a0edf9fc9 CB_VERSION=7.0.0-beta
RUN chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl
# Mon, 26 Jul 2021 22:20:19 GMT
COPY file:d816a67f62bfba76d2812cefbe92252afa13f3852775c3e68599df7741e90cb7 in / 
# Mon, 26 Jul 2021 22:20:20 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 26 Jul 2021 22:20:20 GMT
CMD ["couchbase-server"]
# Mon, 26 Jul 2021 22:20:20 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Mon, 26 Jul 2021 22:20:20 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:16ec32c2132b43494832a05f2b02f7a822479f8250c173d0ab27b3de78b2f058`  
		Last Modified: Sun, 25 Jul 2021 03:03:29 GMT  
		Size: 28.6 MB (28567944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0f4f47bb294f3f6f2dc58514a7dc33b42f8be77cfbbed0dbd1c8a49fca73899`  
		Last Modified: Mon, 26 Jul 2021 22:37:21 GMT  
		Size: 8.3 MB (8287040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e87aaeab53b206101d3fd9751a01810367e7cc684b3636f34e03abd4eec34d3`  
		Last Modified: Mon, 26 Jul 2021 22:37:16 GMT  
		Size: 264.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05de0d37fcdab8c05f8d3dd601550fc44c5c0e54b6027e76be01605072d25f3e`  
		Last Modified: Mon, 26 Jul 2021 22:38:44 GMT  
		Size: 1.8 KB (1836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78abeee70f0cc7e3e35c5ed80e40f7612792abc932284492ed6c2c802c340eb8`  
		Last Modified: Mon, 26 Jul 2021 22:39:34 GMT  
		Size: 397.1 MB (397050011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7de4d4e366a7166ca9ef87fce398afc0a32a043312b48f04dc6cb610eb11cdee`  
		Last Modified: Mon, 26 Jul 2021 22:38:43 GMT  
		Size: 190.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a70a0f3192b9077e9284a28b1896af9be5ca542980d79c396dafa444a6d6cc5a`  
		Last Modified: Mon, 26 Jul 2021 22:38:43 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e3c34d79cdefc0f392c68809bbde60510c2fa628a3af489e85cab9adb33dc9d`  
		Last Modified: Mon, 26 Jul 2021 22:38:41 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55e2c19437f1927a72d3ed739f4c645e1c564ae8d5eb86ebbc64edf737c16e38`  
		Last Modified: Mon, 26 Jul 2021 22:38:41 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c05f18bb421175ddc6769a78668676af2ba2256d8db516c91a1fb179c4bff95`  
		Last Modified: Mon, 26 Jul 2021 22:38:41 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18692f0cd41deeed250c209cad249e1a9d0ee8328e02555e9dbfea028baf8801`  
		Last Modified: Mon, 26 Jul 2021 22:38:41 GMT  
		Size: 125.9 KB (125893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3135664970050d0f698227c0745afda1c4706fb89a96b3e58534bc174e1ad1b`  
		Last Modified: Mon, 26 Jul 2021 22:38:41 GMT  
		Size: 858.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchbase:enterprise`

```console
$ docker pull couchbase@sha256:9e6e9947a937f0e1d692deb0276131e10f0f12a8fd469e33d30fdd6b6a658c73
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `couchbase:enterprise` - linux; amd64

```console
$ docker pull couchbase@sha256:2befadeed5bbfd07b657995c9432dad470840d4b32d8757c4de44f1f8bdb0bf6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **533.2 MB (533222654 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89c4c1a0b656b1893a5cc9277f0a39ac1771db24a19fcb5cd17e2c96f5b6f01d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Mon, 26 Jul 2021 21:21:39 GMT
ADD file:524e8d93ad65f08a0cb0d144268350186e36f508006b05b8faf2e1289499b59f in / 
# Mon, 26 Jul 2021 21:21:40 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 22:17:12 GMT
LABEL maintainer=docker@couchbase.com
# Mon, 26 Jul 2021 22:20:33 GMT
RUN set -x &&     apt-get update &&     apt-get install -yq runit wget chrpath tzdata     lsof lshw sysstat net-tools numactl bzip2 &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Mon, 26 Jul 2021 22:20:33 GMT
RUN if [ ! -x /usr/sbin/runsvdir-start ]; then         cp -a /etc/runit/2 /usr/sbin/runsvdir-start;     fi
# Mon, 26 Jul 2021 22:20:34 GMT
ARG CB_VERSION=6.6.2
# Mon, 26 Jul 2021 22:20:34 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.2
# Mon, 26 Jul 2021 22:20:34 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_6.6.2-ubuntu20.04_amd64.deb
# Mon, 26 Jul 2021 22:20:34 GMT
ARG CB_SHA256=41c033e6c1e98b0844a5cb5768e3769e7012d8374a6bd235c86e10db33b17afc
# Mon, 26 Jul 2021 22:20:34 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Mon, 26 Jul 2021 22:20:35 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.2-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.2 CB_SHA256=41c033e6c1e98b0844a5cb5768e3769e7012d8374a6bd235c86e10db33b17afc CB_VERSION=6.6.2
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Mon, 26 Jul 2021 22:21:31 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.2-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.2 CB_SHA256=41c033e6c1e98b0844a5cb5768e3769e7012d8374a6bd235c86e10db33b17afc CB_VERSION=6.6.2
RUN set -x &&     export INSTALL_DONT_START_SERVER=1 &&     wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE &&     echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - &&     apt-get update &&     apt-get install -y ./$CB_PACKAGE &&     rm -f ./$CB_PACKAGE &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Mon, 26 Jul 2021 22:21:35 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.2-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.2 CB_SHA256=41c033e6c1e98b0844a5cb5768e3769e7012d8374a6bd235c86e10db33b17afc CB_VERSION=6.6.2
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Mon, 26 Jul 2021 22:21:35 GMT
COPY file:d6a307209223b2df102f46f07fd186e09fac7114db2c965bb54097d3b4d3b989 in /etc/service/couchbase-server/run 
# Mon, 26 Jul 2021 22:21:36 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.2-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.2 CB_SHA256=41c033e6c1e98b0844a5cb5768e3769e7012d8374a6bd235c86e10db33b17afc CB_VERSION=6.6.2
RUN mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Mon, 26 Jul 2021 22:21:36 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Mon, 26 Jul 2021 22:21:37 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.2-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.2 CB_SHA256=41c033e6c1e98b0844a5cb5768e3769e7012d8374a6bd235c86e10db33b17afc CB_VERSION=6.6.2
RUN ln -s dummy.sh /usr/local/bin/iptables-save &&     ln -s dummy.sh /usr/local/bin/lvdisplay &&     ln -s dummy.sh /usr/local/bin/vgdisplay &&     ln -s dummy.sh /usr/local/bin/pvdisplay
# Mon, 26 Jul 2021 22:21:38 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.2-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.2 CB_SHA256=41c033e6c1e98b0844a5cb5768e3769e7012d8374a6bd235c86e10db33b17afc CB_VERSION=6.6.2
RUN chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl
# Mon, 26 Jul 2021 22:21:38 GMT
COPY file:d816a67f62bfba76d2812cefbe92252afa13f3852775c3e68599df7741e90cb7 in / 
# Mon, 26 Jul 2021 22:21:38 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 26 Jul 2021 22:21:38 GMT
CMD ["couchbase-server"]
# Mon, 26 Jul 2021 22:21:39 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Mon, 26 Jul 2021 22:21:39 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:16ec32c2132b43494832a05f2b02f7a822479f8250c173d0ab27b3de78b2f058`  
		Last Modified: Sun, 25 Jul 2021 03:03:29 GMT  
		Size: 28.6 MB (28567944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d887c602d6e2b416c36a7344e07f41278a46971fa08be0eeb2fc78a75d7013b`  
		Last Modified: Mon, 26 Jul 2021 22:39:49 GMT  
		Size: 6.3 MB (6272568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b219d16ecda3370190c17757e31f650c0b2db8a483364cebc0add69c976f1fa`  
		Last Modified: Mon, 26 Jul 2021 22:39:45 GMT  
		Size: 264.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:febb3fec572429eea18c02afb8a6c9879b303a8fe54f24c598d70e76284d2e50`  
		Last Modified: Mon, 26 Jul 2021 22:39:45 GMT  
		Size: 1.8 KB (1836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc966ce6300d6331c07980d729ddad541989a337e6eb174cab32a6da22196a4b`  
		Last Modified: Mon, 26 Jul 2021 22:40:42 GMT  
		Size: 498.3 MB (498251893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edb4c7a902a3d8673bde3e41bdcafb1f24b6bd970572a368d1d1c290bc0f0c5c`  
		Last Modified: Mon, 26 Jul 2021 22:39:45 GMT  
		Size: 191.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef06a70d616a9d9e24737530889d9744fa42fa92f9c293f9a47ab5046769e4e5`  
		Last Modified: Mon, 26 Jul 2021 22:39:45 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8a527aa307ea3cd1feffde8b7b71f90af3149dc21432afb9d9c9187c61017c5`  
		Last Modified: Mon, 26 Jul 2021 22:39:42 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4233c8f62d720537a74a69707dd1d651286d9bfab88848bb8d41445266481254`  
		Last Modified: Mon, 26 Jul 2021 22:39:42 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dda6ae4667566d063e0d185b915cc7fe3d16ea8dd7504aa48ae246e35db9d509`  
		Last Modified: Mon, 26 Jul 2021 22:39:42 GMT  
		Size: 217.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01243b96b0b7ddaf69634a7674356f0e483f5f24e91d57de48d161fcf28d65d0`  
		Last Modified: Mon, 26 Jul 2021 22:39:42 GMT  
		Size: 125.9 KB (125893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74aee4374d591a250acc5a5e8b2be6cacffceebba6ee89c2fe32ba3806144098`  
		Last Modified: Mon, 26 Jul 2021 22:39:42 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchbase:enterprise-6.0.1`

```console
$ docker pull couchbase@sha256:33152059c8f0325e94865257494822db62f0cbd4ea07ff54809d5c2f7220ab3b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `couchbase:enterprise-6.0.1` - linux; amd64

```console
$ docker pull couchbase@sha256:eb994494260bba67e8ad1094a0ef2f45806116a27ab2452eab59abd52854784b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **455.2 MB (455214931 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:757245717d3c5546275f8646e84cca7c4354a68d84975b5e4638c41dc58ef654`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Mon, 26 Jul 2021 21:21:30 GMT
ADD file:e729fb032bd2f7cde20fb343da0cd358447e8b23028422c123944e8d0be660fa in / 
# Mon, 26 Jul 2021 21:21:31 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 22:21:49 GMT
LABEL maintainer=docker@couchbase.com
# Mon, 26 Jul 2021 22:23:55 GMT
RUN set -x &&     apt-get update &&     apt-get install -yq runit wget chrpath tzdata man     lsof lshw sysstat net-tools numactl python-httplib2 &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Mon, 26 Jul 2021 22:23:56 GMT
RUN if [ ! -x /usr/sbin/runsvdir-start ]; then         cp -a /etc/runit/2 /usr/sbin/runsvdir-start;     fi
# Mon, 26 Jul 2021 22:34:27 GMT
ARG CB_VERSION=6.0.1
# Mon, 26 Jul 2021 22:34:27 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.1
# Mon, 26 Jul 2021 22:34:27 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_6.0.1-ubuntu18.04_amd64.deb
# Mon, 26 Jul 2021 22:34:27 GMT
ARG CB_SHA256=68deed9ba855e2a84500ae99a787c415fc85b4d4dc1140be28ae6f56662bafea
# Mon, 26 Jul 2021 22:34:28 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Mon, 26 Jul 2021 22:34:28 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.1-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.1 CB_SHA256=68deed9ba855e2a84500ae99a787c415fc85b4d4dc1140be28ae6f56662bafea CB_VERSION=6.0.1
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Mon, 26 Jul 2021 22:35:26 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.1-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.1 CB_SHA256=68deed9ba855e2a84500ae99a787c415fc85b4d4dc1140be28ae6f56662bafea CB_VERSION=6.0.1
RUN set -x &&     export INSTALL_DONT_START_SERVER=1 &&     wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE &&     echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - &&     apt-get update &&     apt-get install -y ./$CB_PACKAGE &&     rm -f ./$CB_PACKAGE &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Mon, 26 Jul 2021 22:35:29 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.1-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.1 CB_SHA256=68deed9ba855e2a84500ae99a787c415fc85b4d4dc1140be28ae6f56662bafea CB_VERSION=6.0.1
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Mon, 26 Jul 2021 22:35:29 GMT
COPY file:d6a307209223b2df102f46f07fd186e09fac7114db2c965bb54097d3b4d3b989 in /etc/service/couchbase-server/run 
# Mon, 26 Jul 2021 22:35:30 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.1-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.1 CB_SHA256=68deed9ba855e2a84500ae99a787c415fc85b4d4dc1140be28ae6f56662bafea CB_VERSION=6.0.1
RUN mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Mon, 26 Jul 2021 22:35:30 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Mon, 26 Jul 2021 22:35:31 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.1-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.1 CB_SHA256=68deed9ba855e2a84500ae99a787c415fc85b4d4dc1140be28ae6f56662bafea CB_VERSION=6.0.1
RUN ln -s dummy.sh /usr/local/bin/iptables-save &&     ln -s dummy.sh /usr/local/bin/lvdisplay &&     ln -s dummy.sh /usr/local/bin/vgdisplay &&     ln -s dummy.sh /usr/local/bin/pvdisplay
# Mon, 26 Jul 2021 22:35:32 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.1-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.1 CB_SHA256=68deed9ba855e2a84500ae99a787c415fc85b4d4dc1140be28ae6f56662bafea CB_VERSION=6.0.1
RUN chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl
# Mon, 26 Jul 2021 22:35:32 GMT
COPY file:d816a67f62bfba76d2812cefbe92252afa13f3852775c3e68599df7741e90cb7 in / 
# Mon, 26 Jul 2021 22:35:32 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 26 Jul 2021 22:35:32 GMT
CMD ["couchbase-server"]
# Mon, 26 Jul 2021 22:35:32 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Mon, 26 Jul 2021 22:35:33 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:feac5306138255e28a9862d3f3d29025d0a4d0648855afe1acd6131af07138ac`  
		Last Modified: Mon, 26 Jul 2021 21:22:52 GMT  
		Size: 26.7 MB (26709039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d34675e7dacc0ce319b39b9ea2535f805fa959a52abc54f87cc0a227b97902ca`  
		Last Modified: Mon, 26 Jul 2021 22:42:05 GMT  
		Size: 15.9 MB (15922947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:889c4fafca81882f6937a23d718195844112f8f700b2bbf19b2fed74fb78653f`  
		Last Modified: Mon, 26 Jul 2021 22:42:00 GMT  
		Size: 266.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cd2998f9f5572111f397f86320964084ff27496510b3f207f2abbd03f280290`  
		Last Modified: Mon, 26 Jul 2021 22:51:25 GMT  
		Size: 2.0 KB (1966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0be5d397f140f7be638b55fc8b192db79f2054c786d19231e732c4b739f611d1`  
		Last Modified: Mon, 26 Jul 2021 22:52:19 GMT  
		Size: 412.5 MB (412452893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03beda794fda7c5d8a531ae36fe1e3bffe5f104c2efcf68bd401eb2c5685eb6f`  
		Last Modified: Mon, 26 Jul 2021 22:51:25 GMT  
		Size: 190.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b3c1409fb418a4d13bcfd92f6c4408f3512059f0453ecee7c03f55c34ce9c52`  
		Last Modified: Mon, 26 Jul 2021 22:51:25 GMT  
		Size: 479.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d80b35c3d361b4c92cefe6a3bb490b5b7591bc5b7b392a0ae6a6f81c46c0f07`  
		Last Modified: Mon, 26 Jul 2021 22:51:22 GMT  
		Size: 280.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6de0d3e36daec3a43bdf425331781a96ac6410418cc148519da3b640f692dcb5`  
		Last Modified: Mon, 26 Jul 2021 22:51:22 GMT  
		Size: 235.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66b0ad6fef042a063da298d8a62d3eaca3d3e59fe4df6df1439e9d347bdfe701`  
		Last Modified: Mon, 26 Jul 2021 22:51:22 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c336a662e1c94b1c42448c50343c47f2afcba4e640e5b9a9e6b6331fdb8ba5bc`  
		Last Modified: Mon, 26 Jul 2021 22:51:22 GMT  
		Size: 125.6 KB (125560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6156f367f101d52bf75f7ad0fed3d8554098a13c50178a7fdac410967b50f541`  
		Last Modified: Mon, 26 Jul 2021 22:51:22 GMT  
		Size: 858.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchbase:enterprise-6.0.2`

```console
$ docker pull couchbase@sha256:75e54afa0e524c05402a044ddbf406a3d7827caea040e6719bad5be4eca55b68
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `couchbase:enterprise-6.0.2` - linux; amd64

```console
$ docker pull couchbase@sha256:b1b18cd89e7873573bab515e983b68da02cd5a3a3513dc891598c7a168baf80f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **463.4 MB (463385372 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:77588e252f19dd926cf26632e179c6108b5e4b73c031f4e77d2bebe9b8f4fb8f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Mon, 26 Jul 2021 21:21:30 GMT
ADD file:e729fb032bd2f7cde20fb343da0cd358447e8b23028422c123944e8d0be660fa in / 
# Mon, 26 Jul 2021 21:21:31 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 22:21:49 GMT
LABEL maintainer=docker@couchbase.com
# Mon, 26 Jul 2021 22:23:55 GMT
RUN set -x &&     apt-get update &&     apt-get install -yq runit wget chrpath tzdata man     lsof lshw sysstat net-tools numactl python-httplib2 &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Mon, 26 Jul 2021 22:23:56 GMT
RUN if [ ! -x /usr/sbin/runsvdir-start ]; then         cp -a /etc/runit/2 /usr/sbin/runsvdir-start;     fi
# Mon, 26 Jul 2021 22:33:15 GMT
ARG CB_VERSION=6.0.2
# Mon, 26 Jul 2021 22:33:15 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.2
# Mon, 26 Jul 2021 22:33:15 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_6.0.2-ubuntu18.04_amd64.deb
# Mon, 26 Jul 2021 22:33:16 GMT
ARG CB_SHA256=5410a56cefd7a9c624a2d64e474058b43a90e8d66c73fea6b2a8b16a4f6fe14d
# Mon, 26 Jul 2021 22:33:16 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Mon, 26 Jul 2021 22:33:17 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.2-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.2 CB_SHA256=5410a56cefd7a9c624a2d64e474058b43a90e8d66c73fea6b2a8b16a4f6fe14d CB_VERSION=6.0.2
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Mon, 26 Jul 2021 22:34:06 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.2-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.2 CB_SHA256=5410a56cefd7a9c624a2d64e474058b43a90e8d66c73fea6b2a8b16a4f6fe14d CB_VERSION=6.0.2
RUN set -x &&     export INSTALL_DONT_START_SERVER=1 &&     wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE &&     echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - &&     apt-get update &&     apt-get install -y ./$CB_PACKAGE &&     rm -f ./$CB_PACKAGE &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Mon, 26 Jul 2021 22:34:09 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.2-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.2 CB_SHA256=5410a56cefd7a9c624a2d64e474058b43a90e8d66c73fea6b2a8b16a4f6fe14d CB_VERSION=6.0.2
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Mon, 26 Jul 2021 22:34:09 GMT
COPY file:d6a307209223b2df102f46f07fd186e09fac7114db2c965bb54097d3b4d3b989 in /etc/service/couchbase-server/run 
# Mon, 26 Jul 2021 22:34:10 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.2-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.2 CB_SHA256=5410a56cefd7a9c624a2d64e474058b43a90e8d66c73fea6b2a8b16a4f6fe14d CB_VERSION=6.0.2
RUN mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Mon, 26 Jul 2021 22:34:10 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Mon, 26 Jul 2021 22:34:11 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.2-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.2 CB_SHA256=5410a56cefd7a9c624a2d64e474058b43a90e8d66c73fea6b2a8b16a4f6fe14d CB_VERSION=6.0.2
RUN ln -s dummy.sh /usr/local/bin/iptables-save &&     ln -s dummy.sh /usr/local/bin/lvdisplay &&     ln -s dummy.sh /usr/local/bin/vgdisplay &&     ln -s dummy.sh /usr/local/bin/pvdisplay
# Mon, 26 Jul 2021 22:34:12 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.2-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.2 CB_SHA256=5410a56cefd7a9c624a2d64e474058b43a90e8d66c73fea6b2a8b16a4f6fe14d CB_VERSION=6.0.2
RUN chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl
# Mon, 26 Jul 2021 22:34:12 GMT
COPY file:d816a67f62bfba76d2812cefbe92252afa13f3852775c3e68599df7741e90cb7 in / 
# Mon, 26 Jul 2021 22:34:12 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 26 Jul 2021 22:34:13 GMT
CMD ["couchbase-server"]
# Mon, 26 Jul 2021 22:34:13 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Mon, 26 Jul 2021 22:34:13 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:feac5306138255e28a9862d3f3d29025d0a4d0648855afe1acd6131af07138ac`  
		Last Modified: Mon, 26 Jul 2021 21:22:52 GMT  
		Size: 26.7 MB (26709039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d34675e7dacc0ce319b39b9ea2535f805fa959a52abc54f87cc0a227b97902ca`  
		Last Modified: Mon, 26 Jul 2021 22:42:05 GMT  
		Size: 15.9 MB (15922947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:889c4fafca81882f6937a23d718195844112f8f700b2bbf19b2fed74fb78653f`  
		Last Modified: Mon, 26 Jul 2021 22:42:00 GMT  
		Size: 266.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ccbcd2e67fd23c9ce7d7ab437d3161706d77a58d568a561dfe8357941eb827e`  
		Last Modified: Mon, 26 Jul 2021 22:50:17 GMT  
		Size: 2.0 KB (1969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a04c3b3ac89e401a3308e91d824719413d8725c6c9ae6d080e1b15cce870804c`  
		Last Modified: Mon, 26 Jul 2021 22:51:07 GMT  
		Size: 420.6 MB (420623327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:911f235b902b36060bc6990a33dce8c0fde76524fe367541939d358ea170595f`  
		Last Modified: Mon, 26 Jul 2021 22:50:16 GMT  
		Size: 191.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c373fecd0c59a07b716080a9e68e5e33ba3fbcb68698852bb2fbcf98e9e0c592`  
		Last Modified: Mon, 26 Jul 2021 22:50:17 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba043cf248186fe7ae560b1556698d5006aa2f71713f396ec964adb8ccf2098c`  
		Last Modified: Mon, 26 Jul 2021 22:50:14 GMT  
		Size: 282.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21441055e9c64021a41a16a2d5dc1efaa9e80c27853dfef40c86594ab9ea4d26`  
		Last Modified: Mon, 26 Jul 2021 22:50:15 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48658a61d80a00eee7991e5c6bc658379847dd9db3ebacd002fb5d881f94aace`  
		Last Modified: Mon, 26 Jul 2021 22:50:14 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:198b0c45eef48b37a9785387ce7bf1cb422308e09d6c5ec63e68bbd7ba4d8c34`  
		Last Modified: Mon, 26 Jul 2021 22:50:14 GMT  
		Size: 125.6 KB (125560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e368762e925c7afc1beaeadd64157a36bfac082cfa2474c5ba50a277b5952c1`  
		Last Modified: Mon, 26 Jul 2021 22:50:14 GMT  
		Size: 858.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchbase:enterprise-6.0.3`

```console
$ docker pull couchbase@sha256:aad83db3e30dd7a658b016f9b1157063654b924dbd78d385ed8192b80bc059b6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `couchbase:enterprise-6.0.3` - linux; amd64

```console
$ docker pull couchbase@sha256:236438660ddd6a6beaf2d79ed57c8d325d6df7493a954d3585d7c1bee02d39d0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **465.9 MB (465909384 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e8b5672ad5d70ccadfb70f377d3997ae77d77db04e470a752a8e1e79215e58b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Mon, 26 Jul 2021 21:21:30 GMT
ADD file:e729fb032bd2f7cde20fb343da0cd358447e8b23028422c123944e8d0be660fa in / 
# Mon, 26 Jul 2021 21:21:31 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 22:21:49 GMT
LABEL maintainer=docker@couchbase.com
# Mon, 26 Jul 2021 22:23:55 GMT
RUN set -x &&     apt-get update &&     apt-get install -yq runit wget chrpath tzdata man     lsof lshw sysstat net-tools numactl python-httplib2 &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Mon, 26 Jul 2021 22:23:56 GMT
RUN if [ ! -x /usr/sbin/runsvdir-start ]; then         cp -a /etc/runit/2 /usr/sbin/runsvdir-start;     fi
# Mon, 26 Jul 2021 22:32:03 GMT
ARG CB_VERSION=6.0.3
# Mon, 26 Jul 2021 22:32:04 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.3
# Mon, 26 Jul 2021 22:32:04 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_6.0.3-ubuntu18.04_amd64.deb
# Mon, 26 Jul 2021 22:32:04 GMT
ARG CB_SHA256=8ee814ea8d99141de5493a6a24423c6a5dc4e01b8393dce87ca1639630315382
# Mon, 26 Jul 2021 22:32:04 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Mon, 26 Jul 2021 22:32:05 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.3-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.3 CB_SHA256=8ee814ea8d99141de5493a6a24423c6a5dc4e01b8393dce87ca1639630315382 CB_VERSION=6.0.3
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Mon, 26 Jul 2021 22:33:04 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.3-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.3 CB_SHA256=8ee814ea8d99141de5493a6a24423c6a5dc4e01b8393dce87ca1639630315382 CB_VERSION=6.0.3
RUN set -x &&     export INSTALL_DONT_START_SERVER=1 &&     wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE &&     echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - &&     apt-get update &&     apt-get install -y ./$CB_PACKAGE &&     rm -f ./$CB_PACKAGE &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Mon, 26 Jul 2021 22:33:07 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.3-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.3 CB_SHA256=8ee814ea8d99141de5493a6a24423c6a5dc4e01b8393dce87ca1639630315382 CB_VERSION=6.0.3
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Mon, 26 Jul 2021 22:33:07 GMT
COPY file:d6a307209223b2df102f46f07fd186e09fac7114db2c965bb54097d3b4d3b989 in /etc/service/couchbase-server/run 
# Mon, 26 Jul 2021 22:33:08 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.3-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.3 CB_SHA256=8ee814ea8d99141de5493a6a24423c6a5dc4e01b8393dce87ca1639630315382 CB_VERSION=6.0.3
RUN mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Mon, 26 Jul 2021 22:33:08 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Mon, 26 Jul 2021 22:33:09 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.3-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.3 CB_SHA256=8ee814ea8d99141de5493a6a24423c6a5dc4e01b8393dce87ca1639630315382 CB_VERSION=6.0.3
RUN ln -s dummy.sh /usr/local/bin/iptables-save &&     ln -s dummy.sh /usr/local/bin/lvdisplay &&     ln -s dummy.sh /usr/local/bin/vgdisplay &&     ln -s dummy.sh /usr/local/bin/pvdisplay
# Mon, 26 Jul 2021 22:33:10 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.3-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.3 CB_SHA256=8ee814ea8d99141de5493a6a24423c6a5dc4e01b8393dce87ca1639630315382 CB_VERSION=6.0.3
RUN chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl
# Mon, 26 Jul 2021 22:33:10 GMT
COPY file:d816a67f62bfba76d2812cefbe92252afa13f3852775c3e68599df7741e90cb7 in / 
# Mon, 26 Jul 2021 22:33:10 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 26 Jul 2021 22:33:11 GMT
CMD ["couchbase-server"]
# Mon, 26 Jul 2021 22:33:11 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Mon, 26 Jul 2021 22:33:11 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:feac5306138255e28a9862d3f3d29025d0a4d0648855afe1acd6131af07138ac`  
		Last Modified: Mon, 26 Jul 2021 21:22:52 GMT  
		Size: 26.7 MB (26709039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d34675e7dacc0ce319b39b9ea2535f805fa959a52abc54f87cc0a227b97902ca`  
		Last Modified: Mon, 26 Jul 2021 22:42:05 GMT  
		Size: 15.9 MB (15922947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:889c4fafca81882f6937a23d718195844112f8f700b2bbf19b2fed74fb78653f`  
		Last Modified: Mon, 26 Jul 2021 22:42:00 GMT  
		Size: 266.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf63d6ecf19ab8433e888d60028f37b72e874642faf85a64dfe14f7f3b59ef21`  
		Last Modified: Mon, 26 Jul 2021 22:49:13 GMT  
		Size: 2.0 KB (1972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:070c0f8805a0755b8ea989ed753ea04b67ca6f7057608928f0bad9fd4d0e5a3c`  
		Last Modified: Mon, 26 Jul 2021 22:50:02 GMT  
		Size: 423.1 MB (423147337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c38f5da1bcc6f8521553f1ec088eac1985025d21f24fec6699ccf102e3baf57`  
		Last Modified: Mon, 26 Jul 2021 22:49:13 GMT  
		Size: 191.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4523762430d789fc41b4820c0d4491176caba39fd15593fb6f27936922c1da8f`  
		Last Modified: Mon, 26 Jul 2021 22:49:13 GMT  
		Size: 480.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04909e44f063c996a682f227885e67d56e15de6a849f7c55a4914edd2eb5d817`  
		Last Modified: Mon, 26 Jul 2021 22:49:11 GMT  
		Size: 280.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d18c0b61e9a5d6d27dd57aa37b5ba3f818b20e77dc8a451b99323bf84a1cb15b`  
		Last Modified: Mon, 26 Jul 2021 22:49:10 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89dec32a65b327246b726136e38e955f8da080e3b2575d5f36e3eaf3ba79d2a5`  
		Last Modified: Mon, 26 Jul 2021 22:49:10 GMT  
		Size: 217.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ac9e10f997ced10558d95ff2b41097eace89bed3867c2c6370a875e624fa671`  
		Last Modified: Mon, 26 Jul 2021 22:49:11 GMT  
		Size: 125.6 KB (125561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ca79437f0ce9c573ffeb4f6960d3ffffb2bde0b794250bd816964fa1c07eb82`  
		Last Modified: Mon, 26 Jul 2021 22:49:10 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchbase:enterprise-6.0.4`

```console
$ docker pull couchbase@sha256:59357050ffc9245a673bb94cf7f473afa8793efe831f8eb43b34cd6c864cf0b1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `couchbase:enterprise-6.0.4` - linux; amd64

```console
$ docker pull couchbase@sha256:2072d81f3b5f827d376965a1cea84f0bffa52384003b6e4f8165c4374341d35f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **467.2 MB (467176565 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92694534bfffd286b6c35bbc4783b3a87fbb8e902d6b070561842970528c5a3d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Mon, 26 Jul 2021 21:21:30 GMT
ADD file:e729fb032bd2f7cde20fb343da0cd358447e8b23028422c123944e8d0be660fa in / 
# Mon, 26 Jul 2021 21:21:31 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 22:21:49 GMT
LABEL maintainer=docker@couchbase.com
# Mon, 26 Jul 2021 22:23:55 GMT
RUN set -x &&     apt-get update &&     apt-get install -yq runit wget chrpath tzdata man     lsof lshw sysstat net-tools numactl python-httplib2 &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Mon, 26 Jul 2021 22:23:56 GMT
RUN if [ ! -x /usr/sbin/runsvdir-start ]; then         cp -a /etc/runit/2 /usr/sbin/runsvdir-start;     fi
# Mon, 26 Jul 2021 22:30:52 GMT
ARG CB_VERSION=6.0.4
# Mon, 26 Jul 2021 22:30:52 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.4
# Mon, 26 Jul 2021 22:30:52 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_6.0.4-ubuntu18.04_amd64.deb
# Mon, 26 Jul 2021 22:30:52 GMT
ARG CB_SHA256=7dbe8dd074f9cabea69468ea488f9ffc19c04dab8fc2e98c937fa32704982aff
# Mon, 26 Jul 2021 22:30:53 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Mon, 26 Jul 2021 22:30:53 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.4-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.4 CB_SHA256=7dbe8dd074f9cabea69468ea488f9ffc19c04dab8fc2e98c937fa32704982aff CB_VERSION=6.0.4
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Mon, 26 Jul 2021 22:31:51 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.4-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.4 CB_SHA256=7dbe8dd074f9cabea69468ea488f9ffc19c04dab8fc2e98c937fa32704982aff CB_VERSION=6.0.4
RUN set -x &&     export INSTALL_DONT_START_SERVER=1 &&     wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE &&     echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - &&     apt-get update &&     apt-get install -y ./$CB_PACKAGE &&     rm -f ./$CB_PACKAGE &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Mon, 26 Jul 2021 22:31:55 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.4-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.4 CB_SHA256=7dbe8dd074f9cabea69468ea488f9ffc19c04dab8fc2e98c937fa32704982aff CB_VERSION=6.0.4
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Mon, 26 Jul 2021 22:31:55 GMT
COPY file:d6a307209223b2df102f46f07fd186e09fac7114db2c965bb54097d3b4d3b989 in /etc/service/couchbase-server/run 
# Mon, 26 Jul 2021 22:31:56 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.4-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.4 CB_SHA256=7dbe8dd074f9cabea69468ea488f9ffc19c04dab8fc2e98c937fa32704982aff CB_VERSION=6.0.4
RUN mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Mon, 26 Jul 2021 22:31:56 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Mon, 26 Jul 2021 22:31:57 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.4-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.4 CB_SHA256=7dbe8dd074f9cabea69468ea488f9ffc19c04dab8fc2e98c937fa32704982aff CB_VERSION=6.0.4
RUN ln -s dummy.sh /usr/local/bin/iptables-save &&     ln -s dummy.sh /usr/local/bin/lvdisplay &&     ln -s dummy.sh /usr/local/bin/vgdisplay &&     ln -s dummy.sh /usr/local/bin/pvdisplay
# Mon, 26 Jul 2021 22:31:57 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.4-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.4 CB_SHA256=7dbe8dd074f9cabea69468ea488f9ffc19c04dab8fc2e98c937fa32704982aff CB_VERSION=6.0.4
RUN chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl
# Mon, 26 Jul 2021 22:31:58 GMT
COPY file:d816a67f62bfba76d2812cefbe92252afa13f3852775c3e68599df7741e90cb7 in / 
# Mon, 26 Jul 2021 22:31:58 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 26 Jul 2021 22:31:58 GMT
CMD ["couchbase-server"]
# Mon, 26 Jul 2021 22:31:58 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Mon, 26 Jul 2021 22:31:59 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:feac5306138255e28a9862d3f3d29025d0a4d0648855afe1acd6131af07138ac`  
		Last Modified: Mon, 26 Jul 2021 21:22:52 GMT  
		Size: 26.7 MB (26709039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d34675e7dacc0ce319b39b9ea2535f805fa959a52abc54f87cc0a227b97902ca`  
		Last Modified: Mon, 26 Jul 2021 22:42:05 GMT  
		Size: 15.9 MB (15922947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:889c4fafca81882f6937a23d718195844112f8f700b2bbf19b2fed74fb78653f`  
		Last Modified: Mon, 26 Jul 2021 22:42:00 GMT  
		Size: 266.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e574c78a46b41674f9a3261a0f0c68f76abd0af29aa26a2362df38dbcb6d3330`  
		Last Modified: Mon, 26 Jul 2021 22:47:59 GMT  
		Size: 2.0 KB (1968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14eb1008642f2ce7d352468ddc36a6f68069d11a44a253a029bfd0c2d1261c9a`  
		Last Modified: Mon, 26 Jul 2021 22:48:57 GMT  
		Size: 424.4 MB (424414525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f1e38580af5926287c75c797617759c89a0d42fc97c3aa2c0c4fe882e99c2b4`  
		Last Modified: Mon, 26 Jul 2021 22:47:59 GMT  
		Size: 191.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5ed61202651841bbbfe7ba1edd60b48fce04ad1b3aeb89a7d52e3b16a7c537c`  
		Last Modified: Mon, 26 Jul 2021 22:47:59 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:821f18160c226c642f0e30b158c5b1f1dc3c62470b537b709873f6c7a476dd33`  
		Last Modified: Mon, 26 Jul 2021 22:47:57 GMT  
		Size: 279.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bfd07498e11d153cd5fded3de1535089da489d5592399519f7b7290c183d61d`  
		Last Modified: Mon, 26 Jul 2021 22:47:57 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2432caa6ca57817ccc6feb3a8338adabb9a699a72a7c14080667989c2da7dd3`  
		Last Modified: Mon, 26 Jul 2021 22:47:57 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:882cf855fdcaee36f9707e3f2fa50e58a7c933e2b3a5f270152a180d5f3b9f4d`  
		Last Modified: Mon, 26 Jul 2021 22:47:57 GMT  
		Size: 125.6 KB (125559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99d9886ac4a5adeee111246e59b940f93799770342238916bfd704a9111e322f`  
		Last Modified: Mon, 26 Jul 2021 22:47:57 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchbase:enterprise-6.0.5`

```console
$ docker pull couchbase@sha256:4076897f81ab96c69d27f42accb996d141dbd3a2e9023579841b2361597553c1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `couchbase:enterprise-6.0.5` - linux; amd64

```console
$ docker pull couchbase@sha256:3a8ee070210558c8a7b4f42d1cef3d608db79a83510927b40eec0423ccbd23d5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **466.1 MB (466124028 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e8db7615f18de1e06f508993a9d442ce0eafcea50895d938de595152a2123121`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Mon, 26 Jul 2021 21:21:30 GMT
ADD file:e729fb032bd2f7cde20fb343da0cd358447e8b23028422c123944e8d0be660fa in / 
# Mon, 26 Jul 2021 21:21:31 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 22:21:49 GMT
LABEL maintainer=docker@couchbase.com
# Mon, 26 Jul 2021 22:23:55 GMT
RUN set -x &&     apt-get update &&     apt-get install -yq runit wget chrpath tzdata man     lsof lshw sysstat net-tools numactl python-httplib2 &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Mon, 26 Jul 2021 22:23:56 GMT
RUN if [ ! -x /usr/sbin/runsvdir-start ]; then         cp -a /etc/runit/2 /usr/sbin/runsvdir-start;     fi
# Mon, 26 Jul 2021 22:23:56 GMT
ARG CB_VERSION=6.0.5
# Mon, 26 Jul 2021 22:23:56 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.5
# Mon, 26 Jul 2021 22:23:56 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_6.0.5-ubuntu18.04_amd64.deb
# Mon, 26 Jul 2021 22:23:57 GMT
ARG CB_SHA256=6b152590867a58d771cffc22774d3cd66c916defcbeeeb339aca8d0a8e6d7f8d
# Mon, 26 Jul 2021 22:23:57 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Mon, 26 Jul 2021 22:23:58 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.5-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.5 CB_SHA256=6b152590867a58d771cffc22774d3cd66c916defcbeeeb339aca8d0a8e6d7f8d CB_VERSION=6.0.5
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Mon, 26 Jul 2021 22:24:57 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.5-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.5 CB_SHA256=6b152590867a58d771cffc22774d3cd66c916defcbeeeb339aca8d0a8e6d7f8d CB_VERSION=6.0.5
RUN set -x &&     export INSTALL_DONT_START_SERVER=1 &&     wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE &&     echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - &&     apt-get update &&     apt-get install -y ./$CB_PACKAGE &&     rm -f ./$CB_PACKAGE &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Mon, 26 Jul 2021 22:25:00 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.5-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.5 CB_SHA256=6b152590867a58d771cffc22774d3cd66c916defcbeeeb339aca8d0a8e6d7f8d CB_VERSION=6.0.5
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Mon, 26 Jul 2021 22:25:00 GMT
COPY file:d6a307209223b2df102f46f07fd186e09fac7114db2c965bb54097d3b4d3b989 in /etc/service/couchbase-server/run 
# Mon, 26 Jul 2021 22:25:01 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.5-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.5 CB_SHA256=6b152590867a58d771cffc22774d3cd66c916defcbeeeb339aca8d0a8e6d7f8d CB_VERSION=6.0.5
RUN mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Mon, 26 Jul 2021 22:25:01 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Mon, 26 Jul 2021 22:25:02 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.5-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.5 CB_SHA256=6b152590867a58d771cffc22774d3cd66c916defcbeeeb339aca8d0a8e6d7f8d CB_VERSION=6.0.5
RUN ln -s dummy.sh /usr/local/bin/iptables-save &&     ln -s dummy.sh /usr/local/bin/lvdisplay &&     ln -s dummy.sh /usr/local/bin/vgdisplay &&     ln -s dummy.sh /usr/local/bin/pvdisplay
# Mon, 26 Jul 2021 22:25:03 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.5-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.5 CB_SHA256=6b152590867a58d771cffc22774d3cd66c916defcbeeeb339aca8d0a8e6d7f8d CB_VERSION=6.0.5
RUN chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl
# Mon, 26 Jul 2021 22:25:03 GMT
COPY file:d816a67f62bfba76d2812cefbe92252afa13f3852775c3e68599df7741e90cb7 in / 
# Mon, 26 Jul 2021 22:25:04 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 26 Jul 2021 22:25:04 GMT
CMD ["couchbase-server"]
# Mon, 26 Jul 2021 22:25:04 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Mon, 26 Jul 2021 22:25:04 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:feac5306138255e28a9862d3f3d29025d0a4d0648855afe1acd6131af07138ac`  
		Last Modified: Mon, 26 Jul 2021 21:22:52 GMT  
		Size: 26.7 MB (26709039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d34675e7dacc0ce319b39b9ea2535f805fa959a52abc54f87cc0a227b97902ca`  
		Last Modified: Mon, 26 Jul 2021 22:42:05 GMT  
		Size: 15.9 MB (15922947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:889c4fafca81882f6937a23d718195844112f8f700b2bbf19b2fed74fb78653f`  
		Last Modified: Mon, 26 Jul 2021 22:42:00 GMT  
		Size: 266.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70f22272715b7ac39bdeb72247eb7c9d676e111cb87f716a6b7d9a3699677895`  
		Last Modified: Mon, 26 Jul 2021 22:41:58 GMT  
		Size: 2.0 KB (1969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6272140edf88cd01360aac5bddc2d13a011276f72173b6d9ae176fe243afbcbe`  
		Last Modified: Mon, 26 Jul 2021 22:42:41 GMT  
		Size: 423.4 MB (423361988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d78863e03e170d48a06840a1f3c0af08fc6a03998bd8b2cc5bd9d42146459335`  
		Last Modified: Mon, 26 Jul 2021 22:41:58 GMT  
		Size: 191.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce9c75079115b27ecc729a3d9a6ea34ffbbf322b75074b937b0a88b311b44e09`  
		Last Modified: Mon, 26 Jul 2021 22:41:58 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8be88b035f8327fce982f782ee4d4f158a491292ab1a83ea9bec04510e2eeedf`  
		Last Modified: Mon, 26 Jul 2021 22:41:55 GMT  
		Size: 280.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93191caa985b907966beca25f0640d7f64475b6f2662beaa3e13685df8684139`  
		Last Modified: Mon, 26 Jul 2021 22:41:58 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab9a7069e44f4669174a2e317fd06732143189d95777bc146d3897c070d52028`  
		Last Modified: Mon, 26 Jul 2021 22:41:55 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3d37421dd736067d67fc2e040630fd1bc247c1f2cfc75354428c93d6ace6ba3`  
		Last Modified: Mon, 26 Jul 2021 22:41:55 GMT  
		Size: 125.6 KB (125559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa4704f88c75024de08db79dc6908a3dc28f99ca5b88bb3d403b7410161fc66d`  
		Last Modified: Mon, 26 Jul 2021 22:41:55 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchbase:enterprise-6.5.0`

```console
$ docker pull couchbase@sha256:9387c6f85e86c0fd1d17503901d7736ef79666d3ee434a05d77cab05eb82944f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `couchbase:enterprise-6.5.0` - linux; amd64

```console
$ docker pull couchbase@sha256:2965cc1703c7207d7c0ab985d3b1d17527ce2b1ed4194c2e94ce4404ab4b7b70
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **542.2 MB (542236366 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:347b738ae0432bd3d41b32b59f1f101c8af3fce36f8aff0db87481fd4b6aa534`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Mon, 26 Jul 2021 21:21:30 GMT
ADD file:e729fb032bd2f7cde20fb343da0cd358447e8b23028422c123944e8d0be660fa in / 
# Mon, 26 Jul 2021 21:21:31 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 22:21:49 GMT
LABEL maintainer=docker@couchbase.com
# Mon, 26 Jul 2021 22:22:25 GMT
RUN set -x &&     apt-get update &&     apt-get install -yq runit wget chrpath tzdata man     lsof lshw sysstat net-tools numactl bzip2 &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Mon, 26 Jul 2021 22:22:26 GMT
RUN if [ ! -x /usr/sbin/runsvdir-start ]; then         cp -a /etc/runit/2 /usr/sbin/runsvdir-start;     fi
# Mon, 26 Jul 2021 22:29:26 GMT
ARG CB_VERSION=6.5.0
# Mon, 26 Jul 2021 22:29:26 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/6.5.0
# Mon, 26 Jul 2021 22:29:27 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_6.5.0-ubuntu18.04_amd64.deb
# Mon, 26 Jul 2021 22:29:27 GMT
ARG CB_SHA256=b4cafdc048b0caba85c24b90e6823e9ec2adc32061cafc527ddc99d706d6bc05
# Mon, 26 Jul 2021 22:29:27 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Mon, 26 Jul 2021 22:29:28 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.5.0-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.5.0 CB_SHA256=b4cafdc048b0caba85c24b90e6823e9ec2adc32061cafc527ddc99d706d6bc05 CB_VERSION=6.5.0
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Mon, 26 Jul 2021 22:30:36 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.5.0-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.5.0 CB_SHA256=b4cafdc048b0caba85c24b90e6823e9ec2adc32061cafc527ddc99d706d6bc05 CB_VERSION=6.5.0
RUN set -x &&     export INSTALL_DONT_START_SERVER=1 &&     wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE &&     echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - &&     apt-get update &&     apt-get install -y ./$CB_PACKAGE &&     rm -f ./$CB_PACKAGE &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Mon, 26 Jul 2021 22:30:40 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.5.0-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.5.0 CB_SHA256=b4cafdc048b0caba85c24b90e6823e9ec2adc32061cafc527ddc99d706d6bc05 CB_VERSION=6.5.0
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Mon, 26 Jul 2021 22:30:40 GMT
COPY file:d6a307209223b2df102f46f07fd186e09fac7114db2c965bb54097d3b4d3b989 in /etc/service/couchbase-server/run 
# Mon, 26 Jul 2021 22:30:41 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.5.0-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.5.0 CB_SHA256=b4cafdc048b0caba85c24b90e6823e9ec2adc32061cafc527ddc99d706d6bc05 CB_VERSION=6.5.0
RUN mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Mon, 26 Jul 2021 22:30:41 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Mon, 26 Jul 2021 22:30:42 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.5.0-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.5.0 CB_SHA256=b4cafdc048b0caba85c24b90e6823e9ec2adc32061cafc527ddc99d706d6bc05 CB_VERSION=6.5.0
RUN ln -s dummy.sh /usr/local/bin/iptables-save &&     ln -s dummy.sh /usr/local/bin/lvdisplay &&     ln -s dummy.sh /usr/local/bin/vgdisplay &&     ln -s dummy.sh /usr/local/bin/pvdisplay
# Mon, 26 Jul 2021 22:30:43 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.5.0-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.5.0 CB_SHA256=b4cafdc048b0caba85c24b90e6823e9ec2adc32061cafc527ddc99d706d6bc05 CB_VERSION=6.5.0
RUN chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl
# Mon, 26 Jul 2021 22:30:43 GMT
COPY file:d816a67f62bfba76d2812cefbe92252afa13f3852775c3e68599df7741e90cb7 in / 
# Mon, 26 Jul 2021 22:30:43 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 26 Jul 2021 22:30:44 GMT
CMD ["couchbase-server"]
# Mon, 26 Jul 2021 22:30:44 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Mon, 26 Jul 2021 22:30:44 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:feac5306138255e28a9862d3f3d29025d0a4d0648855afe1acd6131af07138ac`  
		Last Modified: Mon, 26 Jul 2021 21:22:52 GMT  
		Size: 26.7 MB (26709039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2a4e30704289595ec4268563ba339f4be2e264b88e79d255b680ccc550789ba`  
		Last Modified: Mon, 26 Jul 2021 22:41:09 GMT  
		Size: 7.4 MB (7373152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61d99bab81201d5c70f8e51f9f400575173f81ff7b28365411dc726bd35ec58d`  
		Last Modified: Mon, 26 Jul 2021 22:41:05 GMT  
		Size: 266.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b3f669ec644d0fc9e7ccde33439c5b7d2bbb56bc2ffde1565fdcb2313ffb018`  
		Last Modified: Mon, 26 Jul 2021 22:46:47 GMT  
		Size: 2.0 KB (1968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bad7d2497294635cf86849061925f4f120c3aa5d1f0b2d42ad8676ff616c4f8e`  
		Last Modified: Mon, 26 Jul 2021 22:47:44 GMT  
		Size: 508.0 MB (508031490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:740d72f0611aefdbcbfbab07c53099d044a0588e4316bf4ccd968818aefbd819`  
		Last Modified: Mon, 26 Jul 2021 22:46:46 GMT  
		Size: 191.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f6a2df8e1ea242f8693607bebe20f2a6ab4a568fdf1e6f61228fade370ac06e`  
		Last Modified: Mon, 26 Jul 2021 22:46:46 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0457572c00706de1d6e9522a5f0d2028fefaf79f16be1eb56cbaf6e99847089`  
		Last Modified: Mon, 26 Jul 2021 22:46:44 GMT  
		Size: 281.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9f2e39afe2424c9b028592e19e443ed2f0027473240cc14fdb0b59d093b43c0`  
		Last Modified: Mon, 26 Jul 2021 22:46:44 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d3ab6e813da57c9c0300bce664c95c9915a442625363458afc273024570886c`  
		Last Modified: Mon, 26 Jul 2021 22:46:44 GMT  
		Size: 217.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73f1e5798c71eda8b93bcc34c342819e6549ff71f3a52f972d1cbe39916ce41a`  
		Last Modified: Mon, 26 Jul 2021 22:46:44 GMT  
		Size: 118.2 KB (118191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b285cea2534462bf1b30a6c0fa6e4cab474972698b161529d550b92c8200200`  
		Last Modified: Mon, 26 Jul 2021 22:46:44 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchbase:enterprise-6.5.1`

```console
$ docker pull couchbase@sha256:0254bc931089c931928c7928c76dffbb0e6039c59ae8f94dd5f113cc348700fc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `couchbase:enterprise-6.5.1` - linux; amd64

```console
$ docker pull couchbase@sha256:56a7834eec771d194ef48a8c6c2df0a84c55be5556b2b30cff47bb46f7ef3fc0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **501.5 MB (501511512 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:83022788e529e8261037bba84084b8b245c561f826e586164f0c6ef351137f02`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Mon, 26 Jul 2021 21:21:30 GMT
ADD file:e729fb032bd2f7cde20fb343da0cd358447e8b23028422c123944e8d0be660fa in / 
# Mon, 26 Jul 2021 21:21:31 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 22:21:49 GMT
LABEL maintainer=docker@couchbase.com
# Mon, 26 Jul 2021 22:22:25 GMT
RUN set -x &&     apt-get update &&     apt-get install -yq runit wget chrpath tzdata man     lsof lshw sysstat net-tools numactl bzip2 &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Mon, 26 Jul 2021 22:22:26 GMT
RUN if [ ! -x /usr/sbin/runsvdir-start ]; then         cp -a /etc/runit/2 /usr/sbin/runsvdir-start;     fi
# Mon, 26 Jul 2021 22:28:01 GMT
ARG CB_VERSION=6.5.1
# Mon, 26 Jul 2021 22:28:01 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/6.5.1
# Mon, 26 Jul 2021 22:28:01 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_6.5.1-ubuntu18.04_amd64.deb
# Mon, 26 Jul 2021 22:28:01 GMT
ARG CB_SHA256=992fc9aef85c210cc2d782a1726f2ef56ceb322fd67c2e95500e276ff106e6ff
# Mon, 26 Jul 2021 22:28:02 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Mon, 26 Jul 2021 22:28:03 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.5.1-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.5.1 CB_SHA256=992fc9aef85c210cc2d782a1726f2ef56ceb322fd67c2e95500e276ff106e6ff CB_VERSION=6.5.1
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Mon, 26 Jul 2021 22:29:05 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.5.1-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.5.1 CB_SHA256=992fc9aef85c210cc2d782a1726f2ef56ceb322fd67c2e95500e276ff106e6ff CB_VERSION=6.5.1
RUN set -x &&     export INSTALL_DONT_START_SERVER=1 &&     wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE &&     echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - &&     apt-get update &&     apt-get install -y ./$CB_PACKAGE &&     rm -f ./$CB_PACKAGE &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Mon, 26 Jul 2021 22:29:07 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.5.1-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.5.1 CB_SHA256=992fc9aef85c210cc2d782a1726f2ef56ceb322fd67c2e95500e276ff106e6ff CB_VERSION=6.5.1
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Mon, 26 Jul 2021 22:29:08 GMT
COPY file:d6a307209223b2df102f46f07fd186e09fac7114db2c965bb54097d3b4d3b989 in /etc/service/couchbase-server/run 
# Mon, 26 Jul 2021 22:29:08 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.5.1-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.5.1 CB_SHA256=992fc9aef85c210cc2d782a1726f2ef56ceb322fd67c2e95500e276ff106e6ff CB_VERSION=6.5.1
RUN mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Mon, 26 Jul 2021 22:29:09 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Mon, 26 Jul 2021 22:29:09 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.5.1-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.5.1 CB_SHA256=992fc9aef85c210cc2d782a1726f2ef56ceb322fd67c2e95500e276ff106e6ff CB_VERSION=6.5.1
RUN ln -s dummy.sh /usr/local/bin/iptables-save &&     ln -s dummy.sh /usr/local/bin/lvdisplay &&     ln -s dummy.sh /usr/local/bin/vgdisplay &&     ln -s dummy.sh /usr/local/bin/pvdisplay
# Mon, 26 Jul 2021 22:29:10 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.5.1-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.5.1 CB_SHA256=992fc9aef85c210cc2d782a1726f2ef56ceb322fd67c2e95500e276ff106e6ff CB_VERSION=6.5.1
RUN chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl
# Mon, 26 Jul 2021 22:29:10 GMT
COPY file:d816a67f62bfba76d2812cefbe92252afa13f3852775c3e68599df7741e90cb7 in / 
# Mon, 26 Jul 2021 22:29:11 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 26 Jul 2021 22:29:11 GMT
CMD ["couchbase-server"]
# Mon, 26 Jul 2021 22:29:11 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Mon, 26 Jul 2021 22:29:11 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:feac5306138255e28a9862d3f3d29025d0a4d0648855afe1acd6131af07138ac`  
		Last Modified: Mon, 26 Jul 2021 21:22:52 GMT  
		Size: 26.7 MB (26709039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2a4e30704289595ec4268563ba339f4be2e264b88e79d255b680ccc550789ba`  
		Last Modified: Mon, 26 Jul 2021 22:41:09 GMT  
		Size: 7.4 MB (7373152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61d99bab81201d5c70f8e51f9f400575173f81ff7b28365411dc726bd35ec58d`  
		Last Modified: Mon, 26 Jul 2021 22:41:05 GMT  
		Size: 266.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:909345a645bc1c08329c7e80a3ff9fe1563ed753d2dc3e1eb03710bc35d44b40`  
		Last Modified: Mon, 26 Jul 2021 22:45:20 GMT  
		Size: 2.0 KB (1967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d855aad2e6af91ab6111b5826d3c1f948a6d3c6f173774756d73396793f5b89`  
		Last Modified: Mon, 26 Jul 2021 22:46:31 GMT  
		Size: 467.3 MB (467306639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68ea3f8ca21443b02bfba5a81304bfb1d7fe48119ff7bd55e285060b8c01bc68`  
		Last Modified: Mon, 26 Jul 2021 22:45:19 GMT  
		Size: 191.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a033f399787e6c32952c51add442bbd917a21958d0e4e59a4f3198a7b151205`  
		Last Modified: Mon, 26 Jul 2021 22:45:19 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b018f31e1c826afe291229aca140c54e623e1cfe7856459e93508a1d74799ac1`  
		Last Modified: Mon, 26 Jul 2021 22:45:17 GMT  
		Size: 281.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f041538ba3d0f3d11edbc9bdd75b7bfb070898fce64e34b08f3478780e1f08e`  
		Last Modified: Mon, 26 Jul 2021 22:45:16 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b72a132b7ddc7e6e2880deee77c218e55cc861c431858e464bdb154a2b7add1`  
		Last Modified: Mon, 26 Jul 2021 22:45:17 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ec6595ad3e89a6657440b99ffc0bfb797484e3e0ca28112fda1a4d062992dfc`  
		Last Modified: Mon, 26 Jul 2021 22:45:17 GMT  
		Size: 118.2 KB (118189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cd04f6da791cb9462e3e23cef1a4227594d77bbec153ae8c01cb59b152f3ace`  
		Last Modified: Mon, 26 Jul 2021 22:45:17 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchbase:enterprise-6.6.0`

```console
$ docker pull couchbase@sha256:6b1d9cf03e16f6a4095c6ad367d0fa4e745e56825f794e3f0f6af9365f5eb01a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `couchbase:enterprise-6.6.0` - linux; amd64

```console
$ docker pull couchbase@sha256:a2fc8cdd66c14a37b99b2494605e858bcb143cf9cdf376f3b7d1ec1acd66472e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **527.3 MB (527324890 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66d0f108e14b26d51dd738bb8af7e7f8e3779b0750eaa93ff9a2e3672499a0f6`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Mon, 26 Jul 2021 21:21:30 GMT
ADD file:e729fb032bd2f7cde20fb343da0cd358447e8b23028422c123944e8d0be660fa in / 
# Mon, 26 Jul 2021 21:21:31 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 22:21:49 GMT
LABEL maintainer=docker@couchbase.com
# Mon, 26 Jul 2021 22:22:25 GMT
RUN set -x &&     apt-get update &&     apt-get install -yq runit wget chrpath tzdata man     lsof lshw sysstat net-tools numactl bzip2 &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Mon, 26 Jul 2021 22:22:26 GMT
RUN if [ ! -x /usr/sbin/runsvdir-start ]; then         cp -a /etc/runit/2 /usr/sbin/runsvdir-start;     fi
# Mon, 26 Jul 2021 22:22:27 GMT
ARG CB_VERSION=6.6.0
# Mon, 26 Jul 2021 22:22:27 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0
# Mon, 26 Jul 2021 22:26:35 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_6.6.0-ubuntu18.04_amd64.deb
# Mon, 26 Jul 2021 22:26:36 GMT
ARG CB_SHA256=8e7fd5434537094be2fbdfedf3ab5005f0f7d5b9d0578f59ce540b424215b728
# Mon, 26 Jul 2021 22:26:36 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Mon, 26 Jul 2021 22:26:37 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.0-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=8e7fd5434537094be2fbdfedf3ab5005f0f7d5b9d0578f59ce540b424215b728 CB_VERSION=6.6.0
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Mon, 26 Jul 2021 22:27:43 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.0-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=8e7fd5434537094be2fbdfedf3ab5005f0f7d5b9d0578f59ce540b424215b728 CB_VERSION=6.6.0
RUN set -x &&     export INSTALL_DONT_START_SERVER=1 &&     wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE &&     echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - &&     apt-get update &&     apt-get install -y ./$CB_PACKAGE &&     rm -f ./$CB_PACKAGE &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Mon, 26 Jul 2021 22:27:47 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.0-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=8e7fd5434537094be2fbdfedf3ab5005f0f7d5b9d0578f59ce540b424215b728 CB_VERSION=6.6.0
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Mon, 26 Jul 2021 22:27:47 GMT
COPY file:d6a307209223b2df102f46f07fd186e09fac7114db2c965bb54097d3b4d3b989 in /etc/service/couchbase-server/run 
# Mon, 26 Jul 2021 22:27:48 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.0-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=8e7fd5434537094be2fbdfedf3ab5005f0f7d5b9d0578f59ce540b424215b728 CB_VERSION=6.6.0
RUN mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Mon, 26 Jul 2021 22:27:48 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Mon, 26 Jul 2021 22:27:49 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.0-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=8e7fd5434537094be2fbdfedf3ab5005f0f7d5b9d0578f59ce540b424215b728 CB_VERSION=6.6.0
RUN ln -s dummy.sh /usr/local/bin/iptables-save &&     ln -s dummy.sh /usr/local/bin/lvdisplay &&     ln -s dummy.sh /usr/local/bin/vgdisplay &&     ln -s dummy.sh /usr/local/bin/pvdisplay
# Mon, 26 Jul 2021 22:27:50 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.0-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=8e7fd5434537094be2fbdfedf3ab5005f0f7d5b9d0578f59ce540b424215b728 CB_VERSION=6.6.0
RUN chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl
# Mon, 26 Jul 2021 22:27:50 GMT
COPY file:d816a67f62bfba76d2812cefbe92252afa13f3852775c3e68599df7741e90cb7 in / 
# Mon, 26 Jul 2021 22:27:50 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 26 Jul 2021 22:27:50 GMT
CMD ["couchbase-server"]
# Mon, 26 Jul 2021 22:27:50 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Mon, 26 Jul 2021 22:27:51 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:feac5306138255e28a9862d3f3d29025d0a4d0648855afe1acd6131af07138ac`  
		Last Modified: Mon, 26 Jul 2021 21:22:52 GMT  
		Size: 26.7 MB (26709039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2a4e30704289595ec4268563ba339f4be2e264b88e79d255b680ccc550789ba`  
		Last Modified: Mon, 26 Jul 2021 22:41:09 GMT  
		Size: 7.4 MB (7373152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61d99bab81201d5c70f8e51f9f400575173f81ff7b28365411dc726bd35ec58d`  
		Last Modified: Mon, 26 Jul 2021 22:41:05 GMT  
		Size: 266.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c41056bf321c297635440676aa8845205766d98187c02bbb0a0a92dd844538c4`  
		Last Modified: Mon, 26 Jul 2021 22:44:07 GMT  
		Size: 2.0 KB (1966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1f4495478f55c2361512c14fd11182a2c4762b7dfa481381ad3133b3d9595dd`  
		Last Modified: Mon, 26 Jul 2021 22:45:03 GMT  
		Size: 493.1 MB (493120019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cf43d796878a1c1cbd05a076c43355bd3b70687d8bd28a1932468f2182eefce`  
		Last Modified: Mon, 26 Jul 2021 22:44:07 GMT  
		Size: 192.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af7fb99ce5d639f6830d982c769cde2d24eec0d1bcddb832c2bcee4b3d1f2c60`  
		Last Modified: Mon, 26 Jul 2021 22:44:07 GMT  
		Size: 479.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75040a6a6dac742b25c0f0fa89532c640f15591ec21af151eeafd6db74070c88`  
		Last Modified: Mon, 26 Jul 2021 22:44:04 GMT  
		Size: 280.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c0487699075b1f4c7b8cebd39a8d8973a207bac0c9b3717f95d8e83bd71fbb6`  
		Last Modified: Mon, 26 Jul 2021 22:44:04 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15756c2d9aecb2c909ac2b15a62c03f69345255bf9668f054e508d9c5a190ea1`  
		Last Modified: Mon, 26 Jul 2021 22:44:04 GMT  
		Size: 216.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a5b8651b569598c05e40067a744cc25f246fbce0a6ce50647dcbed6163a809a`  
		Last Modified: Mon, 26 Jul 2021 22:44:05 GMT  
		Size: 118.2 KB (118188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac7d1df271491a4d154090a38f26441d5575fa533057c224ced3295c0ff1871b`  
		Last Modified: Mon, 26 Jul 2021 22:44:04 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchbase:enterprise-6.6.1`

```console
$ docker pull couchbase@sha256:ce27277fe7678f903b02438304ff57ff4455002bb9440844f2ff31a2eed2a2bd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `couchbase:enterprise-6.6.1` - linux; amd64

```console
$ docker pull couchbase@sha256:8bae907adf53a82ae94c070752625dc94f9014807a26a232945d26eccdacbebb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **528.5 MB (528527045 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5b6f9c5715a276870475d948a55b433361fb63fab1c87dc085c57b563e089cda`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Mon, 26 Jul 2021 21:21:30 GMT
ADD file:e729fb032bd2f7cde20fb343da0cd358447e8b23028422c123944e8d0be660fa in / 
# Mon, 26 Jul 2021 21:21:31 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 22:21:49 GMT
LABEL maintainer=docker@couchbase.com
# Mon, 26 Jul 2021 22:22:25 GMT
RUN set -x &&     apt-get update &&     apt-get install -yq runit wget chrpath tzdata man     lsof lshw sysstat net-tools numactl bzip2 &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Mon, 26 Jul 2021 22:22:26 GMT
RUN if [ ! -x /usr/sbin/runsvdir-start ]; then         cp -a /etc/runit/2 /usr/sbin/runsvdir-start;     fi
# Mon, 26 Jul 2021 22:25:10 GMT
ARG CB_VERSION=6.6.1
# Mon, 26 Jul 2021 22:25:10 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.1
# Mon, 26 Jul 2021 22:25:10 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_6.6.1-ubuntu18.04_amd64.deb
# Mon, 26 Jul 2021 22:25:10 GMT
ARG CB_SHA256=4bd8210458905a5801e98bda0663d1214f6743465843f49ef9a52212636b5e89
# Mon, 26 Jul 2021 22:25:11 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Mon, 26 Jul 2021 22:25:11 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.1-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.1 CB_SHA256=4bd8210458905a5801e98bda0663d1214f6743465843f49ef9a52212636b5e89 CB_VERSION=6.6.1
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Mon, 26 Jul 2021 22:26:19 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.1-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.1 CB_SHA256=4bd8210458905a5801e98bda0663d1214f6743465843f49ef9a52212636b5e89 CB_VERSION=6.6.1
RUN set -x &&     export INSTALL_DONT_START_SERVER=1 &&     wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE &&     echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - &&     apt-get update &&     apt-get install -y ./$CB_PACKAGE &&     rm -f ./$CB_PACKAGE &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Mon, 26 Jul 2021 22:26:23 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.1-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.1 CB_SHA256=4bd8210458905a5801e98bda0663d1214f6743465843f49ef9a52212636b5e89 CB_VERSION=6.6.1
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Mon, 26 Jul 2021 22:26:23 GMT
COPY file:d6a307209223b2df102f46f07fd186e09fac7114db2c965bb54097d3b4d3b989 in /etc/service/couchbase-server/run 
# Mon, 26 Jul 2021 22:26:24 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.1-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.1 CB_SHA256=4bd8210458905a5801e98bda0663d1214f6743465843f49ef9a52212636b5e89 CB_VERSION=6.6.1
RUN mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Mon, 26 Jul 2021 22:26:24 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Mon, 26 Jul 2021 22:26:25 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.1-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.1 CB_SHA256=4bd8210458905a5801e98bda0663d1214f6743465843f49ef9a52212636b5e89 CB_VERSION=6.6.1
RUN ln -s dummy.sh /usr/local/bin/iptables-save &&     ln -s dummy.sh /usr/local/bin/lvdisplay &&     ln -s dummy.sh /usr/local/bin/vgdisplay &&     ln -s dummy.sh /usr/local/bin/pvdisplay
# Mon, 26 Jul 2021 22:26:26 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.1-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.1 CB_SHA256=4bd8210458905a5801e98bda0663d1214f6743465843f49ef9a52212636b5e89 CB_VERSION=6.6.1
RUN chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl
# Mon, 26 Jul 2021 22:26:26 GMT
COPY file:d816a67f62bfba76d2812cefbe92252afa13f3852775c3e68599df7741e90cb7 in / 
# Mon, 26 Jul 2021 22:26:26 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 26 Jul 2021 22:26:26 GMT
CMD ["couchbase-server"]
# Mon, 26 Jul 2021 22:26:27 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Mon, 26 Jul 2021 22:26:27 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:feac5306138255e28a9862d3f3d29025d0a4d0648855afe1acd6131af07138ac`  
		Last Modified: Mon, 26 Jul 2021 21:22:52 GMT  
		Size: 26.7 MB (26709039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2a4e30704289595ec4268563ba339f4be2e264b88e79d255b680ccc550789ba`  
		Last Modified: Mon, 26 Jul 2021 22:41:09 GMT  
		Size: 7.4 MB (7373152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61d99bab81201d5c70f8e51f9f400575173f81ff7b28365411dc726bd35ec58d`  
		Last Modified: Mon, 26 Jul 2021 22:41:05 GMT  
		Size: 266.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ab2f6ba05defbc278962d5c3675edb87a2a9aac298f764d149e8dfac6997210`  
		Last Modified: Mon, 26 Jul 2021 22:42:56 GMT  
		Size: 2.0 KB (1967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca281ad084b9caeb2bd4303f9ba708ebf5253a02428a14105ce61f4ad6c1649d`  
		Last Modified: Mon, 26 Jul 2021 22:43:52 GMT  
		Size: 494.3 MB (494322167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ee6152ff40f616ef043558d6c3bdb575595e9dcef1fdd0861342cf30cf9ad83`  
		Last Modified: Mon, 26 Jul 2021 22:42:56 GMT  
		Size: 191.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8076a41dccc574445e6fe0e1c3da4ac85e5d04a288a65f361e88bba93f8608aa`  
		Last Modified: Mon, 26 Jul 2021 22:42:57 GMT  
		Size: 479.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca6e027e9667d6d17e6ce6ac1a8893da041ed62683c31c582bdb8f1d738e50f8`  
		Last Modified: Mon, 26 Jul 2021 22:42:53 GMT  
		Size: 282.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fdbc0e5c5c39515362d1bb28bac1458a462fd9522995f866b1a24b4f5dd9063`  
		Last Modified: Mon, 26 Jul 2021 22:42:53 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4512e7ea1b1be5ec7744ca0b9d0e4c3c0720ed6fb5b2055b3c10f583b3ed25b3`  
		Last Modified: Mon, 26 Jul 2021 22:42:54 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ee32e5567f13959d200c1b58d732468142ea10d9e3e7a05bb249614074b6e05`  
		Last Modified: Mon, 26 Jul 2021 22:42:54 GMT  
		Size: 118.2 KB (118190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3cc78198ad3662750502dc48a81a466e27e0ad29b7f8970f2acfc87524c0d50`  
		Last Modified: Mon, 26 Jul 2021 22:42:53 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchbase:enterprise-6.6.2`

```console
$ docker pull couchbase@sha256:9e6e9947a937f0e1d692deb0276131e10f0f12a8fd469e33d30fdd6b6a658c73
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `couchbase:enterprise-6.6.2` - linux; amd64

```console
$ docker pull couchbase@sha256:2befadeed5bbfd07b657995c9432dad470840d4b32d8757c4de44f1f8bdb0bf6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **533.2 MB (533222654 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89c4c1a0b656b1893a5cc9277f0a39ac1771db24a19fcb5cd17e2c96f5b6f01d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Mon, 26 Jul 2021 21:21:39 GMT
ADD file:524e8d93ad65f08a0cb0d144268350186e36f508006b05b8faf2e1289499b59f in / 
# Mon, 26 Jul 2021 21:21:40 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 22:17:12 GMT
LABEL maintainer=docker@couchbase.com
# Mon, 26 Jul 2021 22:20:33 GMT
RUN set -x &&     apt-get update &&     apt-get install -yq runit wget chrpath tzdata     lsof lshw sysstat net-tools numactl bzip2 &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Mon, 26 Jul 2021 22:20:33 GMT
RUN if [ ! -x /usr/sbin/runsvdir-start ]; then         cp -a /etc/runit/2 /usr/sbin/runsvdir-start;     fi
# Mon, 26 Jul 2021 22:20:34 GMT
ARG CB_VERSION=6.6.2
# Mon, 26 Jul 2021 22:20:34 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.2
# Mon, 26 Jul 2021 22:20:34 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_6.6.2-ubuntu20.04_amd64.deb
# Mon, 26 Jul 2021 22:20:34 GMT
ARG CB_SHA256=41c033e6c1e98b0844a5cb5768e3769e7012d8374a6bd235c86e10db33b17afc
# Mon, 26 Jul 2021 22:20:34 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Mon, 26 Jul 2021 22:20:35 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.2-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.2 CB_SHA256=41c033e6c1e98b0844a5cb5768e3769e7012d8374a6bd235c86e10db33b17afc CB_VERSION=6.6.2
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Mon, 26 Jul 2021 22:21:31 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.2-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.2 CB_SHA256=41c033e6c1e98b0844a5cb5768e3769e7012d8374a6bd235c86e10db33b17afc CB_VERSION=6.6.2
RUN set -x &&     export INSTALL_DONT_START_SERVER=1 &&     wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE &&     echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - &&     apt-get update &&     apt-get install -y ./$CB_PACKAGE &&     rm -f ./$CB_PACKAGE &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Mon, 26 Jul 2021 22:21:35 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.2-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.2 CB_SHA256=41c033e6c1e98b0844a5cb5768e3769e7012d8374a6bd235c86e10db33b17afc CB_VERSION=6.6.2
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Mon, 26 Jul 2021 22:21:35 GMT
COPY file:d6a307209223b2df102f46f07fd186e09fac7114db2c965bb54097d3b4d3b989 in /etc/service/couchbase-server/run 
# Mon, 26 Jul 2021 22:21:36 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.2-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.2 CB_SHA256=41c033e6c1e98b0844a5cb5768e3769e7012d8374a6bd235c86e10db33b17afc CB_VERSION=6.6.2
RUN mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Mon, 26 Jul 2021 22:21:36 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Mon, 26 Jul 2021 22:21:37 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.2-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.2 CB_SHA256=41c033e6c1e98b0844a5cb5768e3769e7012d8374a6bd235c86e10db33b17afc CB_VERSION=6.6.2
RUN ln -s dummy.sh /usr/local/bin/iptables-save &&     ln -s dummy.sh /usr/local/bin/lvdisplay &&     ln -s dummy.sh /usr/local/bin/vgdisplay &&     ln -s dummy.sh /usr/local/bin/pvdisplay
# Mon, 26 Jul 2021 22:21:38 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.2-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.2 CB_SHA256=41c033e6c1e98b0844a5cb5768e3769e7012d8374a6bd235c86e10db33b17afc CB_VERSION=6.6.2
RUN chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl
# Mon, 26 Jul 2021 22:21:38 GMT
COPY file:d816a67f62bfba76d2812cefbe92252afa13f3852775c3e68599df7741e90cb7 in / 
# Mon, 26 Jul 2021 22:21:38 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 26 Jul 2021 22:21:38 GMT
CMD ["couchbase-server"]
# Mon, 26 Jul 2021 22:21:39 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Mon, 26 Jul 2021 22:21:39 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:16ec32c2132b43494832a05f2b02f7a822479f8250c173d0ab27b3de78b2f058`  
		Last Modified: Sun, 25 Jul 2021 03:03:29 GMT  
		Size: 28.6 MB (28567944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d887c602d6e2b416c36a7344e07f41278a46971fa08be0eeb2fc78a75d7013b`  
		Last Modified: Mon, 26 Jul 2021 22:39:49 GMT  
		Size: 6.3 MB (6272568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b219d16ecda3370190c17757e31f650c0b2db8a483364cebc0add69c976f1fa`  
		Last Modified: Mon, 26 Jul 2021 22:39:45 GMT  
		Size: 264.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:febb3fec572429eea18c02afb8a6c9879b303a8fe54f24c598d70e76284d2e50`  
		Last Modified: Mon, 26 Jul 2021 22:39:45 GMT  
		Size: 1.8 KB (1836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc966ce6300d6331c07980d729ddad541989a337e6eb174cab32a6da22196a4b`  
		Last Modified: Mon, 26 Jul 2021 22:40:42 GMT  
		Size: 498.3 MB (498251893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edb4c7a902a3d8673bde3e41bdcafb1f24b6bd970572a368d1d1c290bc0f0c5c`  
		Last Modified: Mon, 26 Jul 2021 22:39:45 GMT  
		Size: 191.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef06a70d616a9d9e24737530889d9744fa42fa92f9c293f9a47ab5046769e4e5`  
		Last Modified: Mon, 26 Jul 2021 22:39:45 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8a527aa307ea3cd1feffde8b7b71f90af3149dc21432afb9d9c9187c61017c5`  
		Last Modified: Mon, 26 Jul 2021 22:39:42 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4233c8f62d720537a74a69707dd1d651286d9bfab88848bb8d41445266481254`  
		Last Modified: Mon, 26 Jul 2021 22:39:42 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dda6ae4667566d063e0d185b915cc7fe3d16ea8dd7504aa48ae246e35db9d509`  
		Last Modified: Mon, 26 Jul 2021 22:39:42 GMT  
		Size: 217.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01243b96b0b7ddaf69634a7674356f0e483f5f24e91d57de48d161fcf28d65d0`  
		Last Modified: Mon, 26 Jul 2021 22:39:42 GMT  
		Size: 125.9 KB (125893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74aee4374d591a250acc5a5e8b2be6cacffceebba6ee89c2fe32ba3806144098`  
		Last Modified: Mon, 26 Jul 2021 22:39:42 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchbase:enterprise-7.0.0-beta`

```console
$ docker pull couchbase@sha256:6e44fa2454163f3b8225d8c4e3e0dfe90b884b78a69c35a806661ce96864adcc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `couchbase:enterprise-7.0.0-beta` - linux; amd64

```console
$ docker pull couchbase@sha256:9fe1cfbda9c8d987400c98872565178920a569c0c9fa50cb0b0e5b6bb40d248c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **628.1 MB (628099501 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f6a21205c8b00e182d981b8f3e6e3cfa85e3302d9ee85cc1c205da4f010f031d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Mon, 26 Jul 2021 21:21:39 GMT
ADD file:524e8d93ad65f08a0cb0d144268350186e36f508006b05b8faf2e1289499b59f in / 
# Mon, 26 Jul 2021 21:21:40 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 22:17:12 GMT
LABEL maintainer=docker@couchbase.com
# Mon, 26 Jul 2021 22:17:38 GMT
RUN set -x &&     apt-get update &&     apt-get install -yq runit wget chrpath tzdata man     lsof lshw sysstat net-tools numactl bzip2 &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Mon, 26 Jul 2021 22:17:39 GMT
RUN if [ ! -x /usr/sbin/runsvdir-start ]; then         cp -a /etc/runit/2 /usr/sbin/runsvdir-start;     fi
# Mon, 26 Jul 2021 22:17:39 GMT
ARG CB_VERSION=7.0.0-beta
# Mon, 26 Jul 2021 22:17:39 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.0-beta
# Mon, 26 Jul 2021 22:17:39 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_7.0.0-beta-ubuntu20.04_amd64.deb
# Mon, 26 Jul 2021 22:17:40 GMT
ARG CB_SHA256=e24be4f765eafbfbfdd5f7eddb780006084e3bd01cbcb3d3880dd9be48b955f6
# Mon, 26 Jul 2021 22:17:40 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Mon, 26 Jul 2021 22:17:41 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.0-beta-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.0-beta CB_SHA256=e24be4f765eafbfbfdd5f7eddb780006084e3bd01cbcb3d3880dd9be48b955f6 CB_VERSION=7.0.0-beta
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Mon, 26 Jul 2021 22:18:57 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.0-beta-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.0-beta CB_SHA256=e24be4f765eafbfbfdd5f7eddb780006084e3bd01cbcb3d3880dd9be48b955f6 CB_VERSION=7.0.0-beta
RUN set -x &&     export INSTALL_DONT_START_SERVER=1 &&     wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE &&     echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - &&     apt-get update &&     apt-get install -y ./$CB_PACKAGE &&     rm -f ./$CB_PACKAGE &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Mon, 26 Jul 2021 22:19:02 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.0-beta-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.0-beta CB_SHA256=e24be4f765eafbfbfdd5f7eddb780006084e3bd01cbcb3d3880dd9be48b955f6 CB_VERSION=7.0.0-beta
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Mon, 26 Jul 2021 22:19:02 GMT
COPY file:d6a307209223b2df102f46f07fd186e09fac7114db2c965bb54097d3b4d3b989 in /etc/service/couchbase-server/run 
# Mon, 26 Jul 2021 22:19:03 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.0-beta-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.0-beta CB_SHA256=e24be4f765eafbfbfdd5f7eddb780006084e3bd01cbcb3d3880dd9be48b955f6 CB_VERSION=7.0.0-beta
RUN mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Mon, 26 Jul 2021 22:19:03 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Mon, 26 Jul 2021 22:19:04 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.0-beta-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.0-beta CB_SHA256=e24be4f765eafbfbfdd5f7eddb780006084e3bd01cbcb3d3880dd9be48b955f6 CB_VERSION=7.0.0-beta
RUN ln -s dummy.sh /usr/local/bin/iptables-save &&     ln -s dummy.sh /usr/local/bin/lvdisplay &&     ln -s dummy.sh /usr/local/bin/vgdisplay &&     ln -s dummy.sh /usr/local/bin/pvdisplay
# Mon, 26 Jul 2021 22:19:05 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.0-beta-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.0-beta CB_SHA256=e24be4f765eafbfbfdd5f7eddb780006084e3bd01cbcb3d3880dd9be48b955f6 CB_VERSION=7.0.0-beta
RUN chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl
# Mon, 26 Jul 2021 22:19:05 GMT
COPY file:d816a67f62bfba76d2812cefbe92252afa13f3852775c3e68599df7741e90cb7 in / 
# Mon, 26 Jul 2021 22:19:05 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 26 Jul 2021 22:19:06 GMT
CMD ["couchbase-server"]
# Mon, 26 Jul 2021 22:19:06 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Mon, 26 Jul 2021 22:19:06 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:16ec32c2132b43494832a05f2b02f7a822479f8250c173d0ab27b3de78b2f058`  
		Last Modified: Sun, 25 Jul 2021 03:03:29 GMT  
		Size: 28.6 MB (28567944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0f4f47bb294f3f6f2dc58514a7dc33b42f8be77cfbbed0dbd1c8a49fca73899`  
		Last Modified: Mon, 26 Jul 2021 22:37:21 GMT  
		Size: 8.3 MB (8287040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e87aaeab53b206101d3fd9751a01810367e7cc684b3636f34e03abd4eec34d3`  
		Last Modified: Mon, 26 Jul 2021 22:37:16 GMT  
		Size: 264.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:417c7614b0fa37252a483308c9753ce5585933d987ea87961c5d9f55f79b720f`  
		Last Modified: Mon, 26 Jul 2021 22:37:16 GMT  
		Size: 1.8 KB (1837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2fde59718fdb413fa07cd7726e0c1f85f79c58d5ed1b201ac7e176d760bbb13`  
		Last Modified: Mon, 26 Jul 2021 22:38:28 GMT  
		Size: 591.1 MB (591114272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c2080252da7d35cf811f882d0f2a573fc3ea1a2c1b150c79368504002e92108`  
		Last Modified: Mon, 26 Jul 2021 22:37:16 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ad5beec000a75f8a1317b3a750fa17fa79638ed6a6fbb98dd91da2cd108a5bf`  
		Last Modified: Mon, 26 Jul 2021 22:37:16 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41bf72ef287f7997839083e39e4cadffa670e9cff91d572cbf064e7401a7bbd2`  
		Last Modified: Mon, 26 Jul 2021 22:37:13 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7973404887aa66902dd9a9e71fb076a67b3fac23ee1f3959be162f6f4bea088`  
		Last Modified: Mon, 26 Jul 2021 22:37:13 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da5872978d3451c5bf98a88425bcbaab9acd795c10fe9a46d5e416e0af549199`  
		Last Modified: Mon, 26 Jul 2021 22:37:13 GMT  
		Size: 217.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03667f47b7202daf73978394d95beca395bc90ecb6a0ff4f6f4e09cd442db30d`  
		Last Modified: Mon, 26 Jul 2021 22:37:14 GMT  
		Size: 125.9 KB (125894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83063b4e8c4354d6466cc2e72d4ec1ff97ff5f81bea8512990a6fa4d01f993e4`  
		Last Modified: Mon, 26 Jul 2021 22:37:14 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchbase:latest`

```console
$ docker pull couchbase@sha256:9e6e9947a937f0e1d692deb0276131e10f0f12a8fd469e33d30fdd6b6a658c73
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `couchbase:latest` - linux; amd64

```console
$ docker pull couchbase@sha256:2befadeed5bbfd07b657995c9432dad470840d4b32d8757c4de44f1f8bdb0bf6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **533.2 MB (533222654 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89c4c1a0b656b1893a5cc9277f0a39ac1771db24a19fcb5cd17e2c96f5b6f01d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Mon, 26 Jul 2021 21:21:39 GMT
ADD file:524e8d93ad65f08a0cb0d144268350186e36f508006b05b8faf2e1289499b59f in / 
# Mon, 26 Jul 2021 21:21:40 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 22:17:12 GMT
LABEL maintainer=docker@couchbase.com
# Mon, 26 Jul 2021 22:20:33 GMT
RUN set -x &&     apt-get update &&     apt-get install -yq runit wget chrpath tzdata     lsof lshw sysstat net-tools numactl bzip2 &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Mon, 26 Jul 2021 22:20:33 GMT
RUN if [ ! -x /usr/sbin/runsvdir-start ]; then         cp -a /etc/runit/2 /usr/sbin/runsvdir-start;     fi
# Mon, 26 Jul 2021 22:20:34 GMT
ARG CB_VERSION=6.6.2
# Mon, 26 Jul 2021 22:20:34 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.2
# Mon, 26 Jul 2021 22:20:34 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_6.6.2-ubuntu20.04_amd64.deb
# Mon, 26 Jul 2021 22:20:34 GMT
ARG CB_SHA256=41c033e6c1e98b0844a5cb5768e3769e7012d8374a6bd235c86e10db33b17afc
# Mon, 26 Jul 2021 22:20:34 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Mon, 26 Jul 2021 22:20:35 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.2-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.2 CB_SHA256=41c033e6c1e98b0844a5cb5768e3769e7012d8374a6bd235c86e10db33b17afc CB_VERSION=6.6.2
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Mon, 26 Jul 2021 22:21:31 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.2-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.2 CB_SHA256=41c033e6c1e98b0844a5cb5768e3769e7012d8374a6bd235c86e10db33b17afc CB_VERSION=6.6.2
RUN set -x &&     export INSTALL_DONT_START_SERVER=1 &&     wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE &&     echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - &&     apt-get update &&     apt-get install -y ./$CB_PACKAGE &&     rm -f ./$CB_PACKAGE &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Mon, 26 Jul 2021 22:21:35 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.2-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.2 CB_SHA256=41c033e6c1e98b0844a5cb5768e3769e7012d8374a6bd235c86e10db33b17afc CB_VERSION=6.6.2
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Mon, 26 Jul 2021 22:21:35 GMT
COPY file:d6a307209223b2df102f46f07fd186e09fac7114db2c965bb54097d3b4d3b989 in /etc/service/couchbase-server/run 
# Mon, 26 Jul 2021 22:21:36 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.2-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.2 CB_SHA256=41c033e6c1e98b0844a5cb5768e3769e7012d8374a6bd235c86e10db33b17afc CB_VERSION=6.6.2
RUN mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Mon, 26 Jul 2021 22:21:36 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Mon, 26 Jul 2021 22:21:37 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.2-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.2 CB_SHA256=41c033e6c1e98b0844a5cb5768e3769e7012d8374a6bd235c86e10db33b17afc CB_VERSION=6.6.2
RUN ln -s dummy.sh /usr/local/bin/iptables-save &&     ln -s dummy.sh /usr/local/bin/lvdisplay &&     ln -s dummy.sh /usr/local/bin/vgdisplay &&     ln -s dummy.sh /usr/local/bin/pvdisplay
# Mon, 26 Jul 2021 22:21:38 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.2-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.2 CB_SHA256=41c033e6c1e98b0844a5cb5768e3769e7012d8374a6bd235c86e10db33b17afc CB_VERSION=6.6.2
RUN chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl
# Mon, 26 Jul 2021 22:21:38 GMT
COPY file:d816a67f62bfba76d2812cefbe92252afa13f3852775c3e68599df7741e90cb7 in / 
# Mon, 26 Jul 2021 22:21:38 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 26 Jul 2021 22:21:38 GMT
CMD ["couchbase-server"]
# Mon, 26 Jul 2021 22:21:39 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Mon, 26 Jul 2021 22:21:39 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:16ec32c2132b43494832a05f2b02f7a822479f8250c173d0ab27b3de78b2f058`  
		Last Modified: Sun, 25 Jul 2021 03:03:29 GMT  
		Size: 28.6 MB (28567944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d887c602d6e2b416c36a7344e07f41278a46971fa08be0eeb2fc78a75d7013b`  
		Last Modified: Mon, 26 Jul 2021 22:39:49 GMT  
		Size: 6.3 MB (6272568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b219d16ecda3370190c17757e31f650c0b2db8a483364cebc0add69c976f1fa`  
		Last Modified: Mon, 26 Jul 2021 22:39:45 GMT  
		Size: 264.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:febb3fec572429eea18c02afb8a6c9879b303a8fe54f24c598d70e76284d2e50`  
		Last Modified: Mon, 26 Jul 2021 22:39:45 GMT  
		Size: 1.8 KB (1836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc966ce6300d6331c07980d729ddad541989a337e6eb174cab32a6da22196a4b`  
		Last Modified: Mon, 26 Jul 2021 22:40:42 GMT  
		Size: 498.3 MB (498251893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edb4c7a902a3d8673bde3e41bdcafb1f24b6bd970572a368d1d1c290bc0f0c5c`  
		Last Modified: Mon, 26 Jul 2021 22:39:45 GMT  
		Size: 191.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef06a70d616a9d9e24737530889d9744fa42fa92f9c293f9a47ab5046769e4e5`  
		Last Modified: Mon, 26 Jul 2021 22:39:45 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8a527aa307ea3cd1feffde8b7b71f90af3149dc21432afb9d9c9187c61017c5`  
		Last Modified: Mon, 26 Jul 2021 22:39:42 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4233c8f62d720537a74a69707dd1d651286d9bfab88848bb8d41445266481254`  
		Last Modified: Mon, 26 Jul 2021 22:39:42 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dda6ae4667566d063e0d185b915cc7fe3d16ea8dd7504aa48ae246e35db9d509`  
		Last Modified: Mon, 26 Jul 2021 22:39:42 GMT  
		Size: 217.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01243b96b0b7ddaf69634a7674356f0e483f5f24e91d57de48d161fcf28d65d0`  
		Last Modified: Mon, 26 Jul 2021 22:39:42 GMT  
		Size: 125.9 KB (125893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74aee4374d591a250acc5a5e8b2be6cacffceebba6ee89c2fe32ba3806144098`  
		Last Modified: Mon, 26 Jul 2021 22:39:42 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
