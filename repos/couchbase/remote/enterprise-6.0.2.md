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
