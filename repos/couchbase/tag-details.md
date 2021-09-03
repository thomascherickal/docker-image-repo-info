<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `couchbase`

-	[`couchbase:6.0.5`](#couchbase605)
-	[`couchbase:6.6.3`](#couchbase663)
-	[`couchbase:7.0.1`](#couchbase701)
-	[`couchbase:community`](#couchbasecommunity)
-	[`couchbase:community-6.6.0`](#couchbasecommunity-660)
-	[`couchbase:community-7.0.1`](#couchbasecommunity-701)
-	[`couchbase:enterprise`](#couchbaseenterprise)
-	[`couchbase:enterprise-6.0.5`](#couchbaseenterprise-605)
-	[`couchbase:enterprise-6.6.3`](#couchbaseenterprise-663)
-	[`couchbase:enterprise-7.0.1`](#couchbaseenterprise-701)
-	[`couchbase:latest`](#couchbaselatest)

## `couchbase:6.0.5`

```console
$ docker pull couchbase@sha256:98299b065e5be953e2762a65c4a848f0b153c863b9b4831b5c879bb66ab4d86c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `couchbase:6.0.5` - linux; amd64

```console
$ docker pull couchbase@sha256:dbe90ce9e946168227833c090d4719986d63aa17e2eb4bb5a73b9c619ed2311f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **466.1 MB (466125041 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1672e6f2e19e654639ea62a998982902461bc803be7694258c54cd3b646c8c22`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Tue, 31 Aug 2021 01:20:48 GMT
ADD file:425a053fd043786e9454fb269d4c93c624550fb913a8c96d03ddd430b4e6c1c3 in / 
# Tue, 31 Aug 2021 01:20:48 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 03:21:37 GMT
LABEL maintainer=docker@couchbase.com
# Tue, 31 Aug 2021 03:23:42 GMT
RUN set -x &&     apt-get update &&     apt-get install -yq runit wget chrpath tzdata man     lsof lshw sysstat net-tools numactl python-httplib2 &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Tue, 31 Aug 2021 03:23:43 GMT
RUN if [ ! -x /usr/sbin/runsvdir-start ]; then         cp -a /etc/runit/2 /usr/sbin/runsvdir-start;     fi
# Tue, 31 Aug 2021 03:23:43 GMT
ARG CB_VERSION=6.0.5
# Tue, 31 Aug 2021 03:23:43 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.5
# Tue, 31 Aug 2021 03:23:43 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_6.0.5-ubuntu18.04_amd64.deb
# Tue, 31 Aug 2021 03:23:43 GMT
ARG CB_SHA256=6b152590867a58d771cffc22774d3cd66c916defcbeeeb339aca8d0a8e6d7f8d
# Tue, 31 Aug 2021 03:23:44 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Tue, 31 Aug 2021 03:23:44 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.5-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.5 CB_SHA256=6b152590867a58d771cffc22774d3cd66c916defcbeeeb339aca8d0a8e6d7f8d CB_VERSION=6.0.5
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Tue, 31 Aug 2021 03:24:33 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.5-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.5 CB_SHA256=6b152590867a58d771cffc22774d3cd66c916defcbeeeb339aca8d0a8e6d7f8d CB_VERSION=6.0.5
RUN set -x &&     export INSTALL_DONT_START_SERVER=1 &&     wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE &&     echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - &&     apt-get update &&     apt-get install -y ./$CB_PACKAGE &&     rm -f ./$CB_PACKAGE &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Tue, 31 Aug 2021 03:24:36 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.5-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.5 CB_SHA256=6b152590867a58d771cffc22774d3cd66c916defcbeeeb339aca8d0a8e6d7f8d CB_VERSION=6.0.5
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Tue, 31 Aug 2021 03:24:36 GMT
COPY file:d6a307209223b2df102f46f07fd186e09fac7114db2c965bb54097d3b4d3b989 in /etc/service/couchbase-server/run 
# Tue, 31 Aug 2021 03:24:37 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.5-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.5 CB_SHA256=6b152590867a58d771cffc22774d3cd66c916defcbeeeb339aca8d0a8e6d7f8d CB_VERSION=6.0.5
RUN mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Tue, 31 Aug 2021 03:24:37 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Tue, 31 Aug 2021 03:24:38 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.5-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.5 CB_SHA256=6b152590867a58d771cffc22774d3cd66c916defcbeeeb339aca8d0a8e6d7f8d CB_VERSION=6.0.5
RUN ln -s dummy.sh /usr/local/bin/iptables-save &&     ln -s dummy.sh /usr/local/bin/lvdisplay &&     ln -s dummy.sh /usr/local/bin/vgdisplay &&     ln -s dummy.sh /usr/local/bin/pvdisplay
# Tue, 31 Aug 2021 03:24:39 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.5-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.5 CB_SHA256=6b152590867a58d771cffc22774d3cd66c916defcbeeeb339aca8d0a8e6d7f8d CB_VERSION=6.0.5
RUN chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl
# Tue, 31 Aug 2021 03:24:39 GMT
COPY file:d816a67f62bfba76d2812cefbe92252afa13f3852775c3e68599df7741e90cb7 in / 
# Tue, 31 Aug 2021 03:24:39 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 31 Aug 2021 03:24:39 GMT
CMD ["couchbase-server"]
# Tue, 31 Aug 2021 03:24:39 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Tue, 31 Aug 2021 03:24:40 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:e4ca327ec0e73c737201b7a6d7b2df779a3ccf34fe9cf1b0c031e767f6464240`  
		Last Modified: Tue, 31 Aug 2021 01:22:00 GMT  
		Size: 26.7 MB (26708511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4ad2462e90bbb875192fc60ad73a37767fd66736c2d77864c1aa1706277e1b8`  
		Last Modified: Tue, 31 Aug 2021 03:29:31 GMT  
		Size: 15.9 MB (15923740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eade3950f0dac395edba948c8a11be6bb13842c0a0bb507d066d3497a8dd7f9`  
		Last Modified: Tue, 31 Aug 2021 03:29:27 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b3385d6562a5a590e21b076d3556b3a9b913f2a4bb301835793cde88d6ad078`  
		Last Modified: Tue, 31 Aug 2021 03:29:27 GMT  
		Size: 2.0 KB (1964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6086cfa42a7e9a96aec888e2245d28d715d9c387136833786b46cc336ef96186`  
		Last Modified: Tue, 31 Aug 2021 03:30:04 GMT  
		Size: 423.4 MB (423362749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:692cbc042cd7250d3bff14a5c3b85c853b497afefc270b93349dbba7501519da`  
		Last Modified: Tue, 31 Aug 2021 03:29:26 GMT  
		Size: 190.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:685784ad28283d623e9acaf2e643630dd7f65d6e792e9e13b69569c3536b6121`  
		Last Modified: Tue, 31 Aug 2021 03:29:26 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:410d54ee1b88dd20786bdb20fb38cd37d8da77195ce4f99e1b6710ee6b529d43`  
		Last Modified: Tue, 31 Aug 2021 03:29:23 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dcf337856e610d54c62aba78828847d0eaa902e745eaaca762084b16972c8b2`  
		Last Modified: Tue, 31 Aug 2021 03:29:24 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44af54e22a6200630e014aa7dc566d5d066d981aa931dcde26108c32a0c6ffd1`  
		Last Modified: Tue, 31 Aug 2021 03:29:23 GMT  
		Size: 217.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ea158ae8b16554d05ce26da1c58f180666d03d25e865f71dd42973f5d7aa6ef`  
		Last Modified: Tue, 31 Aug 2021 03:29:24 GMT  
		Size: 125.6 KB (125561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a055e1c798f0e0dc2dfd3b663ff5c85ef232c924ace8e715277f44d7b5d8967`  
		Last Modified: Tue, 31 Aug 2021 03:29:24 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchbase:6.6.3`

```console
$ docker pull couchbase@sha256:0cdced609b593b8b5f73139618c8cc1b67e5adef88adff9339bc9807cb726bdc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `couchbase:6.6.3` - linux; amd64

```console
$ docker pull couchbase@sha256:6a7d2b34a79f9d30dcf38c80978811c3cda6d0810d7916772eba8018b70ae176
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **537.4 MB (537352018 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c0fd088ab18fbea2b1c7b7a1c953fed9e3d79a45cc60ce91da437663913e4ed`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Tue, 31 Aug 2021 01:20:55 GMT
ADD file:d2abf27fe2e8b0b5f4da68c018560c73e11c53098329246e3e6fe176698ef941 in / 
# Tue, 31 Aug 2021 01:20:56 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 03:17:15 GMT
LABEL maintainer=docker@couchbase.com
# Tue, 31 Aug 2021 03:17:35 GMT
RUN set -x &&     apt-get update &&     apt-get install -yq runit wget chrpath tzdata     lsof lshw sysstat net-tools numactl bzip2 &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Tue, 31 Aug 2021 03:17:36 GMT
RUN if [ ! -x /usr/sbin/runsvdir-start ]; then         cp -a /etc/runit/2 /usr/sbin/runsvdir-start;     fi
# Tue, 31 Aug 2021 03:20:11 GMT
ARG CB_VERSION=6.6.3
# Tue, 31 Aug 2021 03:20:11 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.3
# Tue, 31 Aug 2021 03:20:12 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_6.6.3-ubuntu20.04_amd64.deb
# Tue, 31 Aug 2021 03:20:12 GMT
ARG CB_SHA256=8d62db9365171aba0ee646c0189b81dec8ef9718fac7b44bd72e15da4e2b38fa
# Tue, 31 Aug 2021 03:20:12 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Tue, 31 Aug 2021 03:20:13 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.3-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.3 CB_SHA256=8d62db9365171aba0ee646c0189b81dec8ef9718fac7b44bd72e15da4e2b38fa CB_VERSION=6.6.3
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Tue, 31 Aug 2021 03:21:16 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.3-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.3 CB_SHA256=8d62db9365171aba0ee646c0189b81dec8ef9718fac7b44bd72e15da4e2b38fa CB_VERSION=6.6.3
RUN set -x &&     export INSTALL_DONT_START_SERVER=1 &&     wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE &&     echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - &&     apt-get update &&     apt-get install -y ./$CB_PACKAGE &&     rm -f ./$CB_PACKAGE &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Tue, 31 Aug 2021 03:21:19 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.3-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.3 CB_SHA256=8d62db9365171aba0ee646c0189b81dec8ef9718fac7b44bd72e15da4e2b38fa CB_VERSION=6.6.3
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Tue, 31 Aug 2021 03:21:19 GMT
COPY file:d6a307209223b2df102f46f07fd186e09fac7114db2c965bb54097d3b4d3b989 in /etc/service/couchbase-server/run 
# Tue, 31 Aug 2021 03:21:20 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.3-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.3 CB_SHA256=8d62db9365171aba0ee646c0189b81dec8ef9718fac7b44bd72e15da4e2b38fa CB_VERSION=6.6.3
RUN mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Tue, 31 Aug 2021 03:21:20 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Tue, 31 Aug 2021 03:21:21 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.3-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.3 CB_SHA256=8d62db9365171aba0ee646c0189b81dec8ef9718fac7b44bd72e15da4e2b38fa CB_VERSION=6.6.3
RUN ln -s dummy.sh /usr/local/bin/iptables-save &&     ln -s dummy.sh /usr/local/bin/lvdisplay &&     ln -s dummy.sh /usr/local/bin/vgdisplay &&     ln -s dummy.sh /usr/local/bin/pvdisplay
# Tue, 31 Aug 2021 03:21:22 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.3-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.3 CB_SHA256=8d62db9365171aba0ee646c0189b81dec8ef9718fac7b44bd72e15da4e2b38fa CB_VERSION=6.6.3
RUN chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl
# Tue, 31 Aug 2021 03:21:22 GMT
COPY file:d816a67f62bfba76d2812cefbe92252afa13f3852775c3e68599df7741e90cb7 in / 
# Tue, 31 Aug 2021 03:21:22 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 31 Aug 2021 03:21:22 GMT
CMD ["couchbase-server"]
# Tue, 31 Aug 2021 03:21:22 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Tue, 31 Aug 2021 03:21:23 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:35807b77a593c1147d13dc926a91dcc3015616ff7307cc30442c5a8e07546283`  
		Last Modified: Sat, 28 Aug 2021 03:03:19 GMT  
		Size: 28.6 MB (28570074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:909a89f4ffc52b1bc0efc8b382b1da145d18cc3fe8aa349a8c93a0174473f38d`  
		Last Modified: Tue, 31 Aug 2021 03:25:11 GMT  
		Size: 6.3 MB (6265547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:669f46faa4219d00fffdc48350b495c094272d77b1505e7438e9786ced31ff1f`  
		Last Modified: Tue, 31 Aug 2021 03:25:07 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a89ac926d4775c8d4f51706c70fe390b5b95b0b12f35c987ad907f59009ee536`  
		Last Modified: Tue, 31 Aug 2021 03:27:35 GMT  
		Size: 1.8 KB (1835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bebb7385ebeec7ff3b3d7c596e2e635943a663ae003a5b0d18e1ae1f89488824`  
		Last Modified: Tue, 31 Aug 2021 03:28:25 GMT  
		Size: 502.4 MB (502386144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1a15fa94f9ecea4ad6dce3368e71f33be66591270ffdb1c422a75b66e147b7a`  
		Last Modified: Tue, 31 Aug 2021 03:27:34 GMT  
		Size: 190.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eeb435a3f6e2b1717eac3ab6303aeff19c9753f4024f38bf901c6914686360bd`  
		Last Modified: Tue, 31 Aug 2021 03:27:34 GMT  
		Size: 479.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a92f45b4fdedce790baf8acf9626db3960dae920c03d1ae18825d0cdc1e5ed06`  
		Last Modified: Tue, 31 Aug 2021 03:27:32 GMT  
		Size: 280.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a044aae35413dcb08801b544e0b334257018690f68a91506ac8cc003b6f3a221`  
		Last Modified: Tue, 31 Aug 2021 03:27:32 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cd9c0021b6ef3531ae150814ece79f5020f50d7021bcaaddedaf17f9a472682`  
		Last Modified: Tue, 31 Aug 2021 03:27:32 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56ed7d9a5135475cb0d2f6da610076dae33f53affb9e19395872138f904651d7`  
		Last Modified: Tue, 31 Aug 2021 03:27:32 GMT  
		Size: 125.9 KB (125891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d335ea28a1383ac0227bb8d1ada6eeec85a791ef7af92bc766ce7069fd5334df`  
		Last Modified: Tue, 31 Aug 2021 03:27:32 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchbase:7.0.1`

**does not exist** (yet?)

## `couchbase:community`

```console
$ docker pull couchbase@sha256:24dc913dbba2eaf1690a468e7d0b0ddbf58e6fecaf9a5fbce3105c42b2112ef3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `couchbase:community` - linux; amd64

```console
$ docker pull couchbase@sha256:82f8c9aec3bc79261e8b1e8a29ab23d65bee96d90bf6b6eb2a66d8fa01a4dfe3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **422.2 MB (422209641 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2307dcd4725718311d23366366eda963f9751ee2e048a95b5b8a523dd314243b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Tue, 31 Aug 2021 01:20:55 GMT
ADD file:d2abf27fe2e8b0b5f4da68c018560c73e11c53098329246e3e6fe176698ef941 in / 
# Tue, 31 Aug 2021 01:20:56 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 03:17:15 GMT
LABEL maintainer=docker@couchbase.com
# Tue, 31 Aug 2021 03:17:35 GMT
RUN set -x &&     apt-get update &&     apt-get install -yq runit wget chrpath tzdata     lsof lshw sysstat net-tools numactl bzip2 &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Tue, 31 Aug 2021 03:17:36 GMT
RUN if [ ! -x /usr/sbin/runsvdir-start ]; then         cp -a /etc/runit/2 /usr/sbin/runsvdir-start;     fi
# Tue, 31 Aug 2021 03:17:36 GMT
ARG CB_VERSION=7.0.0
# Tue, 31 Aug 2021 03:17:37 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.0
# Tue, 31 Aug 2021 03:19:11 GMT
ARG CB_PACKAGE=couchbase-server-community_7.0.0-ubuntu20.04_amd64.deb
# Tue, 31 Aug 2021 03:19:11 GMT
ARG CB_SHA256=dd70ca6e45fa40aff5b168aef89509f97eaad5dc2c74c9df7966d28bdc56d917
# Tue, 31 Aug 2021 03:19:11 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Tue, 31 Aug 2021 03:19:12 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.0.0-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.0 CB_SHA256=dd70ca6e45fa40aff5b168aef89509f97eaad5dc2c74c9df7966d28bdc56d917 CB_VERSION=7.0.0
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Tue, 31 Aug 2021 03:19:56 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.0.0-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.0 CB_SHA256=dd70ca6e45fa40aff5b168aef89509f97eaad5dc2c74c9df7966d28bdc56d917 CB_VERSION=7.0.0
RUN set -x &&     export INSTALL_DONT_START_SERVER=1 &&     wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE &&     echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - &&     apt-get update &&     apt-get install -y ./$CB_PACKAGE &&     rm -f ./$CB_PACKAGE &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Tue, 31 Aug 2021 03:20:00 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.0.0-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.0 CB_SHA256=dd70ca6e45fa40aff5b168aef89509f97eaad5dc2c74c9df7966d28bdc56d917 CB_VERSION=7.0.0
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Tue, 31 Aug 2021 03:20:00 GMT
COPY file:d6a307209223b2df102f46f07fd186e09fac7114db2c965bb54097d3b4d3b989 in /etc/service/couchbase-server/run 
# Tue, 31 Aug 2021 03:20:01 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.0.0-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.0 CB_SHA256=dd70ca6e45fa40aff5b168aef89509f97eaad5dc2c74c9df7966d28bdc56d917 CB_VERSION=7.0.0
RUN mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Tue, 31 Aug 2021 03:20:01 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Tue, 31 Aug 2021 03:20:02 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.0.0-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.0 CB_SHA256=dd70ca6e45fa40aff5b168aef89509f97eaad5dc2c74c9df7966d28bdc56d917 CB_VERSION=7.0.0
RUN ln -s dummy.sh /usr/local/bin/iptables-save &&     ln -s dummy.sh /usr/local/bin/lvdisplay &&     ln -s dummy.sh /usr/local/bin/vgdisplay &&     ln -s dummy.sh /usr/local/bin/pvdisplay
# Tue, 31 Aug 2021 03:20:03 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.0.0-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.0 CB_SHA256=dd70ca6e45fa40aff5b168aef89509f97eaad5dc2c74c9df7966d28bdc56d917 CB_VERSION=7.0.0
RUN chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl
# Tue, 31 Aug 2021 03:20:03 GMT
COPY file:d816a67f62bfba76d2812cefbe92252afa13f3852775c3e68599df7741e90cb7 in / 
# Tue, 31 Aug 2021 03:20:03 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 31 Aug 2021 03:20:04 GMT
CMD ["couchbase-server"]
# Tue, 31 Aug 2021 03:20:04 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Tue, 31 Aug 2021 03:20:04 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:35807b77a593c1147d13dc926a91dcc3015616ff7307cc30442c5a8e07546283`  
		Last Modified: Sat, 28 Aug 2021 03:03:19 GMT  
		Size: 28.6 MB (28570074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:909a89f4ffc52b1bc0efc8b382b1da145d18cc3fe8aa349a8c93a0174473f38d`  
		Last Modified: Tue, 31 Aug 2021 03:25:11 GMT  
		Size: 6.3 MB (6265547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:669f46faa4219d00fffdc48350b495c094272d77b1505e7438e9786ced31ff1f`  
		Last Modified: Tue, 31 Aug 2021 03:25:07 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8a62b620335fce18c26fb91910b64876024ecc41ec80acd823f0ec99c34ee62`  
		Last Modified: Tue, 31 Aug 2021 03:26:36 GMT  
		Size: 1.8 KB (1837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:394dc3dd2ddac3da10e4566bb242d5e72c3d72af40a5578826f7865f852248bb`  
		Last Modified: Tue, 31 Aug 2021 03:27:21 GMT  
		Size: 387.2 MB (387243766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28361a37e918d48f8ad486cd0a8ce21f22020219380299510452dde6ce80966c`  
		Last Modified: Tue, 31 Aug 2021 03:26:35 GMT  
		Size: 190.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:451dab312469ffb79ad34ffb6a130d67bd35141c9da160c6fa4686b79f83872b`  
		Last Modified: Tue, 31 Aug 2021 03:26:36 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:413108ff812065b39f2dc49057904690d306509e75eeee98f70ed95a89227737`  
		Last Modified: Tue, 31 Aug 2021 03:26:33 GMT  
		Size: 281.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaddae0cd1c5d50f5eceff8c85c480ba8d15d4a7dd3f844017f15970039c0f20`  
		Last Modified: Tue, 31 Aug 2021 03:26:33 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1a17b87f1fcd6c1bd8e0535f9be8fdfea565b773adbddeb3ed0a32b052f77a7`  
		Last Modified: Tue, 31 Aug 2021 03:26:33 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69eb855a0475602ee5716382aa1f419136c2e88a3c726244f10cb6a929ea3ec9`  
		Last Modified: Tue, 31 Aug 2021 03:26:33 GMT  
		Size: 125.9 KB (125892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8beb3fd3a97c6ccf02668ec412da96c94181aa88fbad86e7471fb4e801158ea`  
		Last Modified: Tue, 31 Aug 2021 03:26:33 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchbase:community-6.6.0`

```console
$ docker pull couchbase@sha256:112625dc0a52fa767d10da4f16effd2d5f5b4d708f30c16c98653a679bb2a289
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `couchbase:community-6.6.0` - linux; amd64

```console
$ docker pull couchbase@sha256:4a29885ce6566911255f7873f72b72d7e927937f9e8556245ae1936f95f19379
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **354.2 MB (354223993 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:76067ef181e26819518d66f7cd289b9a01efe1eb65888c27af69579d62958401`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Tue, 31 Aug 2021 01:20:48 GMT
ADD file:425a053fd043786e9454fb269d4c93c624550fb913a8c96d03ddd430b4e6c1c3 in / 
# Tue, 31 Aug 2021 01:20:48 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 03:21:37 GMT
LABEL maintainer=docker@couchbase.com
# Tue, 31 Aug 2021 03:22:14 GMT
RUN set -x &&     apt-get update &&     apt-get install -yq runit wget chrpath tzdata man     lsof lshw sysstat net-tools numactl bzip2 &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Tue, 31 Aug 2021 03:22:15 GMT
RUN if [ ! -x /usr/sbin/runsvdir-start ]; then         cp -a /etc/runit/2 /usr/sbin/runsvdir-start;     fi
# Tue, 31 Aug 2021 03:22:15 GMT
ARG CB_VERSION=6.6.0
# Tue, 31 Aug 2021 03:22:15 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0
# Tue, 31 Aug 2021 03:22:15 GMT
ARG CB_PACKAGE=couchbase-server-community_6.6.0-ubuntu18.04_amd64.deb
# Tue, 31 Aug 2021 03:22:16 GMT
ARG CB_SHA256=9b196cd7be81d7d6b179838e9d30164fdb7a1f27e96678e61e24e9fe5c93f559
# Tue, 31 Aug 2021 03:22:16 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Tue, 31 Aug 2021 03:22:17 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_6.6.0-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=9b196cd7be81d7d6b179838e9d30164fdb7a1f27e96678e61e24e9fe5c93f559 CB_VERSION=6.6.0
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Tue, 31 Aug 2021 03:22:55 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_6.6.0-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=9b196cd7be81d7d6b179838e9d30164fdb7a1f27e96678e61e24e9fe5c93f559 CB_VERSION=6.6.0
RUN set -x &&     export INSTALL_DONT_START_SERVER=1 &&     wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE &&     echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - &&     apt-get update &&     apt-get install -y ./$CB_PACKAGE &&     rm -f ./$CB_PACKAGE &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Tue, 31 Aug 2021 03:22:58 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_6.6.0-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=9b196cd7be81d7d6b179838e9d30164fdb7a1f27e96678e61e24e9fe5c93f559 CB_VERSION=6.6.0
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Tue, 31 Aug 2021 03:22:58 GMT
COPY file:d6a307209223b2df102f46f07fd186e09fac7114db2c965bb54097d3b4d3b989 in /etc/service/couchbase-server/run 
# Tue, 31 Aug 2021 03:22:59 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_6.6.0-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=9b196cd7be81d7d6b179838e9d30164fdb7a1f27e96678e61e24e9fe5c93f559 CB_VERSION=6.6.0
RUN mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Tue, 31 Aug 2021 03:22:59 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Tue, 31 Aug 2021 03:23:00 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_6.6.0-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=9b196cd7be81d7d6b179838e9d30164fdb7a1f27e96678e61e24e9fe5c93f559 CB_VERSION=6.6.0
RUN ln -s dummy.sh /usr/local/bin/iptables-save &&     ln -s dummy.sh /usr/local/bin/lvdisplay &&     ln -s dummy.sh /usr/local/bin/vgdisplay &&     ln -s dummy.sh /usr/local/bin/pvdisplay
# Tue, 31 Aug 2021 03:23:00 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_6.6.0-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=9b196cd7be81d7d6b179838e9d30164fdb7a1f27e96678e61e24e9fe5c93f559 CB_VERSION=6.6.0
RUN chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl
# Tue, 31 Aug 2021 03:23:01 GMT
COPY file:d816a67f62bfba76d2812cefbe92252afa13f3852775c3e68599df7741e90cb7 in / 
# Tue, 31 Aug 2021 03:23:01 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 31 Aug 2021 03:23:01 GMT
CMD ["couchbase-server"]
# Tue, 31 Aug 2021 03:23:01 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Tue, 31 Aug 2021 03:23:01 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:e4ca327ec0e73c737201b7a6d7b2df779a3ccf34fe9cf1b0c031e767f6464240`  
		Last Modified: Tue, 31 Aug 2021 01:22:00 GMT  
		Size: 26.7 MB (26708511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f3568fede45a221460d4a4be77ba26e77c9a46473d2222007231a9f5330db05`  
		Last Modified: Tue, 31 Aug 2021 03:28:43 GMT  
		Size: 7.4 MB (7374412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3eddc4afd6c8ea74be3ea5e5c50a92e5e456155244fd5b8fdbdae4abe2c97a81`  
		Last Modified: Tue, 31 Aug 2021 03:28:39 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1a85f24a8056215e10d418f76f9428580c631214c82bf7d4f237878f81f675b`  
		Last Modified: Tue, 31 Aug 2021 03:28:38 GMT  
		Size: 2.0 KB (1966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dac496a4ccf145399a0a38180bac726557511e5accef8255097a14ceb3757a88`  
		Last Modified: Tue, 31 Aug 2021 03:29:13 GMT  
		Size: 320.0 MB (320018397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2993d6fb012e37b05cf3d7b4dd419c81a82cb2ac7f8635e2f35f926e232bcfa7`  
		Last Modified: Tue, 31 Aug 2021 03:28:38 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b103b7b10eb12fcb40076fa5162dffe889a3d586d7668c5cbc315f0e85b2bf0`  
		Last Modified: Tue, 31 Aug 2021 03:28:38 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcf4a08383691b8f2a5828e046b9a9298c89db8bfdedc3993ce98826d150664f`  
		Last Modified: Tue, 31 Aug 2021 03:28:36 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85577528d682fceacf82afe1541b01f48ddb62a8219597b0f1f02df5d6801f62`  
		Last Modified: Tue, 31 Aug 2021 03:28:36 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1719b2f11828da91c747313998f3b6fa7d498a475fe253573e2f2f70228c1514`  
		Last Modified: Tue, 31 Aug 2021 03:28:36 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a4b004d16ca85372456965c136f7134b941a69864ff38e38792396388bbb1c9`  
		Last Modified: Tue, 31 Aug 2021 03:28:36 GMT  
		Size: 118.2 KB (118188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fb030634e3e27c0fdefa4d91cfa31fe7cdc010d7d48cfd0cde728283bdd0d79`  
		Last Modified: Tue, 31 Aug 2021 03:28:36 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchbase:community-7.0.1`

**does not exist** (yet?)

## `couchbase:enterprise`

```console
$ docker pull couchbase@sha256:1d5958e7e31427a89b34c3ef3cfaeb12a317d3059eefdc6007b96c99315ecbca
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `couchbase:enterprise` - linux; amd64

```console
$ docker pull couchbase@sha256:ab19f7e9a2dec339e520fadac5fbf5c9d285e914905773af15e5af80876aea45
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **633.1 MB (633079025 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a47887bb55d99c6ff77ed23a48d7c08b17517e38205c61deaa071f12a6fe87ef`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Tue, 31 Aug 2021 01:20:55 GMT
ADD file:d2abf27fe2e8b0b5f4da68c018560c73e11c53098329246e3e6fe176698ef941 in / 
# Tue, 31 Aug 2021 01:20:56 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 03:17:15 GMT
LABEL maintainer=docker@couchbase.com
# Tue, 31 Aug 2021 03:17:35 GMT
RUN set -x &&     apt-get update &&     apt-get install -yq runit wget chrpath tzdata     lsof lshw sysstat net-tools numactl bzip2 &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Tue, 31 Aug 2021 03:17:36 GMT
RUN if [ ! -x /usr/sbin/runsvdir-start ]; then         cp -a /etc/runit/2 /usr/sbin/runsvdir-start;     fi
# Tue, 31 Aug 2021 03:17:36 GMT
ARG CB_VERSION=7.0.0
# Tue, 31 Aug 2021 03:17:37 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.0
# Tue, 31 Aug 2021 03:17:37 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_7.0.0-ubuntu20.04_amd64.deb
# Tue, 31 Aug 2021 03:17:37 GMT
ARG CB_SHA256=6ce174d5ffd22ade6abbf44619e4126c6977635f58f7e08d09553b6b9f8117b7
# Tue, 31 Aug 2021 03:17:37 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Tue, 31 Aug 2021 03:17:38 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.0-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.0 CB_SHA256=6ce174d5ffd22ade6abbf44619e4126c6977635f58f7e08d09553b6b9f8117b7 CB_VERSION=7.0.0
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Tue, 31 Aug 2021 03:18:51 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.0-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.0 CB_SHA256=6ce174d5ffd22ade6abbf44619e4126c6977635f58f7e08d09553b6b9f8117b7 CB_VERSION=7.0.0
RUN set -x &&     export INSTALL_DONT_START_SERVER=1 &&     wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE &&     echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - &&     apt-get update &&     apt-get install -y ./$CB_PACKAGE &&     rm -f ./$CB_PACKAGE &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Tue, 31 Aug 2021 03:18:56 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.0-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.0 CB_SHA256=6ce174d5ffd22ade6abbf44619e4126c6977635f58f7e08d09553b6b9f8117b7 CB_VERSION=7.0.0
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Tue, 31 Aug 2021 03:18:56 GMT
COPY file:d6a307209223b2df102f46f07fd186e09fac7114db2c965bb54097d3b4d3b989 in /etc/service/couchbase-server/run 
# Tue, 31 Aug 2021 03:18:57 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.0-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.0 CB_SHA256=6ce174d5ffd22ade6abbf44619e4126c6977635f58f7e08d09553b6b9f8117b7 CB_VERSION=7.0.0
RUN mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Tue, 31 Aug 2021 03:18:57 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Tue, 31 Aug 2021 03:18:58 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.0-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.0 CB_SHA256=6ce174d5ffd22ade6abbf44619e4126c6977635f58f7e08d09553b6b9f8117b7 CB_VERSION=7.0.0
RUN ln -s dummy.sh /usr/local/bin/iptables-save &&     ln -s dummy.sh /usr/local/bin/lvdisplay &&     ln -s dummy.sh /usr/local/bin/vgdisplay &&     ln -s dummy.sh /usr/local/bin/pvdisplay
# Tue, 31 Aug 2021 03:18:58 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.0-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.0 CB_SHA256=6ce174d5ffd22ade6abbf44619e4126c6977635f58f7e08d09553b6b9f8117b7 CB_VERSION=7.0.0
RUN chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl
# Tue, 31 Aug 2021 03:18:59 GMT
COPY file:d816a67f62bfba76d2812cefbe92252afa13f3852775c3e68599df7741e90cb7 in / 
# Tue, 31 Aug 2021 03:18:59 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 31 Aug 2021 03:18:59 GMT
CMD ["couchbase-server"]
# Tue, 31 Aug 2021 03:18:59 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Tue, 31 Aug 2021 03:19:00 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:35807b77a593c1147d13dc926a91dcc3015616ff7307cc30442c5a8e07546283`  
		Last Modified: Sat, 28 Aug 2021 03:03:19 GMT  
		Size: 28.6 MB (28570074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:909a89f4ffc52b1bc0efc8b382b1da145d18cc3fe8aa349a8c93a0174473f38d`  
		Last Modified: Tue, 31 Aug 2021 03:25:11 GMT  
		Size: 6.3 MB (6265547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:669f46faa4219d00fffdc48350b495c094272d77b1505e7438e9786ced31ff1f`  
		Last Modified: Tue, 31 Aug 2021 03:25:07 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a53f9b2ddfc3ce00356b06b586858b05c8fdab60691fbb96cad5071ffbac765b`  
		Last Modified: Tue, 31 Aug 2021 03:25:07 GMT  
		Size: 1.8 KB (1834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f53522d115fbc68bf09df3876ee4b6b45c363ed5121ff1c91a21b420134c4f5`  
		Last Modified: Tue, 31 Aug 2021 03:26:10 GMT  
		Size: 598.1 MB (598113159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77d1f9b924d9b8d31bf8e1f42941eee07c7ff80d0bbf4603871deba01062a8a1`  
		Last Modified: Tue, 31 Aug 2021 03:25:06 GMT  
		Size: 191.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb68a945837054510edc39f1257b2ef3193b2afb17035c202557e686769404fd`  
		Last Modified: Tue, 31 Aug 2021 03:25:06 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c0637b2abdd1b136a28edd368ec96564d74152c95de7fafa8d12188009c7eef`  
		Last Modified: Tue, 31 Aug 2021 03:25:04 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd5ce4fd6ad511e8d24ce1e11c260dbe3d38422254ae503de847228f1e5b6603`  
		Last Modified: Tue, 31 Aug 2021 03:25:04 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8111e8d7191a575a1a12d65de4cc9cb14fbb4d523d0a11d7a766a2fdf415a21`  
		Last Modified: Tue, 31 Aug 2021 03:25:04 GMT  
		Size: 217.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac33301bae8995be21340628037f93ddf537f43350d0ca71aedb0cb97321a727`  
		Last Modified: Tue, 31 Aug 2021 03:25:04 GMT  
		Size: 125.9 KB (125891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2a266f608eefe10657eb3fb7fea555c6738fff363e95d1383c49eced696c5d6`  
		Last Modified: Tue, 31 Aug 2021 03:25:04 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchbase:enterprise-6.0.5`

```console
$ docker pull couchbase@sha256:98299b065e5be953e2762a65c4a848f0b153c863b9b4831b5c879bb66ab4d86c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `couchbase:enterprise-6.0.5` - linux; amd64

```console
$ docker pull couchbase@sha256:dbe90ce9e946168227833c090d4719986d63aa17e2eb4bb5a73b9c619ed2311f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **466.1 MB (466125041 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1672e6f2e19e654639ea62a998982902461bc803be7694258c54cd3b646c8c22`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Tue, 31 Aug 2021 01:20:48 GMT
ADD file:425a053fd043786e9454fb269d4c93c624550fb913a8c96d03ddd430b4e6c1c3 in / 
# Tue, 31 Aug 2021 01:20:48 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 03:21:37 GMT
LABEL maintainer=docker@couchbase.com
# Tue, 31 Aug 2021 03:23:42 GMT
RUN set -x &&     apt-get update &&     apt-get install -yq runit wget chrpath tzdata man     lsof lshw sysstat net-tools numactl python-httplib2 &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Tue, 31 Aug 2021 03:23:43 GMT
RUN if [ ! -x /usr/sbin/runsvdir-start ]; then         cp -a /etc/runit/2 /usr/sbin/runsvdir-start;     fi
# Tue, 31 Aug 2021 03:23:43 GMT
ARG CB_VERSION=6.0.5
# Tue, 31 Aug 2021 03:23:43 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.5
# Tue, 31 Aug 2021 03:23:43 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_6.0.5-ubuntu18.04_amd64.deb
# Tue, 31 Aug 2021 03:23:43 GMT
ARG CB_SHA256=6b152590867a58d771cffc22774d3cd66c916defcbeeeb339aca8d0a8e6d7f8d
# Tue, 31 Aug 2021 03:23:44 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Tue, 31 Aug 2021 03:23:44 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.5-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.5 CB_SHA256=6b152590867a58d771cffc22774d3cd66c916defcbeeeb339aca8d0a8e6d7f8d CB_VERSION=6.0.5
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Tue, 31 Aug 2021 03:24:33 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.5-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.5 CB_SHA256=6b152590867a58d771cffc22774d3cd66c916defcbeeeb339aca8d0a8e6d7f8d CB_VERSION=6.0.5
RUN set -x &&     export INSTALL_DONT_START_SERVER=1 &&     wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE &&     echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - &&     apt-get update &&     apt-get install -y ./$CB_PACKAGE &&     rm -f ./$CB_PACKAGE &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Tue, 31 Aug 2021 03:24:36 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.5-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.5 CB_SHA256=6b152590867a58d771cffc22774d3cd66c916defcbeeeb339aca8d0a8e6d7f8d CB_VERSION=6.0.5
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Tue, 31 Aug 2021 03:24:36 GMT
COPY file:d6a307209223b2df102f46f07fd186e09fac7114db2c965bb54097d3b4d3b989 in /etc/service/couchbase-server/run 
# Tue, 31 Aug 2021 03:24:37 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.5-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.5 CB_SHA256=6b152590867a58d771cffc22774d3cd66c916defcbeeeb339aca8d0a8e6d7f8d CB_VERSION=6.0.5
RUN mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Tue, 31 Aug 2021 03:24:37 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Tue, 31 Aug 2021 03:24:38 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.5-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.5 CB_SHA256=6b152590867a58d771cffc22774d3cd66c916defcbeeeb339aca8d0a8e6d7f8d CB_VERSION=6.0.5
RUN ln -s dummy.sh /usr/local/bin/iptables-save &&     ln -s dummy.sh /usr/local/bin/lvdisplay &&     ln -s dummy.sh /usr/local/bin/vgdisplay &&     ln -s dummy.sh /usr/local/bin/pvdisplay
# Tue, 31 Aug 2021 03:24:39 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.5-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.5 CB_SHA256=6b152590867a58d771cffc22774d3cd66c916defcbeeeb339aca8d0a8e6d7f8d CB_VERSION=6.0.5
RUN chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl
# Tue, 31 Aug 2021 03:24:39 GMT
COPY file:d816a67f62bfba76d2812cefbe92252afa13f3852775c3e68599df7741e90cb7 in / 
# Tue, 31 Aug 2021 03:24:39 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 31 Aug 2021 03:24:39 GMT
CMD ["couchbase-server"]
# Tue, 31 Aug 2021 03:24:39 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Tue, 31 Aug 2021 03:24:40 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:e4ca327ec0e73c737201b7a6d7b2df779a3ccf34fe9cf1b0c031e767f6464240`  
		Last Modified: Tue, 31 Aug 2021 01:22:00 GMT  
		Size: 26.7 MB (26708511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4ad2462e90bbb875192fc60ad73a37767fd66736c2d77864c1aa1706277e1b8`  
		Last Modified: Tue, 31 Aug 2021 03:29:31 GMT  
		Size: 15.9 MB (15923740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eade3950f0dac395edba948c8a11be6bb13842c0a0bb507d066d3497a8dd7f9`  
		Last Modified: Tue, 31 Aug 2021 03:29:27 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b3385d6562a5a590e21b076d3556b3a9b913f2a4bb301835793cde88d6ad078`  
		Last Modified: Tue, 31 Aug 2021 03:29:27 GMT  
		Size: 2.0 KB (1964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6086cfa42a7e9a96aec888e2245d28d715d9c387136833786b46cc336ef96186`  
		Last Modified: Tue, 31 Aug 2021 03:30:04 GMT  
		Size: 423.4 MB (423362749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:692cbc042cd7250d3bff14a5c3b85c853b497afefc270b93349dbba7501519da`  
		Last Modified: Tue, 31 Aug 2021 03:29:26 GMT  
		Size: 190.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:685784ad28283d623e9acaf2e643630dd7f65d6e792e9e13b69569c3536b6121`  
		Last Modified: Tue, 31 Aug 2021 03:29:26 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:410d54ee1b88dd20786bdb20fb38cd37d8da77195ce4f99e1b6710ee6b529d43`  
		Last Modified: Tue, 31 Aug 2021 03:29:23 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dcf337856e610d54c62aba78828847d0eaa902e745eaaca762084b16972c8b2`  
		Last Modified: Tue, 31 Aug 2021 03:29:24 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44af54e22a6200630e014aa7dc566d5d066d981aa931dcde26108c32a0c6ffd1`  
		Last Modified: Tue, 31 Aug 2021 03:29:23 GMT  
		Size: 217.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ea158ae8b16554d05ce26da1c58f180666d03d25e865f71dd42973f5d7aa6ef`  
		Last Modified: Tue, 31 Aug 2021 03:29:24 GMT  
		Size: 125.6 KB (125561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a055e1c798f0e0dc2dfd3b663ff5c85ef232c924ace8e715277f44d7b5d8967`  
		Last Modified: Tue, 31 Aug 2021 03:29:24 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchbase:enterprise-6.6.3`

```console
$ docker pull couchbase@sha256:0cdced609b593b8b5f73139618c8cc1b67e5adef88adff9339bc9807cb726bdc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `couchbase:enterprise-6.6.3` - linux; amd64

```console
$ docker pull couchbase@sha256:6a7d2b34a79f9d30dcf38c80978811c3cda6d0810d7916772eba8018b70ae176
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **537.4 MB (537352018 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c0fd088ab18fbea2b1c7b7a1c953fed9e3d79a45cc60ce91da437663913e4ed`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Tue, 31 Aug 2021 01:20:55 GMT
ADD file:d2abf27fe2e8b0b5f4da68c018560c73e11c53098329246e3e6fe176698ef941 in / 
# Tue, 31 Aug 2021 01:20:56 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 03:17:15 GMT
LABEL maintainer=docker@couchbase.com
# Tue, 31 Aug 2021 03:17:35 GMT
RUN set -x &&     apt-get update &&     apt-get install -yq runit wget chrpath tzdata     lsof lshw sysstat net-tools numactl bzip2 &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Tue, 31 Aug 2021 03:17:36 GMT
RUN if [ ! -x /usr/sbin/runsvdir-start ]; then         cp -a /etc/runit/2 /usr/sbin/runsvdir-start;     fi
# Tue, 31 Aug 2021 03:20:11 GMT
ARG CB_VERSION=6.6.3
# Tue, 31 Aug 2021 03:20:11 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.3
# Tue, 31 Aug 2021 03:20:12 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_6.6.3-ubuntu20.04_amd64.deb
# Tue, 31 Aug 2021 03:20:12 GMT
ARG CB_SHA256=8d62db9365171aba0ee646c0189b81dec8ef9718fac7b44bd72e15da4e2b38fa
# Tue, 31 Aug 2021 03:20:12 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Tue, 31 Aug 2021 03:20:13 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.3-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.3 CB_SHA256=8d62db9365171aba0ee646c0189b81dec8ef9718fac7b44bd72e15da4e2b38fa CB_VERSION=6.6.3
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Tue, 31 Aug 2021 03:21:16 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.3-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.3 CB_SHA256=8d62db9365171aba0ee646c0189b81dec8ef9718fac7b44bd72e15da4e2b38fa CB_VERSION=6.6.3
RUN set -x &&     export INSTALL_DONT_START_SERVER=1 &&     wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE &&     echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - &&     apt-get update &&     apt-get install -y ./$CB_PACKAGE &&     rm -f ./$CB_PACKAGE &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Tue, 31 Aug 2021 03:21:19 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.3-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.3 CB_SHA256=8d62db9365171aba0ee646c0189b81dec8ef9718fac7b44bd72e15da4e2b38fa CB_VERSION=6.6.3
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Tue, 31 Aug 2021 03:21:19 GMT
COPY file:d6a307209223b2df102f46f07fd186e09fac7114db2c965bb54097d3b4d3b989 in /etc/service/couchbase-server/run 
# Tue, 31 Aug 2021 03:21:20 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.3-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.3 CB_SHA256=8d62db9365171aba0ee646c0189b81dec8ef9718fac7b44bd72e15da4e2b38fa CB_VERSION=6.6.3
RUN mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Tue, 31 Aug 2021 03:21:20 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Tue, 31 Aug 2021 03:21:21 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.3-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.3 CB_SHA256=8d62db9365171aba0ee646c0189b81dec8ef9718fac7b44bd72e15da4e2b38fa CB_VERSION=6.6.3
RUN ln -s dummy.sh /usr/local/bin/iptables-save &&     ln -s dummy.sh /usr/local/bin/lvdisplay &&     ln -s dummy.sh /usr/local/bin/vgdisplay &&     ln -s dummy.sh /usr/local/bin/pvdisplay
# Tue, 31 Aug 2021 03:21:22 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.3-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.3 CB_SHA256=8d62db9365171aba0ee646c0189b81dec8ef9718fac7b44bd72e15da4e2b38fa CB_VERSION=6.6.3
RUN chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl
# Tue, 31 Aug 2021 03:21:22 GMT
COPY file:d816a67f62bfba76d2812cefbe92252afa13f3852775c3e68599df7741e90cb7 in / 
# Tue, 31 Aug 2021 03:21:22 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 31 Aug 2021 03:21:22 GMT
CMD ["couchbase-server"]
# Tue, 31 Aug 2021 03:21:22 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Tue, 31 Aug 2021 03:21:23 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:35807b77a593c1147d13dc926a91dcc3015616ff7307cc30442c5a8e07546283`  
		Last Modified: Sat, 28 Aug 2021 03:03:19 GMT  
		Size: 28.6 MB (28570074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:909a89f4ffc52b1bc0efc8b382b1da145d18cc3fe8aa349a8c93a0174473f38d`  
		Last Modified: Tue, 31 Aug 2021 03:25:11 GMT  
		Size: 6.3 MB (6265547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:669f46faa4219d00fffdc48350b495c094272d77b1505e7438e9786ced31ff1f`  
		Last Modified: Tue, 31 Aug 2021 03:25:07 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a89ac926d4775c8d4f51706c70fe390b5b95b0b12f35c987ad907f59009ee536`  
		Last Modified: Tue, 31 Aug 2021 03:27:35 GMT  
		Size: 1.8 KB (1835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bebb7385ebeec7ff3b3d7c596e2e635943a663ae003a5b0d18e1ae1f89488824`  
		Last Modified: Tue, 31 Aug 2021 03:28:25 GMT  
		Size: 502.4 MB (502386144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1a15fa94f9ecea4ad6dce3368e71f33be66591270ffdb1c422a75b66e147b7a`  
		Last Modified: Tue, 31 Aug 2021 03:27:34 GMT  
		Size: 190.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eeb435a3f6e2b1717eac3ab6303aeff19c9753f4024f38bf901c6914686360bd`  
		Last Modified: Tue, 31 Aug 2021 03:27:34 GMT  
		Size: 479.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a92f45b4fdedce790baf8acf9626db3960dae920c03d1ae18825d0cdc1e5ed06`  
		Last Modified: Tue, 31 Aug 2021 03:27:32 GMT  
		Size: 280.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a044aae35413dcb08801b544e0b334257018690f68a91506ac8cc003b6f3a221`  
		Last Modified: Tue, 31 Aug 2021 03:27:32 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cd9c0021b6ef3531ae150814ece79f5020f50d7021bcaaddedaf17f9a472682`  
		Last Modified: Tue, 31 Aug 2021 03:27:32 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56ed7d9a5135475cb0d2f6da610076dae33f53affb9e19395872138f904651d7`  
		Last Modified: Tue, 31 Aug 2021 03:27:32 GMT  
		Size: 125.9 KB (125891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d335ea28a1383ac0227bb8d1ada6eeec85a791ef7af92bc766ce7069fd5334df`  
		Last Modified: Tue, 31 Aug 2021 03:27:32 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchbase:enterprise-7.0.1`

**does not exist** (yet?)

## `couchbase:latest`

```console
$ docker pull couchbase@sha256:1d5958e7e31427a89b34c3ef3cfaeb12a317d3059eefdc6007b96c99315ecbca
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `couchbase:latest` - linux; amd64

```console
$ docker pull couchbase@sha256:ab19f7e9a2dec339e520fadac5fbf5c9d285e914905773af15e5af80876aea45
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **633.1 MB (633079025 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a47887bb55d99c6ff77ed23a48d7c08b17517e38205c61deaa071f12a6fe87ef`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Tue, 31 Aug 2021 01:20:55 GMT
ADD file:d2abf27fe2e8b0b5f4da68c018560c73e11c53098329246e3e6fe176698ef941 in / 
# Tue, 31 Aug 2021 01:20:56 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 03:17:15 GMT
LABEL maintainer=docker@couchbase.com
# Tue, 31 Aug 2021 03:17:35 GMT
RUN set -x &&     apt-get update &&     apt-get install -yq runit wget chrpath tzdata     lsof lshw sysstat net-tools numactl bzip2 &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Tue, 31 Aug 2021 03:17:36 GMT
RUN if [ ! -x /usr/sbin/runsvdir-start ]; then         cp -a /etc/runit/2 /usr/sbin/runsvdir-start;     fi
# Tue, 31 Aug 2021 03:17:36 GMT
ARG CB_VERSION=7.0.0
# Tue, 31 Aug 2021 03:17:37 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.0
# Tue, 31 Aug 2021 03:17:37 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_7.0.0-ubuntu20.04_amd64.deb
# Tue, 31 Aug 2021 03:17:37 GMT
ARG CB_SHA256=6ce174d5ffd22ade6abbf44619e4126c6977635f58f7e08d09553b6b9f8117b7
# Tue, 31 Aug 2021 03:17:37 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Tue, 31 Aug 2021 03:17:38 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.0-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.0 CB_SHA256=6ce174d5ffd22ade6abbf44619e4126c6977635f58f7e08d09553b6b9f8117b7 CB_VERSION=7.0.0
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Tue, 31 Aug 2021 03:18:51 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.0-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.0 CB_SHA256=6ce174d5ffd22ade6abbf44619e4126c6977635f58f7e08d09553b6b9f8117b7 CB_VERSION=7.0.0
RUN set -x &&     export INSTALL_DONT_START_SERVER=1 &&     wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE &&     echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - &&     apt-get update &&     apt-get install -y ./$CB_PACKAGE &&     rm -f ./$CB_PACKAGE &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Tue, 31 Aug 2021 03:18:56 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.0-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.0 CB_SHA256=6ce174d5ffd22ade6abbf44619e4126c6977635f58f7e08d09553b6b9f8117b7 CB_VERSION=7.0.0
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Tue, 31 Aug 2021 03:18:56 GMT
COPY file:d6a307209223b2df102f46f07fd186e09fac7114db2c965bb54097d3b4d3b989 in /etc/service/couchbase-server/run 
# Tue, 31 Aug 2021 03:18:57 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.0-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.0 CB_SHA256=6ce174d5ffd22ade6abbf44619e4126c6977635f58f7e08d09553b6b9f8117b7 CB_VERSION=7.0.0
RUN mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Tue, 31 Aug 2021 03:18:57 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Tue, 31 Aug 2021 03:18:58 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.0-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.0 CB_SHA256=6ce174d5ffd22ade6abbf44619e4126c6977635f58f7e08d09553b6b9f8117b7 CB_VERSION=7.0.0
RUN ln -s dummy.sh /usr/local/bin/iptables-save &&     ln -s dummy.sh /usr/local/bin/lvdisplay &&     ln -s dummy.sh /usr/local/bin/vgdisplay &&     ln -s dummy.sh /usr/local/bin/pvdisplay
# Tue, 31 Aug 2021 03:18:58 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.0-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.0 CB_SHA256=6ce174d5ffd22ade6abbf44619e4126c6977635f58f7e08d09553b6b9f8117b7 CB_VERSION=7.0.0
RUN chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl
# Tue, 31 Aug 2021 03:18:59 GMT
COPY file:d816a67f62bfba76d2812cefbe92252afa13f3852775c3e68599df7741e90cb7 in / 
# Tue, 31 Aug 2021 03:18:59 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 31 Aug 2021 03:18:59 GMT
CMD ["couchbase-server"]
# Tue, 31 Aug 2021 03:18:59 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Tue, 31 Aug 2021 03:19:00 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:35807b77a593c1147d13dc926a91dcc3015616ff7307cc30442c5a8e07546283`  
		Last Modified: Sat, 28 Aug 2021 03:03:19 GMT  
		Size: 28.6 MB (28570074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:909a89f4ffc52b1bc0efc8b382b1da145d18cc3fe8aa349a8c93a0174473f38d`  
		Last Modified: Tue, 31 Aug 2021 03:25:11 GMT  
		Size: 6.3 MB (6265547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:669f46faa4219d00fffdc48350b495c094272d77b1505e7438e9786ced31ff1f`  
		Last Modified: Tue, 31 Aug 2021 03:25:07 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a53f9b2ddfc3ce00356b06b586858b05c8fdab60691fbb96cad5071ffbac765b`  
		Last Modified: Tue, 31 Aug 2021 03:25:07 GMT  
		Size: 1.8 KB (1834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f53522d115fbc68bf09df3876ee4b6b45c363ed5121ff1c91a21b420134c4f5`  
		Last Modified: Tue, 31 Aug 2021 03:26:10 GMT  
		Size: 598.1 MB (598113159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77d1f9b924d9b8d31bf8e1f42941eee07c7ff80d0bbf4603871deba01062a8a1`  
		Last Modified: Tue, 31 Aug 2021 03:25:06 GMT  
		Size: 191.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb68a945837054510edc39f1257b2ef3193b2afb17035c202557e686769404fd`  
		Last Modified: Tue, 31 Aug 2021 03:25:06 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c0637b2abdd1b136a28edd368ec96564d74152c95de7fafa8d12188009c7eef`  
		Last Modified: Tue, 31 Aug 2021 03:25:04 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd5ce4fd6ad511e8d24ce1e11c260dbe3d38422254ae503de847228f1e5b6603`  
		Last Modified: Tue, 31 Aug 2021 03:25:04 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8111e8d7191a575a1a12d65de4cc9cb14fbb4d523d0a11d7a766a2fdf415a21`  
		Last Modified: Tue, 31 Aug 2021 03:25:04 GMT  
		Size: 217.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac33301bae8995be21340628037f93ddf537f43350d0ca71aedb0cb97321a727`  
		Last Modified: Tue, 31 Aug 2021 03:25:04 GMT  
		Size: 125.9 KB (125891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2a266f608eefe10657eb3fb7fea555c6738fff363e95d1383c49eced696c5d6`  
		Last Modified: Tue, 31 Aug 2021 03:25:04 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
