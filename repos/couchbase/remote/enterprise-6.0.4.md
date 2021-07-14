## `couchbase:enterprise-6.0.4`

```console
$ docker pull couchbase@sha256:b9898e94785b49ddba89e600193dde03e616a41e01676a743dbfb57f4c4d8110
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
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
