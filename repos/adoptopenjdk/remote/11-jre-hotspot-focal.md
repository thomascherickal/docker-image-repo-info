## `adoptopenjdk:11-jre-hotspot-focal`

```console
$ docker pull adoptopenjdk@sha256:159de1ea7c06ae8fbfcdda68a1ddf352778364ef2fc61b095923f075766c99e2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `adoptopenjdk:11-jre-hotspot-focal` - linux; amd64

```console
$ docker pull adoptopenjdk@sha256:490a641fd14f65da7097918b8c5a5a86eeddf9af0eb03423bdc51739c49157b4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.7 MB (87730002 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9b377db43b56d8a19c5b76a44c87c845413b0e1bb50a1b5bf6ca0b55ee45c3f`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 23 Apr 2021 22:21:34 GMT
ADD file:5c44a80f547b7d68b550b0e64aef898b361666857abf9a5c8f3f8d0567b8e8e4 in / 
# Fri, 23 Apr 2021 22:21:35 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:21:36 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 22:21:37 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:21:37 GMT
CMD ["/bin/bash"]
# Fri, 23 Apr 2021 23:22:30 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 23 Apr 2021 23:23:01 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Mon, 10 May 2021 18:19:40 GMT
ENV JAVA_VERSION=jdk-11.0.11+9
# Mon, 10 May 2021 18:20:00 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='fde6b29df23b6e7ed6e16a237a0f44273fb9e267fdfbd0b3de5add98e55649f6';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.11%2B9/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.11_9.tar.gz';          ;;        armhf|armv7l)          ESUM='ad02656f800fd64c2b090b23ad24a099d9cd1054948ecb0e9851bc39c51c8be8';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.11%2B9/OpenJDK11U-jre_arm_linux_hotspot_11.0.11_9.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='37c19c7c2d1cea627b854a475ef1a765d30357d765d20cf3f96590037e79d0f3';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.11%2B9/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.11_9.tar.gz';          ;;        s390x)          ESUM='f18101fc50aad795a41b4d3bbc591308c83664fd2390bf2bc007fd9b3d531e6c';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.11%2B9/OpenJDK11U-jre_s390x_linux_hotspot_11.0.11_9.tar.gz';          ;;        amd64|x86_64)          ESUM='144f2c6bcf64faa32016f2474b6c01031be75d25325e9c3097aed6589bc5d548';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.11%2B9/OpenJDK11U-jre_x64_linux_hotspot_11.0.11_9.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Mon, 10 May 2021 18:20:00 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
```

-	Layers:
	-	`sha256:345e3491a907bb7c6f1bdddcf4a94284b8b6ddd77eb7d93f09432b17b20f2bbe`  
		Last Modified: Fri, 16 Apr 2021 15:20:19 GMT  
		Size: 28.5 MB (28539626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57671312ef6fdbecf340e5fed0fb0863350cd806c92b1fdd7978adbd02afc5c3`  
		Last Modified: Fri, 23 Apr 2021 22:23:02 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e9250ddb7d0fa6d13302c7c3e6a0aa40390e42424caed1e5289077ee4054709`  
		Last Modified: Fri, 23 Apr 2021 22:23:02 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:592ec2d7c1370aca6ef48ee1d20fbb3a4c148db400adc5dc575778c681f5dba0`  
		Last Modified: Fri, 23 Apr 2021 23:32:39 GMT  
		Size: 16.0 MB (16034099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73231ab3afed12396f966eeff26d1567d094c8ca19de796d44babc8dc2becd91`  
		Last Modified: Mon, 10 May 2021 18:28:48 GMT  
		Size: 43.2 MB (43155239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adoptopenjdk:11-jre-hotspot-focal` - linux; arm variant v7

```console
$ docker pull adoptopenjdk@sha256:042c25d1cb3337e4c174270e97b80763fd0fbeb3533f1360b778df21beb00ff5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.8 MB (80797170 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f9a11d94c3eb1905e570a9fd6f3713119734973e352fe5e59404156f403ef5a`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 23 Apr 2021 22:36:44 GMT
ADD file:928fc93f670d53bf065ee8446f4af7f103050e96939dfae34f986b5332254115 in / 
# Fri, 23 Apr 2021 22:36:47 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:36:50 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 22:36:51 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:36:52 GMT
CMD ["/bin/bash"]
# Fri, 23 Apr 2021 22:56:43 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 23 Apr 2021 22:57:30 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Mon, 10 May 2021 17:58:38 GMT
ENV JAVA_VERSION=jdk-11.0.11+9
# Mon, 10 May 2021 17:59:31 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='fde6b29df23b6e7ed6e16a237a0f44273fb9e267fdfbd0b3de5add98e55649f6';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.11%2B9/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.11_9.tar.gz';          ;;        armhf|armv7l)          ESUM='ad02656f800fd64c2b090b23ad24a099d9cd1054948ecb0e9851bc39c51c8be8';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.11%2B9/OpenJDK11U-jre_arm_linux_hotspot_11.0.11_9.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='37c19c7c2d1cea627b854a475ef1a765d30357d765d20cf3f96590037e79d0f3';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.11%2B9/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.11_9.tar.gz';          ;;        s390x)          ESUM='f18101fc50aad795a41b4d3bbc591308c83664fd2390bf2bc007fd9b3d531e6c';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.11%2B9/OpenJDK11U-jre_s390x_linux_hotspot_11.0.11_9.tar.gz';          ;;        amd64|x86_64)          ESUM='144f2c6bcf64faa32016f2474b6c01031be75d25325e9c3097aed6589bc5d548';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.11%2B9/OpenJDK11U-jre_x64_linux_hotspot_11.0.11_9.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Mon, 10 May 2021 17:59:33 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
```

-	Layers:
	-	`sha256:cd0d4853c44dd92753bc49779ae8c6f5bd76ba358989832b5afa42e3a341b4eb`  
		Last Modified: Fri, 23 Apr 2021 22:40:15 GMT  
		Size: 24.0 MB (24038553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3438cfd01915ec245a55dd1047748b26e29a31f4e630766126666c6bc9953a71`  
		Last Modified: Fri, 23 Apr 2021 22:40:09 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cfc3cbbc3a3f69a5c07b934f21be14f7006510ff7a327d2f05f94ff680084d5`  
		Last Modified: Fri, 23 Apr 2021 22:40:09 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c97d902259d822138b34542420feb5d3f49d3e1fe100a791a2a42bcdce4a4b8e`  
		Last Modified: Fri, 23 Apr 2021 23:03:13 GMT  
		Size: 14.9 MB (14899197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d77e69704451ebbccf37c97efc2e7dc53949c705586c8be3728cecda7dc8b83`  
		Last Modified: Mon, 10 May 2021 18:03:39 GMT  
		Size: 41.9 MB (41858384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adoptopenjdk:11-jre-hotspot-focal` - linux; arm64 variant v8

```console
$ docker pull adoptopenjdk@sha256:d70de25b6c10f8e82031253eefc9088d73786029ee44ec3f5692bab43a8a33d1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.5 MB (84506772 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:779ce746f966059cf5ca10cf7ac1205de849d16c3fbb0473bac389466817ca0a`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 23 Apr 2021 22:47:51 GMT
ADD file:57e6f432b1329c286e596ded8065bebdfc70a87fae91dd79bd805363ef008e5d in / 
# Fri, 23 Apr 2021 22:47:54 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:47:57 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 22:47:59 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:47:59 GMT
CMD ["/bin/bash"]
# Fri, 23 Apr 2021 23:13:07 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 23 Apr 2021 23:13:41 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Mon, 10 May 2021 17:40:15 GMT
ENV JAVA_VERSION=jdk-11.0.11+9
# Mon, 10 May 2021 17:40:42 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='fde6b29df23b6e7ed6e16a237a0f44273fb9e267fdfbd0b3de5add98e55649f6';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.11%2B9/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.11_9.tar.gz';          ;;        armhf|armv7l)          ESUM='ad02656f800fd64c2b090b23ad24a099d9cd1054948ecb0e9851bc39c51c8be8';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.11%2B9/OpenJDK11U-jre_arm_linux_hotspot_11.0.11_9.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='37c19c7c2d1cea627b854a475ef1a765d30357d765d20cf3f96590037e79d0f3';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.11%2B9/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.11_9.tar.gz';          ;;        s390x)          ESUM='f18101fc50aad795a41b4d3bbc591308c83664fd2390bf2bc007fd9b3d531e6c';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.11%2B9/OpenJDK11U-jre_s390x_linux_hotspot_11.0.11_9.tar.gz';          ;;        amd64|x86_64)          ESUM='144f2c6bcf64faa32016f2474b6c01031be75d25325e9c3097aed6589bc5d548';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.11%2B9/OpenJDK11U-jre_x64_linux_hotspot_11.0.11_9.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Mon, 10 May 2021 17:40:43 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
```

-	Layers:
	-	`sha256:80bc30679ac1fd798f3241208c14accd6a364cb8a6224d1127dfb1577d10554f`  
		Last Modified: Fri, 16 Apr 2021 08:25:26 GMT  
		Size: 27.1 MB (27144417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bf18fab4cfbf479fa9f8409ad47e2702c63241304c2cdd4c33f2a1633c5f85e`  
		Last Modified: Fri, 23 Apr 2021 22:50:04 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5979309c983a2adeff352538937475cf961d49c34194fa2aab142effe19ed9c1`  
		Last Modified: Fri, 23 Apr 2021 22:50:04 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6482171366cbde14bd4de2fe7eade385c2d307e224a008056f39e553b9c93d7`  
		Last Modified: Fri, 23 Apr 2021 23:18:01 GMT  
		Size: 15.9 MB (15895133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:346e1b8b8ce5a7b50141c05c9cd1d3584013717e60423800ee5d3b6ab224760c`  
		Last Modified: Mon, 10 May 2021 17:43:55 GMT  
		Size: 41.5 MB (41466183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adoptopenjdk:11-jre-hotspot-focal` - linux; ppc64le

```console
$ docker pull adoptopenjdk@sha256:87bdfb307963e844eeddb4e72745bc6923da1f95cdadb707aaec6daaa5fd2989
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **89.1 MB (89055696 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31cc221442783a0b2f9232300d998b6b31b73261394e6e355e8fe77f0e394bd8`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 23 Apr 2021 22:31:45 GMT
ADD file:ec80070ca931734843261734e9ca18cd45a6130030c1a25abac3268e54776be5 in / 
# Fri, 23 Apr 2021 22:32:02 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:32:15 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 22:32:33 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:32:38 GMT
CMD ["/bin/bash"]
# Sat, 24 Apr 2021 01:16:16 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Sat, 24 Apr 2021 01:19:33 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Mon, 10 May 2021 18:18:08 GMT
ENV JAVA_VERSION=jdk-11.0.11+9
# Mon, 10 May 2021 18:19:05 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='fde6b29df23b6e7ed6e16a237a0f44273fb9e267fdfbd0b3de5add98e55649f6';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.11%2B9/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.11_9.tar.gz';          ;;        armhf|armv7l)          ESUM='ad02656f800fd64c2b090b23ad24a099d9cd1054948ecb0e9851bc39c51c8be8';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.11%2B9/OpenJDK11U-jre_arm_linux_hotspot_11.0.11_9.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='37c19c7c2d1cea627b854a475ef1a765d30357d765d20cf3f96590037e79d0f3';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.11%2B9/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.11_9.tar.gz';          ;;        s390x)          ESUM='f18101fc50aad795a41b4d3bbc591308c83664fd2390bf2bc007fd9b3d531e6c';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.11%2B9/OpenJDK11U-jre_s390x_linux_hotspot_11.0.11_9.tar.gz';          ;;        amd64|x86_64)          ESUM='144f2c6bcf64faa32016f2474b6c01031be75d25325e9c3097aed6589bc5d548';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.11%2B9/OpenJDK11U-jre_x64_linux_hotspot_11.0.11_9.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Mon, 10 May 2021 18:19:14 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
```

-	Layers:
	-	`sha256:8cdb522ceff72cef6133f5b26b5f9eac72760a06a86d5d6b7db34a5dde7b156f`  
		Last Modified: Fri, 23 Apr 2021 22:37:11 GMT  
		Size: 33.3 MB (33255388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21136d6107eea0892211e712ba6b20d15f74a37dd1bde1b2f0802e083e85c183`  
		Last Modified: Fri, 23 Apr 2021 22:37:05 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a03f1456f472e398050e94cf3ac8873969ce172a153bb511be780fe49403c47`  
		Last Modified: Fri, 23 Apr 2021 22:37:05 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da07529aeac8fe5c90c5bb8c4f516c9d6fd248cc1daa5fecd137c809bce39bb6`  
		Last Modified: Sat, 24 Apr 2021 01:40:58 GMT  
		Size: 17.2 MB (17209103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c0ff0b8e3f27c68d5e722b66390d28c1aaf5468ef1ad4ffd24dc4646fc2dee4`  
		Last Modified: Mon, 10 May 2021 18:35:57 GMT  
		Size: 38.6 MB (38590169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adoptopenjdk:11-jre-hotspot-focal` - linux; s390x

```console
$ docker pull adoptopenjdk@sha256:42982a6dd8cdeb1d02314e08f42874c1eff58d34f027e1db27c6f68e580c7e36
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.4 MB (80396845 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bca38b0d012a0f368b7aedf75ca0c519c4e52368a90eabe1bb19dd546a6ed2af`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 23 Apr 2021 21:45:20 GMT
ADD file:282d950116f923276efabd13c7dc17b942821edb14ffac4b89b9a50bcdf99e17 in / 
# Fri, 23 Apr 2021 21:45:26 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 21:45:27 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 21:45:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 21:45:29 GMT
CMD ["/bin/bash"]
# Fri, 23 Apr 2021 22:03:30 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 23 Apr 2021 22:04:03 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Mon, 10 May 2021 17:43:08 GMT
ENV JAVA_VERSION=jdk-11.0.11+9
# Mon, 10 May 2021 17:44:13 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='fde6b29df23b6e7ed6e16a237a0f44273fb9e267fdfbd0b3de5add98e55649f6';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.11%2B9/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.11_9.tar.gz';          ;;        armhf|armv7l)          ESUM='ad02656f800fd64c2b090b23ad24a099d9cd1054948ecb0e9851bc39c51c8be8';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.11%2B9/OpenJDK11U-jre_arm_linux_hotspot_11.0.11_9.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='37c19c7c2d1cea627b854a475ef1a765d30357d765d20cf3f96590037e79d0f3';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.11%2B9/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.11_9.tar.gz';          ;;        s390x)          ESUM='f18101fc50aad795a41b4d3bbc591308c83664fd2390bf2bc007fd9b3d531e6c';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.11%2B9/OpenJDK11U-jre_s390x_linux_hotspot_11.0.11_9.tar.gz';          ;;        amd64|x86_64)          ESUM='144f2c6bcf64faa32016f2474b6c01031be75d25325e9c3097aed6589bc5d548';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.11%2B9/OpenJDK11U-jre_x64_linux_hotspot_11.0.11_9.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Mon, 10 May 2021 17:44:16 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
```

-	Layers:
	-	`sha256:de53239ada2db01e7972c3f6eddcf6729f7cf3102be78e0b41363125ce7c2425`  
		Last Modified: Fri, 23 Apr 2021 21:47:14 GMT  
		Size: 27.1 MB (27136362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12932016d0f51acb5c5e5ba5b420a369401a7df47a219f24680bbc05ffde7e11`  
		Last Modified: Fri, 23 Apr 2021 21:47:10 GMT  
		Size: 840.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46997f76c5876e3274170b667463b3d88475cd696ccbc735d2f63965668673ad`  
		Last Modified: Fri, 23 Apr 2021 21:47:10 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bab416938acf6dd045c9fc9097e5768c61b5899b07d110ab3844f447e12b113`  
		Last Modified: Fri, 23 Apr 2021 22:19:05 GMT  
		Size: 15.7 MB (15741779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48d7f49a7eb5c004b6adb96ed99cc46bff270617a72b0a32ff9df2f8b97d1777`  
		Last Modified: Mon, 10 May 2021 18:00:25 GMT  
		Size: 37.5 MB (37517678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
