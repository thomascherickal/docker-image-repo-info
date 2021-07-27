## `couchbase:enterprise-7.0.0`

```console
$ docker pull couchbase@sha256:005fb3ba97c2362b9ccc9d96f0d94bf09c2fe784d889fe71c5a2ba475e4645a4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `couchbase:enterprise-7.0.0` - linux; amd64

```console
$ docker pull couchbase@sha256:f2a81b4271f0bdec4d2e5f8f2b9e9febced79048b4cd9c144ff3b832272ba76e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **633.1 MB (633083217 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9022428339d4615af519685439630f4532bb43a64f4c82f29c299271e16d0e56`
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
# Tue, 27 Jul 2021 19:19:36 GMT
ARG CB_VERSION=7.0.0
# Tue, 27 Jul 2021 19:19:36 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.0
# Tue, 27 Jul 2021 19:19:37 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_7.0.0-ubuntu20.04_amd64.deb
# Tue, 27 Jul 2021 19:19:37 GMT
ARG CB_SHA256=6ce174d5ffd22ade6abbf44619e4126c6977635f58f7e08d09553b6b9f8117b7
# Tue, 27 Jul 2021 19:19:37 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Tue, 27 Jul 2021 19:19:38 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.0-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.0 CB_SHA256=6ce174d5ffd22ade6abbf44619e4126c6977635f58f7e08d09553b6b9f8117b7 CB_VERSION=7.0.0
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Tue, 27 Jul 2021 19:20:52 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.0-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.0 CB_SHA256=6ce174d5ffd22ade6abbf44619e4126c6977635f58f7e08d09553b6b9f8117b7 CB_VERSION=7.0.0
RUN set -x &&     export INSTALL_DONT_START_SERVER=1 &&     wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE &&     echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - &&     apt-get update &&     apt-get install -y ./$CB_PACKAGE &&     rm -f ./$CB_PACKAGE &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Tue, 27 Jul 2021 19:20:58 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.0-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.0 CB_SHA256=6ce174d5ffd22ade6abbf44619e4126c6977635f58f7e08d09553b6b9f8117b7 CB_VERSION=7.0.0
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Tue, 27 Jul 2021 19:20:58 GMT
COPY file:d6a307209223b2df102f46f07fd186e09fac7114db2c965bb54097d3b4d3b989 in /etc/service/couchbase-server/run 
# Tue, 27 Jul 2021 19:20:59 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.0-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.0 CB_SHA256=6ce174d5ffd22ade6abbf44619e4126c6977635f58f7e08d09553b6b9f8117b7 CB_VERSION=7.0.0
RUN mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Tue, 27 Jul 2021 19:20:59 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Tue, 27 Jul 2021 19:21:00 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.0-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.0 CB_SHA256=6ce174d5ffd22ade6abbf44619e4126c6977635f58f7e08d09553b6b9f8117b7 CB_VERSION=7.0.0
RUN ln -s dummy.sh /usr/local/bin/iptables-save &&     ln -s dummy.sh /usr/local/bin/lvdisplay &&     ln -s dummy.sh /usr/local/bin/vgdisplay &&     ln -s dummy.sh /usr/local/bin/pvdisplay
# Tue, 27 Jul 2021 19:21:00 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.0-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.0 CB_SHA256=6ce174d5ffd22ade6abbf44619e4126c6977635f58f7e08d09553b6b9f8117b7 CB_VERSION=7.0.0
RUN chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl
# Tue, 27 Jul 2021 19:21:01 GMT
COPY file:d816a67f62bfba76d2812cefbe92252afa13f3852775c3e68599df7741e90cb7 in / 
# Tue, 27 Jul 2021 19:21:01 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 27 Jul 2021 19:21:01 GMT
CMD ["couchbase-server"]
# Tue, 27 Jul 2021 19:21:01 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Tue, 27 Jul 2021 19:21:01 GMT
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
	-	`sha256:a6cdc5f71c3710468544fa224018c4a47ccf6c406ead41085cedf89ef99d1775`  
		Last Modified: Tue, 27 Jul 2021 19:22:41 GMT  
		Size: 1.8 KB (1842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e678d3290280e91fe94b0fc2b0faff059cab446516e5fb869856421c7001f4e`  
		Last Modified: Tue, 27 Jul 2021 19:23:43 GMT  
		Size: 598.1 MB (598112447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6969abcd0ca4371e2769bc97077e2f43ced0451abd159601e138e1edf5b1e283`  
		Last Modified: Tue, 27 Jul 2021 19:22:41 GMT  
		Size: 191.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3aa359b4f22f914a20e211ae281fe312fe947736087893320e7c6543ccae9be`  
		Last Modified: Tue, 27 Jul 2021 19:22:41 GMT  
		Size: 480.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07230fb0fa2e887a74bad436262a80d194b7ffe238041586fd2b4130b1e9c0d9`  
		Last Modified: Tue, 27 Jul 2021 19:22:38 GMT  
		Size: 282.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9404dfab9613ac5843b1093f86d2cbaba3da74f61f3f5afb689f34b58298c55a`  
		Last Modified: Tue, 27 Jul 2021 19:22:39 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e73844eba4f0814d5e3f122bcd4fe4af5b787a43cad92054aa50926896fea85`  
		Last Modified: Tue, 27 Jul 2021 19:22:39 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90ce7876a709925e51b4b5d0cee4cf4e000bf2bda2719984b15d8977e5256d50`  
		Last Modified: Tue, 27 Jul 2021 19:22:38 GMT  
		Size: 125.9 KB (125889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10f13caac7cd9de24759a20e590d18b3ce3c085c8ce971e0a023b96f4ed12c4f`  
		Last Modified: Tue, 27 Jul 2021 19:22:38 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
