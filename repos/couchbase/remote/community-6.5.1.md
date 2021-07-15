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
