## `couchbase:enterprise`

```console
$ docker pull couchbase@sha256:892398f3ecab1a5d543edd8d5b4231cb8c8889febb54cdb31d3adf17a4a5e3d2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `couchbase:enterprise` - linux; amd64

```console
$ docker pull couchbase@sha256:3048b0d0d034240cd30a8a686377899630a08db901bce52b34d15c149b1ac925
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **653.6 MB (653562786 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0344c44e7e0b7600bba3b1d9a95eb9d9107b1360ebb130fd52ae329177534866`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Fri, 18 Mar 2022 05:30:40 GMT
ADD file:1d3b09cf9e041d608a00c2dc25cdf3c388e436c5db607a3d124f2aa0f764fc69 in / 
# Fri, 18 Mar 2022 05:30:40 GMT
CMD ["bash"]
# Sat, 19 Mar 2022 22:36:59 GMT
LABEL maintainer=docker@couchbase.com
# Sat, 19 Mar 2022 22:36:59 GMT
ARG UPDATE_COMMAND=apt-get update -y -q
# Sat, 19 Mar 2022 22:36:59 GMT
ARG CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Sat, 19 Mar 2022 22:37:20 GMT
# ARGS: CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ${UPDATE_COMMAND}     && apt-get install -y -q wget tzdata       lsof lshw sysstat net-tools numactl bzip2 runit     && ${CLEANUP_COMMAND}
# Sat, 19 Mar 2022 22:37:20 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.3-MP1
# Sat, 19 Mar 2022 22:37:20 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_7.0.3-MP1-ubuntu20.04_amd64.deb
# Sat, 19 Mar 2022 22:37:20 GMT
ARG CB_SHA256=a1bfcc476e01c71a212c2ed5026f24f3df01b3591c24dcf45678fdb2625cfc0f
# Sat, 19 Mar 2022 22:37:20 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Sat, 19 Mar 2022 22:37:21 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.3-MP1-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.3-MP1 CB_SHA256=a1bfcc476e01c71a212c2ed5026f24f3df01b3591c24dcf45678fdb2625cfc0f CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Sat, 19 Mar 2022 22:38:27 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.3-MP1-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.3-MP1 CB_SHA256=a1bfcc476e01c71a212c2ed5026f24f3df01b3591c24dcf45678fdb2625cfc0f CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && export INSTALL_DONT_START_SERVER=1     && wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE     && echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c -     && ${UPDATE_COMMAND}     && apt-get install -y ./$CB_PACKAGE     && rm -f ./$CB_PACKAGE     && ${CLEANUP_COMMAND}     && rm -rf /tmp/* /var/tmp/*
# Sat, 19 Mar 2022 22:38:29 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.3-MP1-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.3-MP1 CB_SHA256=a1bfcc476e01c71a212c2ed5026f24f3df01b3591c24dcf45678fdb2625cfc0f CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Sat, 19 Mar 2022 22:38:29 GMT
COPY file:018fa38d92aa0a4679f57c2d43b5c14547b2c603cab6ec7fd3240af5545472b5 in /etc/service/couchbase-server/run 
# Sat, 19 Mar 2022 22:38:30 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.3-MP1-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.3-MP1 CB_SHA256=a1bfcc476e01c71a212c2ed5026f24f3df01b3591c24dcf45678fdb2625cfc0f CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Sat, 19 Mar 2022 22:38:30 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Sat, 19 Mar 2022 22:38:31 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.3-MP1-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.3-MP1 CB_SHA256=a1bfcc476e01c71a212c2ed5026f24f3df01b3591c24dcf45678fdb2625cfc0f CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ln -s dummy.sh /usr/local/bin/iptables-save     && ln -s dummy.sh /usr/local/bin/lvdisplay     && ln -s dummy.sh /usr/local/bin/vgdisplay     && ln -s dummy.sh /usr/local/bin/pvdisplay
# Sat, 19 Mar 2022 22:38:37 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.3-MP1-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.3-MP1 CB_SHA256=a1bfcc476e01c71a212c2ed5026f24f3df01b3591c24dcf45678fdb2625cfc0f CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -ex     &&  if [ ! -e /opt/couchbase/bin/curl.real ]; then             ${UPDATE_COMMAND};             apt-get install -y chrpath;             chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl;             apt-get remove -y chrpath;             apt-get autoremove -y;             ${CLEANUP_COMMAND};         fi
# Sat, 19 Mar 2022 22:38:38 GMT
COPY file:6e5292e89c7124e038a0d80ea3b942bff1ed578e67a07e764b041ea95b129aa3 in / 
# Sat, 19 Mar 2022 22:38:38 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 19 Mar 2022 22:38:38 GMT
CMD ["couchbase-server"]
# Sat, 19 Mar 2022 22:38:38 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Sat, 19 Mar 2022 22:38:38 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:4d32b49e2995210e8937f0898327f196d3fcc52486f0be920e8b2d65f150a7ab`  
		Last Modified: Thu, 17 Mar 2022 11:55:39 GMT  
		Size: 28.6 MB (28565909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86529d73905e42bcf85f4b77874345ada783cdcf2868034ead07a8ebab8dd789`  
		Last Modified: Sat, 19 Mar 2022 22:46:58 GMT  
		Size: 6.3 MB (6251549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c7d16a033e8dd40e907e5a31cfcac287a02f476f21256b3e6c3a6f048101ef0`  
		Last Modified: Sat, 19 Mar 2022 22:46:57 GMT  
		Size: 1.8 KB (1836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1c7f80e065cacf5165f173dc46921fca9ff927173695096f1cf74ce0186aa1a`  
		Last Modified: Sat, 19 Mar 2022 22:48:00 GMT  
		Size: 618.3 MB (618297521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b3fe1cc1903f71f6475af05b20a14b714f8f2ccff126b3de58cad24bda0dadc`  
		Last Modified: Sat, 19 Mar 2022 22:46:57 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d12602f49e8743ef855fcdf69aac765ca8348565d5d2bdac93904926686e07d`  
		Last Modified: Sat, 19 Mar 2022 22:46:57 GMT  
		Size: 742.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0551f258f170ac3f88cc8c6ecc5d3a0e6f8daafa62fde996f950402a54fdb0a2`  
		Last Modified: Sat, 19 Mar 2022 22:46:55 GMT  
		Size: 279.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:501021cf157ccf8cce3344a4b7ea813fcc1c934e35e3b65efdb43ca04c78948f`  
		Last Modified: Sat, 19 Mar 2022 22:46:55 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:380b52d30fcc401cbe074688e3c968ff821e31832a15379503b160c57af595f8`  
		Last Modified: Sat, 19 Mar 2022 22:46:55 GMT  
		Size: 215.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9db7941619fb7d91c3a26b5145fb15df2acf931c2371c3493aa2e5790364cdf`  
		Last Modified: Sat, 19 Mar 2022 22:46:55 GMT  
		Size: 443.4 KB (443444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cff92b53f697a3cf767acfe8909856cd1abf34e9a046001486b38c8e928b5ee7`  
		Last Modified: Sat, 19 Mar 2022 22:46:55 GMT  
		Size: 867.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
