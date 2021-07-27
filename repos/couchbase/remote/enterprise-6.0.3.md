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
