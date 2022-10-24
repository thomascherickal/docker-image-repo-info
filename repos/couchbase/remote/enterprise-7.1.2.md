## `couchbase:enterprise-7.1.2`

```console
$ docker pull couchbase@sha256:fb14ff77878dcc2f53b40764d8b7413268026a3a52d04ed3a06fede454e64d8a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchbase:enterprise-7.1.2` - linux; amd64

```console
$ docker pull couchbase@sha256:43db9f11908feafb47719a0e926bfb3875efa4eb34bf233856b7e3a75778c2e7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **600.1 MB (600052223 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:94a4e33350b160e36ed40a8ffe8424cfb308dad94279fa3e50445693d7666352`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Tue, 04 Oct 2022 23:35:12 GMT
ADD file:8faed18d471598732aa3816c8f70e227f16f4de5db6c5c32812a09141048f56d in / 
# Tue, 04 Oct 2022 23:35:12 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 16:43:58 GMT
LABEL maintainer=docker@couchbase.com
# Wed, 05 Oct 2022 16:43:58 GMT
ARG UPDATE_COMMAND=apt-get update -y -q
# Wed, 05 Oct 2022 16:43:58 GMT
ARG CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Wed, 05 Oct 2022 16:44:32 GMT
# ARGS: CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ${UPDATE_COMMAND}     && apt-get install -y -q wget tzdata       lsof lshw sysstat net-tools numactl bzip2 runit     && ${CLEANUP_COMMAND}
# Mon, 24 Oct 2022 21:25:59 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.2
# Mon, 24 Oct 2022 21:25:59 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_7.1.2-linux_@@ARCH@@.deb
# Mon, 24 Oct 2022 21:25:59 GMT
ARG CB_SKIP_CHECKSUM=false
# Mon, 24 Oct 2022 21:25:59 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Mon, 24 Oct 2022 21:26:00 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.2-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.2 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Mon, 24 Oct 2022 21:27:18 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.2-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.2 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && export INSTALL_DONT_START_SERVER=1     && dpkgArch="$(dpkg --print-architecture)"     && case "${dpkgArch}" in          'arm64')            CB_SHA256=1c7c757cf8aee87b98c96ffea1c26f4c98b6e0c053d966c8e760224030d98477            ;;          'amd64')            CB_SHA256=26fd9ae8585e0ea6637d4f1b492ed637dcf06d664a49d369e1faf0782327b3ec            ;;        esac     && CB_PACKAGE=$(echo ${CB_PACKAGE} | sed -e "s/@@ARCH@@/${dpkgArch}/")     && wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE     && { ${CB_SKIP_CHECKSUM} || echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - ; }     && ${UPDATE_COMMAND}     && apt-get install -y ./$CB_PACKAGE     && rm -f ./$CB_PACKAGE     && ${CLEANUP_COMMAND}     && rm -rf /tmp/* /var/tmp/*
# Mon, 24 Oct 2022 21:27:22 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.2-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.2 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Mon, 24 Oct 2022 21:27:22 GMT
COPY file:018fa38d92aa0a4679f57c2d43b5c14547b2c603cab6ec7fd3240af5545472b5 in /etc/service/couchbase-server/run 
# Mon, 24 Oct 2022 21:27:23 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.2-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.2 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Mon, 24 Oct 2022 21:27:23 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Mon, 24 Oct 2022 21:27:24 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.2-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.2 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ln -s dummy.sh /usr/local/bin/iptables-save     && ln -s dummy.sh /usr/local/bin/lvdisplay     && ln -s dummy.sh /usr/local/bin/vgdisplay     && ln -s dummy.sh /usr/local/bin/pvdisplay
# Mon, 24 Oct 2022 21:27:24 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.2-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.2 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -ex     &&  if [ ! -e /opt/couchbase/bin/curl.real ]; then             ${UPDATE_COMMAND};             apt-get install -y chrpath;             chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl;             apt-get remove -y chrpath;             apt-get autoremove -y;             ${CLEANUP_COMMAND};         fi
# Mon, 24 Oct 2022 21:27:24 GMT
COPY file:6e5292e89c7124e038a0d80ea3b942bff1ed578e67a07e764b041ea95b129aa3 in / 
# Mon, 24 Oct 2022 21:27:24 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 24 Oct 2022 21:27:25 GMT
CMD ["couchbase-server"]
# Mon, 24 Oct 2022 21:27:25 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Mon, 24 Oct 2022 21:27:25 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:fb0b3276a519f5e7085f51c75989b287b234b3508e1524cf2cdcbc397c06ec3d`  
		Last Modified: Thu, 22 Sep 2022 20:37:52 GMT  
		Size: 28.6 MB (28574451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8f6521e7788616a3d54de1df237a477200baa4fcdcbc80f1ca20102c8dac9a2`  
		Last Modified: Wed, 05 Oct 2022 16:52:36 GMT  
		Size: 6.2 MB (6232202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ed4294155157022063832d043e5870cf3f0041b257eb6d0591a71ccb884e1ad`  
		Last Modified: Mon, 24 Oct 2022 21:29:40 GMT  
		Size: 1.8 KB (1841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b75350ea80943a6d0b728ac523d24812c072e9df29e1b3dc9245795be253cdd`  
		Last Modified: Mon, 24 Oct 2022 21:30:37 GMT  
		Size: 565.2 MB (565241194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b83fd8b65df9e1924726130bc71fd564d349c9362c18c537a875332b7868199e`  
		Last Modified: Mon, 24 Oct 2022 21:29:40 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a99cbee36c8d0b15280d3e06198929d60faa79e9b8c68d8eeb0a3876496659e`  
		Last Modified: Mon, 24 Oct 2022 21:29:38 GMT  
		Size: 744.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efa185d8f3874bc3626d0f50eb0c3a5807922e71c9df2f2c80dcb396fd02f6d4`  
		Last Modified: Mon, 24 Oct 2022 21:29:38 GMT  
		Size: 281.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1041a169a865e16423286b77033d7444428e6accaf344bbaa08ee980294ddb4d`  
		Last Modified: Mon, 24 Oct 2022 21:29:38 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4d34e150d092d28dd1b92731f930fe34902f1007e6d3b5281bffdd8f401de39`  
		Last Modified: Mon, 24 Oct 2022 21:29:38 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53731c36206040583c501d6cafb21deff20d807630c1eec787c7506843899a6f`  
		Last Modified: Mon, 24 Oct 2022 21:29:38 GMT  
		Size: 868.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchbase:enterprise-7.1.2` - linux; arm64 variant v8

```console
$ docker pull couchbase@sha256:fbdbeb909ed702aa4b1ae01e65338a169fa05e2c4c9ea2f8ee68707981de72ff
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **574.1 MB (574082024 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5586e67f79257d6baa7d552a99933db1b205b6e626eb90e54a9b2458464284e`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Wed, 05 Oct 2022 00:02:10 GMT
ADD file:30b589901d2a6b82d0b7271487bdaf37514649a798cc13a17f74394321bdd051 in / 
# Wed, 05 Oct 2022 00:02:11 GMT
CMD ["bash"]
# Mon, 24 Oct 2022 21:55:44 GMT
LABEL maintainer=docker@couchbase.com
# Mon, 24 Oct 2022 21:55:44 GMT
ARG UPDATE_COMMAND=apt-get update -y -q
# Mon, 24 Oct 2022 21:55:44 GMT
ARG CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Mon, 24 Oct 2022 21:56:22 GMT
# ARGS: CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ${UPDATE_COMMAND}     && apt-get install -y -q wget tzdata       lsof lshw sysstat net-tools numactl bzip2 runit     && ${CLEANUP_COMMAND}
# Mon, 24 Oct 2022 21:56:22 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.2
# Mon, 24 Oct 2022 21:56:23 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_7.1.2-linux_@@ARCH@@.deb
# Mon, 24 Oct 2022 21:56:23 GMT
ARG CB_SKIP_CHECKSUM=false
# Mon, 24 Oct 2022 21:56:23 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Mon, 24 Oct 2022 21:56:23 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.2-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.2 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Mon, 24 Oct 2022 21:57:20 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.2-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.2 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && export INSTALL_DONT_START_SERVER=1     && dpkgArch="$(dpkg --print-architecture)"     && case "${dpkgArch}" in          'arm64')            CB_SHA256=1c7c757cf8aee87b98c96ffea1c26f4c98b6e0c053d966c8e760224030d98477            ;;          'amd64')            CB_SHA256=26fd9ae8585e0ea6637d4f1b492ed637dcf06d664a49d369e1faf0782327b3ec            ;;        esac     && CB_PACKAGE=$(echo ${CB_PACKAGE} | sed -e "s/@@ARCH@@/${dpkgArch}/")     && wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE     && { ${CB_SKIP_CHECKSUM} || echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - ; }     && ${UPDATE_COMMAND}     && apt-get install -y ./$CB_PACKAGE     && rm -f ./$CB_PACKAGE     && ${CLEANUP_COMMAND}     && rm -rf /tmp/* /var/tmp/*
# Mon, 24 Oct 2022 21:57:29 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.2-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.2 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Mon, 24 Oct 2022 21:57:29 GMT
COPY file:018fa38d92aa0a4679f57c2d43b5c14547b2c603cab6ec7fd3240af5545472b5 in /etc/service/couchbase-server/run 
# Mon, 24 Oct 2022 21:57:30 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.2-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.2 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Mon, 24 Oct 2022 21:57:30 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Mon, 24 Oct 2022 21:57:30 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.2-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.2 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ln -s dummy.sh /usr/local/bin/iptables-save     && ln -s dummy.sh /usr/local/bin/lvdisplay     && ln -s dummy.sh /usr/local/bin/vgdisplay     && ln -s dummy.sh /usr/local/bin/pvdisplay
# Mon, 24 Oct 2022 21:57:31 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.2-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.2 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -ex     &&  if [ ! -e /opt/couchbase/bin/curl.real ]; then             ${UPDATE_COMMAND};             apt-get install -y chrpath;             chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl;             apt-get remove -y chrpath;             apt-get autoremove -y;             ${CLEANUP_COMMAND};         fi
# Mon, 24 Oct 2022 21:57:31 GMT
COPY file:6e5292e89c7124e038a0d80ea3b942bff1ed578e67a07e764b041ea95b129aa3 in / 
# Mon, 24 Oct 2022 21:57:31 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 24 Oct 2022 21:57:31 GMT
CMD ["couchbase-server"]
# Mon, 24 Oct 2022 21:57:31 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Mon, 24 Oct 2022 21:57:31 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:514fa78e57ce0d9437bc984cc36ab780c24b69da2b922bfff16737072e3e7de2`  
		Last Modified: Wed, 05 Oct 2022 00:03:51 GMT  
		Size: 27.2 MB (27191622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fd4213541647e0bd157630575f1ce12ab34bf86ddb1f38275d007ddee3c42e3`  
		Last Modified: Mon, 24 Oct 2022 21:58:32 GMT  
		Size: 6.1 MB (6058434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57bf2e4f8352f457f4e17cefdb0a853638baf4f56e1918c045ddec2b1665ab2f`  
		Last Modified: Mon, 24 Oct 2022 21:58:31 GMT  
		Size: 1.8 KB (1840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f2b3271e89db387353725884822dba008cc472d29ce0fec112cfd2078a7100c`  
		Last Modified: Mon, 24 Oct 2022 21:59:11 GMT  
		Size: 540.8 MB (540827599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e08a5945a886b16aedbd5dd6ae9b23996713053bf098818f205afea19881dbec`  
		Last Modified: Mon, 24 Oct 2022 21:58:31 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:950b15f3a20c220dbcd3618f3772fd0bbdf7de89c7c3fb50627640a67bd1dff5`  
		Last Modified: Mon, 24 Oct 2022 21:58:29 GMT  
		Size: 740.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:727cf7782ced5c81cc91ffb1f9fb51766c5c2020061c14c87b2d3d8a12bf5c8d`  
		Last Modified: Mon, 24 Oct 2022 21:58:29 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35449a251c18f484ccc31aedcb342ed8debd2e68abad0df55fed778de335c5fa`  
		Last Modified: Mon, 24 Oct 2022 21:58:29 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36decd7e85da0aaf07f59bb9bc5f5dbe4d8924e028ba94e924b9199496c1b2cd`  
		Last Modified: Mon, 24 Oct 2022 21:58:29 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10c55cf5bd60c9cb4080ffb3224f22f72f7acf4bffefb903590a1f7b3e41977c`  
		Last Modified: Mon, 24 Oct 2022 21:58:29 GMT  
		Size: 868.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
