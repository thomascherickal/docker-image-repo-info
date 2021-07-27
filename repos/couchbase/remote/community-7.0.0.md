## `couchbase:community-7.0.0`

```console
$ docker pull couchbase@sha256:5209e8a3f6d820f51156b2d42022f1ad9ed307d06bed98200e9640104bc6903c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `couchbase:community-7.0.0` - linux; amd64

```console
$ docker pull couchbase@sha256:1596930a8d36d5ccab44257d51e12b2af353f43b4c0578df69c0cf7a747be928
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **422.2 MB (422213968 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb087be1f30a05c7a561653462f48398876552d038d6dfa0d8033bd565345108`
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
# Tue, 27 Jul 2021 19:21:17 GMT
ARG CB_PACKAGE=couchbase-server-community_7.0.0-ubuntu20.04_amd64.deb
# Tue, 27 Jul 2021 19:21:17 GMT
ARG CB_SHA256=dd70ca6e45fa40aff5b168aef89509f97eaad5dc2c74c9df7966d28bdc56d917
# Tue, 27 Jul 2021 19:21:17 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Tue, 27 Jul 2021 19:21:18 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.0.0-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.0 CB_SHA256=dd70ca6e45fa40aff5b168aef89509f97eaad5dc2c74c9df7966d28bdc56d917 CB_VERSION=7.0.0
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Tue, 27 Jul 2021 19:22:06 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.0.0-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.0 CB_SHA256=dd70ca6e45fa40aff5b168aef89509f97eaad5dc2c74c9df7966d28bdc56d917 CB_VERSION=7.0.0
RUN set -x &&     export INSTALL_DONT_START_SERVER=1 &&     wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE &&     echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - &&     apt-get update &&     apt-get install -y ./$CB_PACKAGE &&     rm -f ./$CB_PACKAGE &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Tue, 27 Jul 2021 19:22:10 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.0.0-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.0 CB_SHA256=dd70ca6e45fa40aff5b168aef89509f97eaad5dc2c74c9df7966d28bdc56d917 CB_VERSION=7.0.0
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Tue, 27 Jul 2021 19:22:10 GMT
COPY file:d6a307209223b2df102f46f07fd186e09fac7114db2c965bb54097d3b4d3b989 in /etc/service/couchbase-server/run 
# Tue, 27 Jul 2021 19:22:11 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.0.0-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.0 CB_SHA256=dd70ca6e45fa40aff5b168aef89509f97eaad5dc2c74c9df7966d28bdc56d917 CB_VERSION=7.0.0
RUN mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Tue, 27 Jul 2021 19:22:11 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Tue, 27 Jul 2021 19:22:12 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.0.0-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.0 CB_SHA256=dd70ca6e45fa40aff5b168aef89509f97eaad5dc2c74c9df7966d28bdc56d917 CB_VERSION=7.0.0
RUN ln -s dummy.sh /usr/local/bin/iptables-save &&     ln -s dummy.sh /usr/local/bin/lvdisplay &&     ln -s dummy.sh /usr/local/bin/vgdisplay &&     ln -s dummy.sh /usr/local/bin/pvdisplay
# Tue, 27 Jul 2021 19:22:12 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.0.0-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.0 CB_SHA256=dd70ca6e45fa40aff5b168aef89509f97eaad5dc2c74c9df7966d28bdc56d917 CB_VERSION=7.0.0
RUN chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl
# Tue, 27 Jul 2021 19:22:13 GMT
COPY file:d816a67f62bfba76d2812cefbe92252afa13f3852775c3e68599df7741e90cb7 in / 
# Tue, 27 Jul 2021 19:22:13 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 27 Jul 2021 19:22:13 GMT
CMD ["couchbase-server"]
# Tue, 27 Jul 2021 19:22:13 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Tue, 27 Jul 2021 19:22:13 GMT
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
	-	`sha256:a1cf83af44430a71943715b43e7c8f87d6ce82d8bdb88192cc20b73a87b43f33`  
		Last Modified: Tue, 27 Jul 2021 19:24:04 GMT  
		Size: 1.8 KB (1840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39aaeb2cc13bed178c9e5e91c6ba3ecf54abb4454f39364d358a700f69d05bac`  
		Last Modified: Tue, 27 Jul 2021 19:24:50 GMT  
		Size: 387.2 MB (387243194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cde7395f0568ff1c42d851212ce76a4f9bf40ec9a71afb1952aae67fc7bed1aa`  
		Last Modified: Tue, 27 Jul 2021 19:24:04 GMT  
		Size: 191.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f38df88bcf23d7f037db5fc4e006badc005366761c3c1cf420c3c7774f17f030`  
		Last Modified: Tue, 27 Jul 2021 19:24:04 GMT  
		Size: 482.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2d04a1e99ea14c12b42d9753fc2fdb631bdbbc9fff53fc6eab1ed040f779383`  
		Last Modified: Tue, 27 Jul 2021 19:24:02 GMT  
		Size: 281.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54719ccd40bb0f33aea8d0a9c5df90325fb22efae883c578ac83f0de97750248`  
		Last Modified: Tue, 27 Jul 2021 19:24:02 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20a2045c058ad8acb998220d05cbf9de249e96103ed80d428da13e49913b6bf5`  
		Last Modified: Tue, 27 Jul 2021 19:24:02 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7ad80e471e34c27ed65fa8e3fde09a29a6cdaec8853d1df31d959a6915b8b9a`  
		Last Modified: Tue, 27 Jul 2021 19:24:02 GMT  
		Size: 125.9 KB (125892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:189da50f7a164483d6c24dcbc7c1a374400c56482cef8b36cd5652beb9b0b910`  
		Last Modified: Tue, 27 Jul 2021 19:24:02 GMT  
		Size: 856.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
