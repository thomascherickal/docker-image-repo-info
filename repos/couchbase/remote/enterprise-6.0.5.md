## `couchbase:enterprise-6.0.5`

```console
$ docker pull couchbase@sha256:cd885801bbd0a2baba91b1a96e127a05f05b263ccf8c61152d5228963cf86936
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `couchbase:enterprise-6.0.5` - linux; amd64

```console
$ docker pull couchbase@sha256:dc2d6c0025db1f53228dd23902857c4c499c4bacc598ca57f311730619629c52
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **466.1 MB (466121367 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c0f0d275e916577f8a04db8a1b908776a84ed1dffbeb0e64e2c535b8294bf7d8`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Tue, 05 Apr 2022 22:20:42 GMT
ADD file:8a4ddbd462c1dd2016c64bd71ea6b5dba2ac4934bfd235a04d55b364666b67d1 in / 
# Tue, 05 Apr 2022 22:20:43 GMT
CMD ["bash"]
# Tue, 05 Apr 2022 23:20:02 GMT
LABEL maintainer=docker@couchbase.com
# Tue, 05 Apr 2022 23:23:03 GMT
RUN set -x &&     apt-get update &&     apt-get install -yq runit wget chrpath tzdata man     lsof lshw sysstat net-tools numactl python-httplib2 &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Tue, 05 Apr 2022 23:23:03 GMT
RUN if [ ! -x /usr/sbin/runsvdir-start ]; then         cp -a /etc/runit/2 /usr/sbin/runsvdir-start;     fi
# Tue, 05 Apr 2022 23:23:03 GMT
ARG CB_VERSION=6.0.5
# Tue, 05 Apr 2022 23:23:04 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.5
# Tue, 05 Apr 2022 23:23:04 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_6.0.5-ubuntu18.04_amd64.deb
# Tue, 05 Apr 2022 23:23:04 GMT
ARG CB_SHA256=6b152590867a58d771cffc22774d3cd66c916defcbeeeb339aca8d0a8e6d7f8d
# Tue, 05 Apr 2022 23:23:04 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Tue, 05 Apr 2022 23:23:04 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.5-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.5 CB_SHA256=6b152590867a58d771cffc22774d3cd66c916defcbeeeb339aca8d0a8e6d7f8d CB_VERSION=6.0.5
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Tue, 05 Apr 2022 23:23:59 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.5-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.5 CB_SHA256=6b152590867a58d771cffc22774d3cd66c916defcbeeeb339aca8d0a8e6d7f8d CB_VERSION=6.0.5
RUN set -x &&     export INSTALL_DONT_START_SERVER=1 &&     wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE &&     echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - &&     apt-get update &&     apt-get install -y ./$CB_PACKAGE &&     rm -f ./$CB_PACKAGE &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Tue, 05 Apr 2022 23:24:02 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.5-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.5 CB_SHA256=6b152590867a58d771cffc22774d3cd66c916defcbeeeb339aca8d0a8e6d7f8d CB_VERSION=6.0.5
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Tue, 05 Apr 2022 23:24:02 GMT
COPY file:d6a307209223b2df102f46f07fd186e09fac7114db2c965bb54097d3b4d3b989 in /etc/service/couchbase-server/run 
# Tue, 05 Apr 2022 23:24:02 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.5-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.5 CB_SHA256=6b152590867a58d771cffc22774d3cd66c916defcbeeeb339aca8d0a8e6d7f8d CB_VERSION=6.0.5
RUN mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Tue, 05 Apr 2022 23:24:03 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Tue, 05 Apr 2022 23:24:03 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.5-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.5 CB_SHA256=6b152590867a58d771cffc22774d3cd66c916defcbeeeb339aca8d0a8e6d7f8d CB_VERSION=6.0.5
RUN ln -s dummy.sh /usr/local/bin/iptables-save &&     ln -s dummy.sh /usr/local/bin/lvdisplay &&     ln -s dummy.sh /usr/local/bin/vgdisplay &&     ln -s dummy.sh /usr/local/bin/pvdisplay
# Tue, 05 Apr 2022 23:24:04 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.5-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.5 CB_SHA256=6b152590867a58d771cffc22774d3cd66c916defcbeeeb339aca8d0a8e6d7f8d CB_VERSION=6.0.5
RUN chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl
# Tue, 05 Apr 2022 23:24:04 GMT
COPY file:d816a67f62bfba76d2812cefbe92252afa13f3852775c3e68599df7741e90cb7 in / 
# Tue, 05 Apr 2022 23:24:04 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 05 Apr 2022 23:24:04 GMT
CMD ["couchbase-server"]
# Tue, 05 Apr 2022 23:24:04 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Tue, 05 Apr 2022 23:24:04 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:08a6abff89437fab99b52abbefed82ea907f12845c30eeb94f6b93c69be93166`  
		Last Modified: Tue, 05 Apr 2022 13:10:59 GMT  
		Size: 26.7 MB (26708938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a23fa2871d969daefc06c3ea472b580809aadbd7729326a061f75a5ba07e3344`  
		Last Modified: Tue, 05 Apr 2022 23:28:17 GMT  
		Size: 15.9 MB (15919314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19b9502dfde6f5c587ab139f70c96c68210abce12f38896370549a06a0ff1c65`  
		Last Modified: Tue, 05 Apr 2022 23:28:12 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3fb9cca7ec445e4d5701a7522e7f7b94781ef1d797e6a2e6e70952010b63b44`  
		Last Modified: Tue, 05 Apr 2022 23:28:12 GMT  
		Size: 2.0 KB (1962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3294366258eaa730467600398870288d2b636f5876f0a6ca28ec986faed42348`  
		Last Modified: Tue, 05 Apr 2022 23:28:49 GMT  
		Size: 423.4 MB (423363066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c721af9ac48daebb1e82e601075dde102ffb9dd4c72c3e9edebae15aff0d0adb`  
		Last Modified: Tue, 05 Apr 2022 23:28:12 GMT  
		Size: 192.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b28ed14537b0472887e67feda0ce0d26a7878f210e4518527d2292a3d1524f8`  
		Last Modified: Tue, 05 Apr 2022 23:28:12 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a550b3e2de587f059c7160dd6105f3461a9f002f4a8937aa7b87adbc8624ff4`  
		Last Modified: Tue, 05 Apr 2022 23:28:09 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc07ab9bf6004feb0b5b84afb89689c31644d1655dd3f067258404f21ee052ef`  
		Last Modified: Tue, 05 Apr 2022 23:28:09 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cc287a2b6d59d3cd91b28d52891e5938f42bcfb47921a3e1981beb1dc7c70a0`  
		Last Modified: Tue, 05 Apr 2022 23:28:09 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7852a25d0d395675e8fca4b474f7426fc55abfa720cbb22a01c9d545eb0ae99d`  
		Last Modified: Tue, 05 Apr 2022 23:28:09 GMT  
		Size: 125.6 KB (125562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:936782c07cbc65be722f35c29013d983023b11a2447ad0ccbfc901fa6d1de705`  
		Last Modified: Tue, 05 Apr 2022 23:28:09 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
