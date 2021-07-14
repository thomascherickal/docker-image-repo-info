## `couchbase:enterprise-6.5.0`

```console
$ docker pull couchbase@sha256:1c2654f480ef8427c0362829bdb0e6bda8645489ae87ddf0c7eb4424d43926de
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
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
