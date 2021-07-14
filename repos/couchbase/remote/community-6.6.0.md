## `couchbase:community-6.6.0`

```console
$ docker pull couchbase@sha256:a3b49c114e2c940ee412c4039120168389e52f4e351c81d2950f2e38f32fe7bf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
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
