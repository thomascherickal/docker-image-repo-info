## `couchbase:latest`

```console
$ docker pull couchbase@sha256:066a96ee394b6b9d80bd165951ba93a0132088d238576ce2743faeb3b51d198d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchbase:latest` - linux; amd64

```console
$ docker pull couchbase@sha256:15680d9acfc80b79deb297c4920e73ed274b433e4fa1448baeae03bab0cc9b53
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **596.7 MB (596656200 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3449f52cbf2ba6c3d4994054d104dd740bdb4a953d9a3f9b6cf45b22d7062b17`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Mon, 06 Jun 2022 22:21:11 GMT
ADD file:00dae10e79b05c4e1a3db053a1f85a4f38a39fe85cbbd88d74201a01a7dd59b5 in / 
# Mon, 06 Jun 2022 22:21:12 GMT
CMD ["bash"]
# Mon, 06 Jun 2022 23:57:21 GMT
LABEL maintainer=docker@couchbase.com
# Mon, 06 Jun 2022 23:57:21 GMT
ARG UPDATE_COMMAND=apt-get update -y -q
# Mon, 06 Jun 2022 23:57:21 GMT
ARG CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Mon, 06 Jun 2022 23:57:42 GMT
# ARGS: CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ${UPDATE_COMMAND}     && apt-get install -y -q wget tzdata       lsof lshw sysstat net-tools numactl bzip2 runit     && ${CLEANUP_COMMAND}
# Thu, 07 Jul 2022 19:19:30 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.1
# Thu, 07 Jul 2022 19:19:30 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_7.1.1-linux_@@ARCH@@.deb
# Thu, 07 Jul 2022 19:19:30 GMT
ARG CB_SKIP_CHECKSUM=false
# Thu, 07 Jul 2022 19:19:30 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Thu, 07 Jul 2022 19:19:31 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.1-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.1 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Thu, 07 Jul 2022 19:21:12 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.1-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.1 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && export INSTALL_DONT_START_SERVER=1     && dpkgArch="$(dpkg --print-architecture)"     && case "${dpkgArch}" in          'arm64')            CB_SHA256=fe1d40c6406f2b047ebf3d4cbe4a539e532f7ce57dc48d1e7aef58dbe43c7d0c            ;;          'amd64')            CB_SHA256=f311b16425fe38dc59d76eb0eb7d31e7ee718b7e7618a56eb1e9f95717baca6f            ;;        esac     && CB_PACKAGE=$(echo ${CB_PACKAGE} | sed -e "s/@@ARCH@@/${dpkgArch}/")     && wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE     && { ${CB_SKIP_CHECKSUM} || echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - ; }     && ${UPDATE_COMMAND}     && apt-get install -y ./$CB_PACKAGE     && rm -f ./$CB_PACKAGE     && ${CLEANUP_COMMAND}     && rm -rf /tmp/* /var/tmp/*
# Thu, 07 Jul 2022 19:21:17 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.1-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.1 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Thu, 07 Jul 2022 19:21:17 GMT
COPY file:018fa38d92aa0a4679f57c2d43b5c14547b2c603cab6ec7fd3240af5545472b5 in /etc/service/couchbase-server/run 
# Thu, 07 Jul 2022 19:21:18 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.1-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.1 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Thu, 07 Jul 2022 19:21:18 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Thu, 07 Jul 2022 19:21:18 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.1-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.1 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ln -s dummy.sh /usr/local/bin/iptables-save     && ln -s dummy.sh /usr/local/bin/lvdisplay     && ln -s dummy.sh /usr/local/bin/vgdisplay     && ln -s dummy.sh /usr/local/bin/pvdisplay
# Thu, 07 Jul 2022 19:21:19 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.1-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.1 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -ex     &&  if [ ! -e /opt/couchbase/bin/curl.real ]; then             ${UPDATE_COMMAND};             apt-get install -y chrpath;             chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl;             apt-get remove -y chrpath;             apt-get autoremove -y;             ${CLEANUP_COMMAND};         fi
# Thu, 07 Jul 2022 19:21:19 GMT
COPY file:6e5292e89c7124e038a0d80ea3b942bff1ed578e67a07e764b041ea95b129aa3 in / 
# Thu, 07 Jul 2022 19:21:19 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 07 Jul 2022 19:21:19 GMT
CMD ["couchbase-server"]
# Thu, 07 Jul 2022 19:21:19 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Thu, 07 Jul 2022 19:21:20 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:d7bfe07ed8476565a440c2113cc64d7c0409dba8ef761fb3ec019d7e6b5952df`  
		Last Modified: Wed, 01 Jun 2022 21:51:10 GMT  
		Size: 28.6 MB (28572632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b15b7718218cb8c8adc351f6e6d4b00e354a525046c18ec4d6f5bab108a1a66`  
		Last Modified: Tue, 07 Jun 2022 00:07:47 GMT  
		Size: 6.3 MB (6251734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b6372c4fb481828324e1ad41b72bee3b201ccc91662e6e1b7c85b6abd2843e2`  
		Last Modified: Thu, 07 Jul 2022 19:22:46 GMT  
		Size: 1.8 KB (1836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b322fe23793cbfac6125d820d14611c59f6704c28c3f770f85bd0f1253b99fe4`  
		Last Modified: Thu, 07 Jul 2022 19:23:44 GMT  
		Size: 561.8 MB (561827459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd6c561ca385a87c4b4e45fd3028e9ff03bb546b40b12024a10c291560aec5ee`  
		Last Modified: Thu, 07 Jul 2022 19:22:46 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:794e8ea252d6c4675352f5b65986b4b22c124054b2b8ca7573218935c42d7f72`  
		Last Modified: Thu, 07 Jul 2022 19:22:44 GMT  
		Size: 746.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20b99d6f148d1ef96717bd4959fe26ad7ea987ae035a6857b68419b6e06fa23d`  
		Last Modified: Thu, 07 Jul 2022 19:22:44 GMT  
		Size: 281.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf7a943c711c8522f31d142c45fe74c69aa10212c32256e460fb9064cdcf9d6d`  
		Last Modified: Thu, 07 Jul 2022 19:22:44 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d010ce5703d8d5a246c6c18d81c3335643fdd8177ecbd84db346d867088763bc`  
		Last Modified: Thu, 07 Jul 2022 19:22:44 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd8d0120f5b641565fed2ac0f24002dd89734b23c2e3b1774f062e782214290a`  
		Last Modified: Thu, 07 Jul 2022 19:22:44 GMT  
		Size: 868.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchbase:latest` - linux; arm64 variant v8

```console
$ docker pull couchbase@sha256:2e212e17bc3e61550136d8e3afb432aa16a335606b0b82b8c29eccd260a67d8b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **571.8 MB (571842104 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d71d5d362ccc5676e859558ff2de8412291041f6d0f968b0ed996489d8fb5d7c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Tue, 07 Jun 2022 01:25:15 GMT
ADD file:8bb0809a8ac8e978274cf731cff7529372088d22c5b0233a28f01ef414aefbca in / 
# Tue, 07 Jun 2022 01:25:16 GMT
CMD ["bash"]
# Thu, 07 Jul 2022 19:41:46 GMT
LABEL maintainer=docker@couchbase.com
# Thu, 07 Jul 2022 19:41:47 GMT
ARG UPDATE_COMMAND=apt-get update -y -q
# Thu, 07 Jul 2022 19:41:48 GMT
ARG CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Thu, 07 Jul 2022 19:42:01 GMT
# ARGS: CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ${UPDATE_COMMAND}     && apt-get install -y -q wget tzdata       lsof lshw sysstat net-tools numactl bzip2 runit     && ${CLEANUP_COMMAND}
# Thu, 07 Jul 2022 19:42:01 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.1
# Thu, 07 Jul 2022 19:42:02 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_7.1.1-linux_@@ARCH@@.deb
# Thu, 07 Jul 2022 19:42:03 GMT
ARG CB_SKIP_CHECKSUM=false
# Thu, 07 Jul 2022 19:42:04 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Thu, 07 Jul 2022 19:42:05 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.1-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.1 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Thu, 07 Jul 2022 19:42:55 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.1-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.1 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && export INSTALL_DONT_START_SERVER=1     && dpkgArch="$(dpkg --print-architecture)"     && case "${dpkgArch}" in          'arm64')            CB_SHA256=fe1d40c6406f2b047ebf3d4cbe4a539e532f7ce57dc48d1e7aef58dbe43c7d0c            ;;          'amd64')            CB_SHA256=f311b16425fe38dc59d76eb0eb7d31e7ee718b7e7618a56eb1e9f95717baca6f            ;;        esac     && CB_PACKAGE=$(echo ${CB_PACKAGE} | sed -e "s/@@ARCH@@/${dpkgArch}/")     && wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE     && { ${CB_SKIP_CHECKSUM} || echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - ; }     && ${UPDATE_COMMAND}     && apt-get install -y ./$CB_PACKAGE     && rm -f ./$CB_PACKAGE     && ${CLEANUP_COMMAND}     && rm -rf /tmp/* /var/tmp/*
# Thu, 07 Jul 2022 19:42:57 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.1-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.1 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Thu, 07 Jul 2022 19:42:58 GMT
COPY file:018fa38d92aa0a4679f57c2d43b5c14547b2c603cab6ec7fd3240af5545472b5 in /etc/service/couchbase-server/run 
# Thu, 07 Jul 2022 19:42:59 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.1-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.1 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Thu, 07 Jul 2022 19:43:00 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Thu, 07 Jul 2022 19:43:01 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.1-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.1 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ln -s dummy.sh /usr/local/bin/iptables-save     && ln -s dummy.sh /usr/local/bin/lvdisplay     && ln -s dummy.sh /usr/local/bin/vgdisplay     && ln -s dummy.sh /usr/local/bin/pvdisplay
# Thu, 07 Jul 2022 19:43:02 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.1-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.1 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -ex     &&  if [ ! -e /opt/couchbase/bin/curl.real ]; then             ${UPDATE_COMMAND};             apt-get install -y chrpath;             chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl;             apt-get remove -y chrpath;             apt-get autoremove -y;             ${CLEANUP_COMMAND};         fi
# Thu, 07 Jul 2022 19:43:03 GMT
COPY file:6e5292e89c7124e038a0d80ea3b942bff1ed578e67a07e764b041ea95b129aa3 in / 
# Thu, 07 Jul 2022 19:43:03 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 07 Jul 2022 19:43:04 GMT
CMD ["couchbase-server"]
# Thu, 07 Jul 2022 19:43:05 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Thu, 07 Jul 2022 19:43:06 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:11e23ac719b33170b39b7e30b8027dc09c9cbad6b503b2b6b3ebbd9d33f4adad`  
		Last Modified: Thu, 02 Jun 2022 08:33:07 GMT  
		Size: 27.2 MB (27191210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:005b29c60273af78ee16787d9ab3ba27a5ee1a28c2237ee0d59d796af37e56df`  
		Last Modified: Thu, 07 Jul 2022 19:44:24 GMT  
		Size: 6.1 MB (6074235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e4b6abe305301ce790822edfac978bd9700f95c258ed4728b73dee494538781`  
		Last Modified: Thu, 07 Jul 2022 19:44:23 GMT  
		Size: 1.8 KB (1817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97655a7b8561f61113bb176047d12897bfebcde6327b8c7b30d143bd1875be2b`  
		Last Modified: Thu, 07 Jul 2022 19:45:20 GMT  
		Size: 538.6 MB (538572362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f783706b2bc77d164a6710768e3c4fe24f743d4f67a24fef36204a9f7f349e34`  
		Last Modified: Thu, 07 Jul 2022 19:44:23 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07e0cdbe1ad45ba347cc11e522c40854e7ca6bb82c639c7605f3220a16932d64`  
		Last Modified: Thu, 07 Jul 2022 19:44:21 GMT  
		Size: 716.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56b434bdd5edb44b8fb8e2fc382d4367c98311db5a416cfd64f147389affb149`  
		Last Modified: Thu, 07 Jul 2022 19:44:21 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b797480a8ad90dc09ead3242983eebf32c083c610ac8f1c42e0f57cc10b42936`  
		Last Modified: Thu, 07 Jul 2022 19:44:21 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cc5dfec0a40b9eb4c25bff87c69336a4fc9d0664e1ac3b602814040bae3f1ce`  
		Last Modified: Thu, 07 Jul 2022 19:44:21 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aa07bb15190e2fb6f56bfe45e409367a7d3eb6006f63e602801154f0ab59bbb`  
		Last Modified: Thu, 07 Jul 2022 19:44:21 GMT  
		Size: 868.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
