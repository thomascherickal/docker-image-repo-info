## `couchbase:enterprise-6.5.2`

```console
$ docker pull couchbase@sha256:4e19cf0e5ec5f0c57e0bc44d9170ac011243a1fc9cc37a0ebd0362d8dd0bc4ac
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `couchbase:enterprise-6.5.2` - linux; amd64

```console
$ docker pull couchbase@sha256:b8f43ad49a00b04e0a670b530cdad2633c97add377dddca10ab235d21a694d5f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **503.8 MB (503759986 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90f3c9f7ee3c535ad7673a245614a05f9ab4ced807cc3a3a2aaf4815fd2253aa`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Fri, 29 Apr 2022 23:20:51 GMT
ADD file:f657a56a18426c3a88d620a7024e7b91424d926e7b47faa6a97c2369c4c4a228 in / 
# Fri, 29 Apr 2022 23:20:51 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 00:11:49 GMT
LABEL maintainer=docker@couchbase.com
# Sat, 30 Apr 2022 00:15:40 GMT
ARG UPDATE_COMMAND=apt-get update -y -q
# Sat, 30 Apr 2022 00:15:40 GMT
ARG CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Sat, 30 Apr 2022 00:15:49 GMT
# ARGS: CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ${UPDATE_COMMAND}     && apt-get install -y -q wget tzdata       lsof lshw sysstat net-tools numactl bzip2 runit     && ${CLEANUP_COMMAND}
# Sat, 30 Apr 2022 00:15:49 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/6.5.2
# Sat, 30 Apr 2022 00:15:49 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_6.5.2-ubuntu18.04_amd64.deb
# Sat, 30 Apr 2022 00:15:49 GMT
ARG CB_PACKAGE_NAME=couchbase-server
# Sat, 30 Apr 2022 00:15:49 GMT
ARG CB_SHA256=62f9ffad86eab90137701baab421586af49fe0e7c458bb047b6c364c6ad11684
# Sat, 30 Apr 2022 00:15:49 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Sat, 30 Apr 2022 00:15:50 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.5.2-ubuntu18.04_amd64.deb CB_PACKAGE_NAME=couchbase-server CB_RELEASE_URL=https://packages.couchbase.com/releases/6.5.2 CB_SHA256=62f9ffad86eab90137701baab421586af49fe0e7c458bb047b6c364c6ad11684 CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Sat, 30 Apr 2022 00:17:21 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.5.2-ubuntu18.04_amd64.deb CB_PACKAGE_NAME=couchbase-server CB_RELEASE_URL=https://packages.couchbase.com/releases/6.5.2 CB_SHA256=62f9ffad86eab90137701baab421586af49fe0e7c458bb047b6c364c6ad11684 CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && export INSTALL_DONT_START_SERVER=1     && wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE     && echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c -     && ${UPDATE_COMMAND}     && dpkg --unpack ./$CB_PACKAGE     && sed -i -e '/Best heuristic/ a \ \ \ \ [ -d /run/systemd/system ] && return 1; return 0' /opt/couchbase/bin/install/systemd-ctl     && dpkg --configure couchbase-server     && apt-get install -yf     && rm -f ./$CB_PACKAGE     && ${CLEANUP_COMMAND}     && rm -rf /tmp/* /var/tmp/*
# Sat, 30 Apr 2022 00:17:24 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.5.2-ubuntu18.04_amd64.deb CB_PACKAGE_NAME=couchbase-server CB_RELEASE_URL=https://packages.couchbase.com/releases/6.5.2 CB_SHA256=62f9ffad86eab90137701baab421586af49fe0e7c458bb047b6c364c6ad11684 CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Sat, 30 Apr 2022 00:17:24 GMT
COPY file:018fa38d92aa0a4679f57c2d43b5c14547b2c603cab6ec7fd3240af5545472b5 in /etc/service/couchbase-server/run 
# Sat, 30 Apr 2022 00:17:25 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.5.2-ubuntu18.04_amd64.deb CB_PACKAGE_NAME=couchbase-server CB_RELEASE_URL=https://packages.couchbase.com/releases/6.5.2 CB_SHA256=62f9ffad86eab90137701baab421586af49fe0e7c458bb047b6c364c6ad11684 CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Sat, 30 Apr 2022 00:17:25 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Sat, 30 Apr 2022 00:17:26 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.5.2-ubuntu18.04_amd64.deb CB_PACKAGE_NAME=couchbase-server CB_RELEASE_URL=https://packages.couchbase.com/releases/6.5.2 CB_SHA256=62f9ffad86eab90137701baab421586af49fe0e7c458bb047b6c364c6ad11684 CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ln -s dummy.sh /usr/local/bin/iptables-save     && ln -s dummy.sh /usr/local/bin/lvdisplay     && ln -s dummy.sh /usr/local/bin/vgdisplay     && ln -s dummy.sh /usr/local/bin/pvdisplay
# Sat, 30 Apr 2022 00:17:34 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.5.2-ubuntu18.04_amd64.deb CB_PACKAGE_NAME=couchbase-server CB_RELEASE_URL=https://packages.couchbase.com/releases/6.5.2 CB_SHA256=62f9ffad86eab90137701baab421586af49fe0e7c458bb047b6c364c6ad11684 CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -ex     &&  if [ ! -e /opt/couchbase/bin/curl.real ]; then             ${UPDATE_COMMAND};             apt-get install -y chrpath;             chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl;             apt-get remove -y chrpath;             apt-get autoremove -y;             ${CLEANUP_COMMAND};         fi
# Sat, 30 Apr 2022 00:17:34 GMT
COPY file:6e5292e89c7124e038a0d80ea3b942bff1ed578e67a07e764b041ea95b129aa3 in / 
# Sat, 30 Apr 2022 00:17:34 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 30 Apr 2022 00:17:34 GMT
CMD ["couchbase-server"]
# Sat, 30 Apr 2022 00:17:34 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Sat, 30 Apr 2022 00:17:34 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:40dd5be53814ae70b2898558673b7ea18d58bf7ab3433560b9ce3cb76d9ff0b1`  
		Last Modified: Fri, 29 Apr 2022 23:22:07 GMT  
		Size: 26.7 MB (26709108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae179a0fd9533e29049994a549a8b8d0fecafeaf5bf3cae63a0526d2310f88bc`  
		Last Modified: Sat, 30 Apr 2022 00:21:22 GMT  
		Size: 5.6 MB (5638867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d412ed7f219ba0b874ba637945dadab1ba637c8fca1c5a8e814c01c798e74793`  
		Last Modified: Sat, 30 Apr 2022 00:21:20 GMT  
		Size: 2.0 KB (1959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0769600ac1a446b2d12b7a2e921c35c2293a2787023ef472c94f7245f1748aca`  
		Last Modified: Sat, 30 Apr 2022 00:22:09 GMT  
		Size: 471.0 MB (470974353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7314e0df3b04b61df78cf2836e723ee00f9ce2f8b8d24a40e942eb88e3c3e930`  
		Last Modified: Sat, 30 Apr 2022 00:21:21 GMT  
		Size: 192.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:852f9263b4256b1809121ab87ca18d1fa517923bcdb07793ec11c58e6d294943`  
		Last Modified: Sat, 30 Apr 2022 00:21:20 GMT  
		Size: 745.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a48c59bade46100d8a807f338c009aaae34fd15ae31fe4f1d149faf82cdbad17`  
		Last Modified: Sat, 30 Apr 2022 00:21:18 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40a2ec2096780171d7e5236a7f1a8af282c6bb4f7521c266adf47ad15e9a1b33`  
		Last Modified: Sat, 30 Apr 2022 00:21:18 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5483146720dfb8433e50e99472d841b711fe4dd0809596697daa1dc16a00ebea`  
		Last Modified: Sat, 30 Apr 2022 00:21:18 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5d80eca6318c4acf977b52ac7946e3ecdc488a6aac1084a16edba7c13df33c6`  
		Last Modified: Sat, 30 Apr 2022 00:21:18 GMT  
		Size: 433.2 KB (433154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82e52f7d98be3607228b093351115339effa1a17e884a5530b389ceedd062073`  
		Last Modified: Sat, 30 Apr 2022 00:21:18 GMT  
		Size: 868.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
