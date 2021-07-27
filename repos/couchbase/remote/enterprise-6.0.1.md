## `couchbase:enterprise-6.0.1`

```console
$ docker pull couchbase@sha256:33152059c8f0325e94865257494822db62f0cbd4ea07ff54809d5c2f7220ab3b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `couchbase:enterprise-6.0.1` - linux; amd64

```console
$ docker pull couchbase@sha256:eb994494260bba67e8ad1094a0ef2f45806116a27ab2452eab59abd52854784b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **455.2 MB (455214931 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:757245717d3c5546275f8646e84cca7c4354a68d84975b5e4638c41dc58ef654`
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
# Mon, 26 Jul 2021 22:34:27 GMT
ARG CB_VERSION=6.0.1
# Mon, 26 Jul 2021 22:34:27 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.1
# Mon, 26 Jul 2021 22:34:27 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_6.0.1-ubuntu18.04_amd64.deb
# Mon, 26 Jul 2021 22:34:27 GMT
ARG CB_SHA256=68deed9ba855e2a84500ae99a787c415fc85b4d4dc1140be28ae6f56662bafea
# Mon, 26 Jul 2021 22:34:28 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Mon, 26 Jul 2021 22:34:28 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.1-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.1 CB_SHA256=68deed9ba855e2a84500ae99a787c415fc85b4d4dc1140be28ae6f56662bafea CB_VERSION=6.0.1
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Mon, 26 Jul 2021 22:35:26 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.1-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.1 CB_SHA256=68deed9ba855e2a84500ae99a787c415fc85b4d4dc1140be28ae6f56662bafea CB_VERSION=6.0.1
RUN set -x &&     export INSTALL_DONT_START_SERVER=1 &&     wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE &&     echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - &&     apt-get update &&     apt-get install -y ./$CB_PACKAGE &&     rm -f ./$CB_PACKAGE &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Mon, 26 Jul 2021 22:35:29 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.1-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.1 CB_SHA256=68deed9ba855e2a84500ae99a787c415fc85b4d4dc1140be28ae6f56662bafea CB_VERSION=6.0.1
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Mon, 26 Jul 2021 22:35:29 GMT
COPY file:d6a307209223b2df102f46f07fd186e09fac7114db2c965bb54097d3b4d3b989 in /etc/service/couchbase-server/run 
# Mon, 26 Jul 2021 22:35:30 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.1-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.1 CB_SHA256=68deed9ba855e2a84500ae99a787c415fc85b4d4dc1140be28ae6f56662bafea CB_VERSION=6.0.1
RUN mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Mon, 26 Jul 2021 22:35:30 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Mon, 26 Jul 2021 22:35:31 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.1-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.1 CB_SHA256=68deed9ba855e2a84500ae99a787c415fc85b4d4dc1140be28ae6f56662bafea CB_VERSION=6.0.1
RUN ln -s dummy.sh /usr/local/bin/iptables-save &&     ln -s dummy.sh /usr/local/bin/lvdisplay &&     ln -s dummy.sh /usr/local/bin/vgdisplay &&     ln -s dummy.sh /usr/local/bin/pvdisplay
# Mon, 26 Jul 2021 22:35:32 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.1-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.1 CB_SHA256=68deed9ba855e2a84500ae99a787c415fc85b4d4dc1140be28ae6f56662bafea CB_VERSION=6.0.1
RUN chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl
# Mon, 26 Jul 2021 22:35:32 GMT
COPY file:d816a67f62bfba76d2812cefbe92252afa13f3852775c3e68599df7741e90cb7 in / 
# Mon, 26 Jul 2021 22:35:32 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 26 Jul 2021 22:35:32 GMT
CMD ["couchbase-server"]
# Mon, 26 Jul 2021 22:35:32 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Mon, 26 Jul 2021 22:35:33 GMT
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
	-	`sha256:2cd2998f9f5572111f397f86320964084ff27496510b3f207f2abbd03f280290`  
		Last Modified: Mon, 26 Jul 2021 22:51:25 GMT  
		Size: 2.0 KB (1966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0be5d397f140f7be638b55fc8b192db79f2054c786d19231e732c4b739f611d1`  
		Last Modified: Mon, 26 Jul 2021 22:52:19 GMT  
		Size: 412.5 MB (412452893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03beda794fda7c5d8a531ae36fe1e3bffe5f104c2efcf68bd401eb2c5685eb6f`  
		Last Modified: Mon, 26 Jul 2021 22:51:25 GMT  
		Size: 190.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b3c1409fb418a4d13bcfd92f6c4408f3512059f0453ecee7c03f55c34ce9c52`  
		Last Modified: Mon, 26 Jul 2021 22:51:25 GMT  
		Size: 479.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d80b35c3d361b4c92cefe6a3bb490b5b7591bc5b7b392a0ae6a6f81c46c0f07`  
		Last Modified: Mon, 26 Jul 2021 22:51:22 GMT  
		Size: 280.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6de0d3e36daec3a43bdf425331781a96ac6410418cc148519da3b640f692dcb5`  
		Last Modified: Mon, 26 Jul 2021 22:51:22 GMT  
		Size: 235.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66b0ad6fef042a063da298d8a62d3eaca3d3e59fe4df6df1439e9d347bdfe701`  
		Last Modified: Mon, 26 Jul 2021 22:51:22 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c336a662e1c94b1c42448c50343c47f2afcba4e640e5b9a9e6b6331fdb8ba5bc`  
		Last Modified: Mon, 26 Jul 2021 22:51:22 GMT  
		Size: 125.6 KB (125560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6156f367f101d52bf75f7ad0fed3d8554098a13c50178a7fdac410967b50f541`  
		Last Modified: Mon, 26 Jul 2021 22:51:22 GMT  
		Size: 858.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
