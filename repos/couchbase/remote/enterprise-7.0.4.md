## `couchbase:enterprise-7.0.4`

```console
$ docker pull couchbase@sha256:d460b07489d7c8448fd156d0ffca64c9ea813c1b7e20ff2f89fcd35fc56ef325
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `couchbase:enterprise-7.0.4` - linux; amd64

```console
$ docker pull couchbase@sha256:0f94afe1b669c8e530b716fbeddea938a5256ae9e91038f00bc34786ebc7d58b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **641.1 MB (641131247 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c01f005a80586feccd04a29188f9c8c7477246596751f528b7578ee17217b0cd`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Fri, 09 Dec 2022 01:20:21 GMT
ADD file:9d282119af0c42bc823c95b4192a3350cf2cad670622017356dd2e637762e425 in / 
# Fri, 09 Dec 2022 01:20:21 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 06:11:50 GMT
LABEL maintainer=docker@couchbase.com
# Fri, 09 Dec 2022 06:11:50 GMT
ARG UPDATE_COMMAND=apt-get update -y -q
# Fri, 09 Dec 2022 06:11:50 GMT
ARG CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Fri, 09 Dec 2022 06:12:09 GMT
# ARGS: CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ${UPDATE_COMMAND}     && apt-get install -y -q wget tzdata       lsof lshw sysstat net-tools numactl bzip2 runit     && ${CLEANUP_COMMAND}
# Fri, 09 Dec 2022 06:14:31 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.4
# Fri, 09 Dec 2022 06:14:32 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_7.0.4-ubuntu20.04_amd64.deb
# Fri, 09 Dec 2022 06:14:32 GMT
ARG CB_SHA256=dfa3c2eec3cbf31ee200eb1423f4b19719edd0b73fdf1132956302462b74a9b2
# Fri, 09 Dec 2022 06:14:32 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Fri, 09 Dec 2022 06:14:32 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.4-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.4 CB_SHA256=dfa3c2eec3cbf31ee200eb1423f4b19719edd0b73fdf1132956302462b74a9b2 CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Fri, 09 Dec 2022 06:15:41 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.4-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.4 CB_SHA256=dfa3c2eec3cbf31ee200eb1423f4b19719edd0b73fdf1132956302462b74a9b2 CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && export INSTALL_DONT_START_SERVER=1     && wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE     && echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c -     && ${UPDATE_COMMAND}     && apt-get install -y ./$CB_PACKAGE     && rm -f ./$CB_PACKAGE     && ${CLEANUP_COMMAND}     && rm -rf /tmp/* /var/tmp/*
# Fri, 09 Dec 2022 06:15:46 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.4-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.4 CB_SHA256=dfa3c2eec3cbf31ee200eb1423f4b19719edd0b73fdf1132956302462b74a9b2 CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Fri, 09 Dec 2022 06:15:46 GMT
COPY file:018fa38d92aa0a4679f57c2d43b5c14547b2c603cab6ec7fd3240af5545472b5 in /etc/service/couchbase-server/run 
# Fri, 09 Dec 2022 06:15:47 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.4-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.4 CB_SHA256=dfa3c2eec3cbf31ee200eb1423f4b19719edd0b73fdf1132956302462b74a9b2 CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Fri, 09 Dec 2022 06:15:47 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Fri, 09 Dec 2022 06:15:47 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.4-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.4 CB_SHA256=dfa3c2eec3cbf31ee200eb1423f4b19719edd0b73fdf1132956302462b74a9b2 CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ln -s dummy.sh /usr/local/bin/iptables-save     && ln -s dummy.sh /usr/local/bin/lvdisplay     && ln -s dummy.sh /usr/local/bin/vgdisplay     && ln -s dummy.sh /usr/local/bin/pvdisplay
# Fri, 09 Dec 2022 06:15:55 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.4-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.4 CB_SHA256=dfa3c2eec3cbf31ee200eb1423f4b19719edd0b73fdf1132956302462b74a9b2 CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -ex     &&  if [ ! -e /opt/couchbase/bin/curl.real ]; then             ${UPDATE_COMMAND};             apt-get install -y chrpath;             chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl;             apt-get remove -y chrpath;             apt-get autoremove -y;             ${CLEANUP_COMMAND};         fi
# Fri, 09 Dec 2022 06:15:55 GMT
COPY file:6e5292e89c7124e038a0d80ea3b942bff1ed578e67a07e764b041ea95b129aa3 in / 
# Fri, 09 Dec 2022 06:15:55 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 09 Dec 2022 06:15:55 GMT
CMD ["couchbase-server"]
# Fri, 09 Dec 2022 06:15:55 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Fri, 09 Dec 2022 06:15:55 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:846c0b181fff0c667d9444f8378e8fcfa13116da8d308bf21673f7e4bea8d580`  
		Last Modified: Thu, 08 Dec 2022 13:18:11 GMT  
		Size: 28.6 MB (28576882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a266fa58ec7bd5adffaae9152c63d27666a9a1ce40e9ecf1e9c12cc2eef31848`  
		Last Modified: Fri, 09 Dec 2022 06:20:54 GMT  
		Size: 6.2 MB (6216914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5405510b757ec9c16b8ec3bf12d7db6996c7269dcb4499a04fd82d6b33f1905`  
		Last Modified: Fri, 09 Dec 2022 06:22:56 GMT  
		Size: 1.8 KB (1841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1cdcc6935ed4739938a7740229e17d9ced5df35dc85ea5219e462a96eef7bdb`  
		Last Modified: Fri, 09 Dec 2022 06:24:00 GMT  
		Size: 605.9 MB (605889093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dd33c42bec399cd169e10c3eaa5948ee184c3ec78b8a36ed844d0525dbd44c2`  
		Last Modified: Fri, 09 Dec 2022 06:22:56 GMT  
		Size: 190.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f80feff94084e0c14b649ba57a5de2126452eba6c8468973a0efd14d1e558bfe`  
		Last Modified: Fri, 09 Dec 2022 06:22:56 GMT  
		Size: 745.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c866d40f1bbb0629834fcd2c0424dd504a76433e9dc4e80c0e0483af56b30f2`  
		Last Modified: Fri, 09 Dec 2022 06:22:54 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ff8115b34de01492b2a8e5157068fc4493a87f4ee980ae390a93073d1800d8c`  
		Last Modified: Fri, 09 Dec 2022 06:22:54 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:522419f361ca7e61affb1055417eff0e83d261557bfcf51d2b71ee96081fbce9`  
		Last Modified: Fri, 09 Dec 2022 06:22:54 GMT  
		Size: 217.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45df098827280287012d03e23aaec1e38aff8419436cbaf79c4dcc26e3d45d3b`  
		Last Modified: Fri, 09 Dec 2022 06:22:54 GMT  
		Size: 444.0 KB (443984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ec441f96ea4b53caec4b23a01cf786323ea8bed9255b0504e3ae67ce5247f7a`  
		Last Modified: Fri, 09 Dec 2022 06:22:54 GMT  
		Size: 867.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
