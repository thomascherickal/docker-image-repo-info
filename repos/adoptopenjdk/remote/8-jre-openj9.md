## `adoptopenjdk:8-jre-openj9`

```console
$ docker pull adoptopenjdk@sha256:086bbf12a39ea343ea6657f0f59779ddb6c1547cf178b26ab45cc3ef977cb021
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.14393.3750; amd64
	-	windows version 10.0.17763.1282; amd64

### `adoptopenjdk:8-jre-openj9` - linux; amd64

```console
$ docker pull adoptopenjdk@sha256:59e6728044e5478a60c002b8ff90a6312f1bbdf98a4a5f4e559777032aed7a84
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **88.5 MB (88539188 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:753e6517ea05e78acc0bc55fb809b91c7eec92a1b3c875fa243307f17daa1c0b`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 17 Jun 2020 01:20:29 GMT
ADD file:1e8d02626176dc8141df3c0a1365774ce73d79934654fe24a4b1e7f173108232 in / 
# Wed, 17 Jun 2020 01:20:30 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 17 Jun 2020 01:20:31 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 17 Jun 2020 01:20:31 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 17 Jun 2020 01:20:32 GMT
CMD ["/bin/bash"]
# Wed, 17 Jun 2020 01:46:10 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 17 Jun 2020 01:46:25 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 17 Jun 2020 01:48:08 GMT
ENV JAVA_VERSION=jdk8u252-b09_openj9-0.20.0
# Wed, 17 Jun 2020 01:48:27 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='00095854b2219c71a142135ef2b63ae48869f4366c82524353991a36204cf7e9';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u252-b09_openj9-0.20.0/OpenJDK8U-jre_ppc64le_linux_openj9_8u252b09_openj9-0.20.0.tar.gz';          ;;        s390x)          ESUM='7cb7d392fb7240c30b0993a6ec332060b406641589b4c0207b7f9cbbaad81fc8';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u252-b09_openj9-0.20.0/OpenJDK8U-jre_s390x_linux_openj9_8u252b09_openj9-0.20.0.tar.gz';          ;;        amd64|x86_64)          ESUM='5c0ab4691ff5f8e69bb14462f2afb8d73d751b01048eacf4b426ed6d6646dc63';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u252-b09_openj9-0.20.0/OpenJDK8U-jre_x64_linux_openj9_8u252b09_openj9-0.20.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 17 Jun 2020 01:48:28 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Jun 2020 01:48:28 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+UseContainerSupport -XX:+IdleTuningCompactOnIdle -XX:+IdleTuningGcOnIdle
```

-	Layers:
	-	`sha256:d7c3167c320d7a820935f54cf4290890ea19567da496ecf774e8773b35d5f065`  
		Last Modified: Wed, 27 May 2020 12:21:15 GMT  
		Size: 26.7 MB (26688718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:131f805ec7fd68d45a887e2ef82de61de0247b4eb934ab03b7c933650e854baa`  
		Last Modified: Wed, 17 Jun 2020 01:21:41 GMT  
		Size: 35.4 KB (35369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:322ed380e680a77f30528ba013e3a802a7b44948a0609c7d1d732dd46a9a310d`  
		Last Modified: Wed, 17 Jun 2020 01:21:41 GMT  
		Size: 844.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ac240b130982ad1c3ba3188abbf18ba4e54bdd9e504ce2d5c2eff6d3e86b8dd`  
		Last Modified: Wed, 17 Jun 2020 01:21:41 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:205a7ec514d2cd428757163aacefd82b2947b6a557973f9bf6587fe2bc31e3b8`  
		Last Modified: Wed, 17 Jun 2020 01:50:17 GMT  
		Size: 13.3 MB (13311450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:783fe3f38ac2ace41cdfb5c8bcb0b62ad1d09048cd808a7c9ea1db52043590cd`  
		Last Modified: Wed, 17 Jun 2020 01:52:59 GMT  
		Size: 48.5 MB (48502644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adoptopenjdk:8-jre-openj9` - linux; ppc64le

```console
$ docker pull adoptopenjdk@sha256:670a15699ee5fee686404571199ee471a1511bab0614113326b9b20cf194932a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.4 MB (93385032 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ca3af757f6418d5f288cae158fb4c99de6c97d024e13efb872d8c36ebea8660`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 17 Jun 2020 01:23:28 GMT
ADD file:3d8a4167931b708419d8f212295ee2e69c2e17523d93de0f36af7c8b7adaf6b0 in / 
# Wed, 17 Jun 2020 01:23:41 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 17 Jun 2020 01:23:47 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 17 Jun 2020 01:23:53 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 17 Jun 2020 01:23:59 GMT
CMD ["/bin/bash"]
# Wed, 17 Jun 2020 03:25:24 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 17 Jun 2020 03:26:55 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 17 Jun 2020 03:32:31 GMT
ENV JAVA_VERSION=jdk8u252-b09_openj9-0.20.0
# Wed, 17 Jun 2020 03:33:26 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='00095854b2219c71a142135ef2b63ae48869f4366c82524353991a36204cf7e9';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u252-b09_openj9-0.20.0/OpenJDK8U-jre_ppc64le_linux_openj9_8u252b09_openj9-0.20.0.tar.gz';          ;;        s390x)          ESUM='7cb7d392fb7240c30b0993a6ec332060b406641589b4c0207b7f9cbbaad81fc8';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u252-b09_openj9-0.20.0/OpenJDK8U-jre_s390x_linux_openj9_8u252b09_openj9-0.20.0.tar.gz';          ;;        amd64|x86_64)          ESUM='5c0ab4691ff5f8e69bb14462f2afb8d73d751b01048eacf4b426ed6d6646dc63';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u252-b09_openj9-0.20.0/OpenJDK8U-jre_x64_linux_openj9_8u252b09_openj9-0.20.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 17 Jun 2020 03:33:31 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Jun 2020 03:33:33 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+UseContainerSupport -XX:+IdleTuningCompactOnIdle -XX:+IdleTuningGcOnIdle
```

-	Layers:
	-	`sha256:c82758296165adcddbc1b265a621d9938f9c807decd8469ae7f939d875188bf5`  
		Last Modified: Sat, 30 May 2020 05:26:15 GMT  
		Size: 30.4 MB (30400411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:740d34e8b0154512b13d50a28cb641b322092ef53e5681dd77102035104fbffe`  
		Last Modified: Wed, 17 Jun 2020 01:28:15 GMT  
		Size: 35.2 KB (35202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e49637d96cd01435b847808eee898f2f13837bf3034497154962bb88ef0416b`  
		Last Modified: Wed, 17 Jun 2020 01:28:15 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:042abc2d98a7172c5b211cb1f6be22813334814c096e94c8fbf0a7972587d765`  
		Last Modified: Wed, 17 Jun 2020 01:28:15 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68a910ee11e6ad058caab92c085018fc0da3bfc7f3d1bb0c650f7aa3eb0c7d7c`  
		Last Modified: Wed, 17 Jun 2020 03:39:07 GMT  
		Size: 14.0 MB (13955963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c7c12832a6a83f2f842f13e6f498631e889f6af057d69f403d2d603ffb5b355`  
		Last Modified: Wed, 17 Jun 2020 03:43:18 GMT  
		Size: 49.0 MB (48992420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adoptopenjdk:8-jre-openj9` - linux; s390x

```console
$ docker pull adoptopenjdk@sha256:ad0faa023aa245428e6cb1e4b69fcb30096054d1d5e90453f42c099c342df01a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **86.7 MB (86724847 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d4b0f1d35739da60b636fcfa6aa54c9c11d916e575a7188df219b16cdb6bf0e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 17 Jun 2020 01:41:48 GMT
ADD file:8708e93980b416070ba0bb024a7858748129059a85d2c771a4489c31710a9df1 in / 
# Wed, 17 Jun 2020 01:41:51 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 17 Jun 2020 01:41:52 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 17 Jun 2020 01:41:52 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 17 Jun 2020 01:41:53 GMT
CMD ["/bin/bash"]
# Wed, 17 Jun 2020 02:57:43 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 17 Jun 2020 02:58:00 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 17 Jun 2020 03:00:09 GMT
ENV JAVA_VERSION=jdk8u252-b09_openj9-0.20.0
# Wed, 17 Jun 2020 03:00:30 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='00095854b2219c71a142135ef2b63ae48869f4366c82524353991a36204cf7e9';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u252-b09_openj9-0.20.0/OpenJDK8U-jre_ppc64le_linux_openj9_8u252b09_openj9-0.20.0.tar.gz';          ;;        s390x)          ESUM='7cb7d392fb7240c30b0993a6ec332060b406641589b4c0207b7f9cbbaad81fc8';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u252-b09_openj9-0.20.0/OpenJDK8U-jre_s390x_linux_openj9_8u252b09_openj9-0.20.0.tar.gz';          ;;        amd64|x86_64)          ESUM='5c0ab4691ff5f8e69bb14462f2afb8d73d751b01048eacf4b426ed6d6646dc63';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u252-b09_openj9-0.20.0/OpenJDK8U-jre_x64_linux_openj9_8u252b09_openj9-0.20.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 17 Jun 2020 03:00:32 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Jun 2020 03:00:32 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+UseContainerSupport -XX:+IdleTuningCompactOnIdle -XX:+IdleTuningGcOnIdle
```

-	Layers:
	-	`sha256:f3c26641772baa3348c0cce190edb38690a41f1824570c5c65cc363b42e5a5b5`  
		Last Modified: Sat, 30 May 2020 09:30:29 GMT  
		Size: 25.4 MB (25365846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bf76fcee55454304ffbf9e321dda388a7e8de8a3916f854e1e588bc6c19b088`  
		Last Modified: Wed, 17 Jun 2020 01:42:56 GMT  
		Size: 36.2 KB (36165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5173e4f9f1868daa26021e1e701a000b0aadb2b611a487d089e7de4b728a7424`  
		Last Modified: Wed, 17 Jun 2020 01:42:56 GMT  
		Size: 846.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13da9fe451bd0f377d042d4bebef4ffd19163113e3e66dcd718fe187149a0dbd`  
		Last Modified: Wed, 17 Jun 2020 01:42:57 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ed532570dcab9ebdbb790d8ffbc4d7efd4d3032c37c5279da2aff135f7a2514`  
		Last Modified: Wed, 17 Jun 2020 03:02:51 GMT  
		Size: 13.0 MB (13032315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3f870ab5567cf00a1feca789c25868ac4f1f0ea8e055a0f82b12c7e7a4eab30`  
		Last Modified: Wed, 17 Jun 2020 03:05:19 GMT  
		Size: 48.3 MB (48289486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adoptopenjdk:8-jre-openj9` - windows version 10.0.14393.3750; amd64

```console
$ docker pull adoptopenjdk@sha256:180a391ce46dbae5f0d312fc571e3cea4d69c33bb9fb46c716fabbc3d28c43b0
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5827475039 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bce46ef93609778aa5267da716c95d9f80174e77516be76a4ac00806438da5ae`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 01 Jun 2020 18:53:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 09 Jun 2020 22:36:45 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Jun 2020 16:54:58 GMT
ENV JAVA_VERSION=jdk8u252-b09.1_openj9-0.20.0
# Wed, 10 Jun 2020 17:02:15 GMT
RUN Write-Host ('Downloading https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u252-b09.1_openj9-0.20.0/OpenJDK8U-jre_x64_windows_openj9_8u252b09_openj9-0.20.0.msi ...');         [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;         wget https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u252-b09.1_openj9-0.20.0/OpenJDK8U-jre_x64_windows_openj9_8u252b09_openj9-0.20.0.msi -O 'openjdk.msi';         Write-Host ('Verifying sha256 (3cd2f93eb25832e7ececa054d90d674db70552613c316a38403226eb831f7ed3) ...');         if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne '3cd2f93eb25832e7ececa054d90d674db70552613c316a38403226eb831f7ed3') {                 Write-Host 'FAILED!';                 exit 1;         };                 New-Item -ItemType Directory -Path C:\temp | Out-Null;                 Write-Host 'Installing using MSI ...';         Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',         '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome' -Wait -Passthru;         Write-Host 'Removing openjdk.msi ...';         Remove-Item openjdk.msi -Force;         Remove-Item -Path C:\temp -Recurse | Out-Null;
# Wed, 10 Jun 2020 17:02:16 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+UseContainerSupport -XX:+IdleTuningCompactOnIdle -XX:+IdleTuningGcOnIdle
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:375fbabb84945635805b46a02a17ac15a3177bcaae7404cfab5f1ceb0460cb60`  
		Size: 1.7 GB (1664011795 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c938241e0507e1ada5f864325483d86fd08533a5a31e7cb6ec1357db9891b245`  
		Last Modified: Tue, 09 Jun 2020 23:18:33 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4c360094c426e39ad2c8305d957d2b969f91635dfa67304f21b1eca9852931f`  
		Last Modified: Wed, 10 Jun 2020 17:49:07 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4acd242cedd1974d78e1469875dddb36350d3f0be9bba5c98c977e371d8746e3`  
		Last Modified: Wed, 10 Jun 2020 17:50:41 GMT  
		Size: 93.5 MB (93473882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1051878f46098548438a05c0e61a22e49ec3a2851c1a4f66e38c6f8121048e3`  
		Last Modified: Wed, 10 Jun 2020 17:50:28 GMT  
		Size: 1.2 KB (1178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adoptopenjdk:8-jre-openj9` - windows version 10.0.17763.1282; amd64

```console
$ docker pull adoptopenjdk@sha256:7bb54dda5459ed392b8f13806db32561e079363b4cbc3897ad07c139677f3ed3
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2386811138 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b8f26bdbdabe9e39eef027fafe76369309dd8845e339a95a8b486658c71b748`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 04 Jun 2020 01:48:42 GMT
RUN Install update 1809-amd64
# Tue, 09 Jun 2020 22:33:19 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Jun 2020 16:57:55 GMT
ENV JAVA_VERSION=jdk8u252-b09.1_openj9-0.20.0
# Wed, 10 Jun 2020 17:04:03 GMT
RUN Write-Host ('Downloading https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u252-b09.1_openj9-0.20.0/OpenJDK8U-jre_x64_windows_openj9_8u252b09_openj9-0.20.0.msi ...');         [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;         wget https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u252-b09.1_openj9-0.20.0/OpenJDK8U-jre_x64_windows_openj9_8u252b09_openj9-0.20.0.msi -O 'openjdk.msi';         Write-Host ('Verifying sha256 (3cd2f93eb25832e7ececa054d90d674db70552613c316a38403226eb831f7ed3) ...');         if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne '3cd2f93eb25832e7ececa054d90d674db70552613c316a38403226eb831f7ed3') {                 Write-Host 'FAILED!';                 exit 1;         };                 New-Item -ItemType Directory -Path C:\temp | Out-Null;                 Write-Host 'Installing using MSI ...';         Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',         '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome' -Wait -Passthru;         Write-Host 'Removing openjdk.msi ...';         Remove-Item openjdk.msi -Force;         Remove-Item -Path C:\temp -Recurse | Out-Null;
# Wed, 10 Jun 2020 17:04:04 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+UseContainerSupport -XX:+IdleTuningCompactOnIdle -XX:+IdleTuningGcOnIdle
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:666079ee04606f07f4a27dd98526f5049ef8fed93e347d8b4c447b0d5060c77d`  
		Size: 575.6 MB (575581379 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f841c6a0c622cd36b5b2688011a224ac3e8e96273758f4a2804f2f3f099f267d`  
		Last Modified: Tue, 09 Jun 2020 23:17:50 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e19aa9603e414283e8175327dd4a8eb55ad5e9eef24fb3d45bcc662edb416b2`  
		Last Modified: Wed, 10 Jun 2020 17:49:54 GMT  
		Size: 1.1 KB (1086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b44cddfa09242d3412089d30cbf0d25337876d53e4de3df44837122e62216b6`  
		Last Modified: Wed, 10 Jun 2020 17:51:02 GMT  
		Size: 92.9 MB (92893500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30628a6343ac65aec55ab32ff8ee4600a1e7bc5868813947e3a637b2b32cf42c`  
		Last Modified: Wed, 10 Jun 2020 17:50:51 GMT  
		Size: 1.1 KB (1141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
