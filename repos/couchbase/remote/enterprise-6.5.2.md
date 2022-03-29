## `couchbase:enterprise-6.5.2`

```console
$ docker pull couchbase@sha256:5e39134e583c7c30ba4e5b7c6b14209fda3f02e8710b11c86af89a1644cea8e3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `couchbase:enterprise-6.5.2` - linux; amd64

```console
$ docker pull couchbase@sha256:44f4077235027539095c8de7e450581bca30057f3742c7c9176fcaa28255675f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **503.8 MB (503759626 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:da0c263bf8a51f543e347d524c71df9b376d23c43542707e7609760bc11d293f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Fri, 18 Mar 2022 05:30:26 GMT
ADD file:f554512cb0acad99508554656767804e4821ece488fac0e46fd2c643a39f7021 in / 
# Fri, 18 Mar 2022 05:30:27 GMT
CMD ["bash"]
# Sat, 19 Mar 2022 22:42:52 GMT
LABEL maintainer=docker@couchbase.com
# Mon, 28 Mar 2022 22:24:52 GMT
ARG UPDATE_COMMAND=apt-get update -y -q
# Mon, 28 Mar 2022 22:24:52 GMT
ARG CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Mon, 28 Mar 2022 22:25:01 GMT
# ARGS: CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ${UPDATE_COMMAND}     && apt-get install -y -q wget tzdata       lsof lshw sysstat net-tools numactl bzip2 runit     && ${CLEANUP_COMMAND}
# Mon, 28 Mar 2022 22:25:01 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/6.5.2
# Mon, 28 Mar 2022 22:25:01 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_6.5.2-ubuntu18.04_amd64.deb
# Mon, 28 Mar 2022 22:25:02 GMT
ARG CB_PACKAGE_NAME=couchbase-server
# Mon, 28 Mar 2022 22:25:02 GMT
ARG CB_SHA256=62f9ffad86eab90137701baab421586af49fe0e7c458bb047b6c364c6ad11684
# Mon, 28 Mar 2022 22:25:02 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Mon, 28 Mar 2022 22:25:03 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.5.2-ubuntu18.04_amd64.deb CB_PACKAGE_NAME=couchbase-server CB_RELEASE_URL=https://packages.couchbase.com/releases/6.5.2 CB_SHA256=62f9ffad86eab90137701baab421586af49fe0e7c458bb047b6c364c6ad11684 CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Mon, 28 Mar 2022 22:26:01 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.5.2-ubuntu18.04_amd64.deb CB_PACKAGE_NAME=couchbase-server CB_RELEASE_URL=https://packages.couchbase.com/releases/6.5.2 CB_SHA256=62f9ffad86eab90137701baab421586af49fe0e7c458bb047b6c364c6ad11684 CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && export INSTALL_DONT_START_SERVER=1     && wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE     && echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c -     && ${UPDATE_COMMAND}     && dpkg --unpack ./$CB_PACKAGE     && sed -i -e '/Best heuristic/ a \ \ \ \ [ -d /run/systemd/system ] && return 1; return 0' /opt/couchbase/bin/install/systemd-ctl     && dpkg --configure couchbase-server     && apt-get install -yf     && rm -f ./$CB_PACKAGE     && ${CLEANUP_COMMAND}     && rm -rf /tmp/* /var/tmp/*
# Mon, 28 Mar 2022 22:26:04 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.5.2-ubuntu18.04_amd64.deb CB_PACKAGE_NAME=couchbase-server CB_RELEASE_URL=https://packages.couchbase.com/releases/6.5.2 CB_SHA256=62f9ffad86eab90137701baab421586af49fe0e7c458bb047b6c364c6ad11684 CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Mon, 28 Mar 2022 22:26:05 GMT
COPY file:018fa38d92aa0a4679f57c2d43b5c14547b2c603cab6ec7fd3240af5545472b5 in /etc/service/couchbase-server/run 
# Mon, 28 Mar 2022 22:26:05 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.5.2-ubuntu18.04_amd64.deb CB_PACKAGE_NAME=couchbase-server CB_RELEASE_URL=https://packages.couchbase.com/releases/6.5.2 CB_SHA256=62f9ffad86eab90137701baab421586af49fe0e7c458bb047b6c364c6ad11684 CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Mon, 28 Mar 2022 22:26:05 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Mon, 28 Mar 2022 22:26:06 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.5.2-ubuntu18.04_amd64.deb CB_PACKAGE_NAME=couchbase-server CB_RELEASE_URL=https://packages.couchbase.com/releases/6.5.2 CB_SHA256=62f9ffad86eab90137701baab421586af49fe0e7c458bb047b6c364c6ad11684 CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ln -s dummy.sh /usr/local/bin/iptables-save     && ln -s dummy.sh /usr/local/bin/lvdisplay     && ln -s dummy.sh /usr/local/bin/vgdisplay     && ln -s dummy.sh /usr/local/bin/pvdisplay
# Mon, 28 Mar 2022 22:26:14 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.5.2-ubuntu18.04_amd64.deb CB_PACKAGE_NAME=couchbase-server CB_RELEASE_URL=https://packages.couchbase.com/releases/6.5.2 CB_SHA256=62f9ffad86eab90137701baab421586af49fe0e7c458bb047b6c364c6ad11684 CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -ex     &&  if [ ! -e /opt/couchbase/bin/curl.real ]; then             ${UPDATE_COMMAND};             apt-get install -y chrpath;             chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl;             apt-get remove -y chrpath;             apt-get autoremove -y;             ${CLEANUP_COMMAND};         fi
# Mon, 28 Mar 2022 22:26:14 GMT
COPY file:6e5292e89c7124e038a0d80ea3b942bff1ed578e67a07e764b041ea95b129aa3 in / 
# Mon, 28 Mar 2022 22:26:14 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 28 Mar 2022 22:26:14 GMT
CMD ["couchbase-server"]
# Mon, 28 Mar 2022 22:26:14 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Mon, 28 Mar 2022 22:26:14 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:11323ed2c65349758e68a03a8e43825ec263dc9790daea93cf83b18ad0703109`  
		Last Modified: Thu, 17 Mar 2022 11:55:05 GMT  
		Size: 26.7 MB (26708634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e65e4923b79646d25d75b888999043d196f25ce051436f045b1e75fff6ae1ab8`  
		Last Modified: Mon, 28 Mar 2022 22:26:51 GMT  
		Size: 5.6 MB (5638780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd73140748ce0418a11a1b52dcdb4b8046207f52c6ba2e3c4bba95233feb4194`  
		Last Modified: Mon, 28 Mar 2022 22:26:49 GMT  
		Size: 2.0 KB (1965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63503eedd17f489e8120b41b25ab38d1bb71e65df1cda82723ce1ae9d1672f7f`  
		Last Modified: Mon, 28 Mar 2022 22:27:41 GMT  
		Size: 471.0 MB (470974663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3241abcc8b0e283186c99e72d7430e3cc92a75fe19a168fc2079ae31ec61ae33`  
		Last Modified: Mon, 28 Mar 2022 22:26:49 GMT  
		Size: 190.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39c30ba2267e90cfd26fce1587c258e4c1eb23b7a9619b4b453e2be36f291d79`  
		Last Modified: Mon, 28 Mar 2022 22:26:49 GMT  
		Size: 747.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b88940b3a904b3b740a05f96a62e79dadf217e023eb206cebb7c1585d0410256`  
		Last Modified: Mon, 28 Mar 2022 22:26:47 GMT  
		Size: 281.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc645b8d83b1d4db1a0d8acb37dec2be4ae2598c3fa466f17ac99598c8ffbee0`  
		Last Modified: Mon, 28 Mar 2022 22:26:47 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51f6067a56834d9cac4b52dfca44d186df9ce5e051dd3170df450b94f4055bde`  
		Last Modified: Mon, 28 Mar 2022 22:26:47 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c7185792908dc5239ca6d6d543bf0c3d9dc166c7d4a45aace5a3d4a943a5edc`  
		Last Modified: Mon, 28 Mar 2022 22:26:47 GMT  
		Size: 433.0 KB (433040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a1a64d81e3aaa5081b9a2f37a935857bcd467c9e1beb29480bb56c0c27493b1`  
		Last Modified: Mon, 28 Mar 2022 22:26:47 GMT  
		Size: 869.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
