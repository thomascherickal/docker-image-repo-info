## `adoptopenjdk:8-jre-hotspot-bionic`

```console
$ docker pull adoptopenjdk@sha256:5e5f1e717ad4720502d99fa8dee20d1912b235ae1d5875a84b31572be24e50f5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `adoptopenjdk:8-jre-hotspot-bionic` - linux; amd64

```console
$ docker pull adoptopenjdk@sha256:36f967c4af4bcb5616fd48125d98cf74096498e661c01c238456da3d5aa0ebe2
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.5 MB (81490354 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23c63e57953ee43d78a5614f74ec1ba08e87840fd8c02931551b0a953a2f7305`
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
# Wed, 17 Jun 2020 01:46:25 GMT
ENV JAVA_VERSION=jdk8u252-b09
# Wed, 17 Jun 2020 01:46:43 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='30bba4425497f5b4aabcba7b45db69d582d278fb17357d64c22c9dc6b2d29ca1';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u252-b09/OpenJDK8U-jre_aarch64_linux_hotspot_8u252b09.tar.gz';          ;;        armhf|armv7l)          ESUM='107699a88f611e0c2d57816be25821ef9b17db860b14402c4e9e5bf0b9cf16fd';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u252-b09/OpenJDK8U-jre_arm_linux_hotspot_8u252b09.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='fbc559e8f75107f3c2ef92b33938dd48aee5728d471774d04fa3f68ed3b992fe';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u252-b09/OpenJDK8U-jre_ppc64le_linux_hotspot_8u252b09.tar.gz';          ;;        s390x)          ESUM='23daa316ebcd965197e74dff011708a050516cd108a27a40e5b5cfa3c88beaba';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u252-b09/OpenJDK8U-jre_s390x_linux_hotspot_8u252b09.tar.gz';          ;;        amd64|x86_64)          ESUM='a93be303ed62398dba9acb0376fb3caf8f488fcde80dc62d0a8e46256b3adfb1';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u252-b09/OpenJDK8U-jre_x64_linux_hotspot_8u252b09.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 17 Jun 2020 01:46:43 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
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
	-	`sha256:f1e1ecb02e286efcc00d80efac1a03cb5bb9f30149a57793f03f94765d5ac56c`  
		Last Modified: Wed, 17 Jun 2020 01:50:36 GMT  
		Size: 41.5 MB (41453810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adoptopenjdk:8-jre-hotspot-bionic` - linux; arm variant v7

```console
$ docker pull adoptopenjdk@sha256:a24b3236262535082b2f5a469229b654cfbb9177e5c56a5f3390b02ca886e688
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.8 MB (72783677 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce08e63905576650face6612eb9fc38d41e207aa39a34871b059896fdb43bf0b`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 17 Jun 2020 02:02:00 GMT
ADD file:579f3bbed274bd8ec97aa5bfc4eb09fdcfe3e12e37fb3739f3096138b765581c in / 
# Wed, 17 Jun 2020 02:02:04 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 17 Jun 2020 02:02:06 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 17 Jun 2020 02:02:09 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 17 Jun 2020 02:02:09 GMT
CMD ["/bin/bash"]
# Wed, 17 Jun 2020 02:21:36 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 17 Jun 2020 02:22:23 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 17 Jun 2020 02:22:27 GMT
ENV JAVA_VERSION=jdk8u252-b09
# Wed, 17 Jun 2020 02:23:00 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='30bba4425497f5b4aabcba7b45db69d582d278fb17357d64c22c9dc6b2d29ca1';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u252-b09/OpenJDK8U-jre_aarch64_linux_hotspot_8u252b09.tar.gz';          ;;        armhf|armv7l)          ESUM='107699a88f611e0c2d57816be25821ef9b17db860b14402c4e9e5bf0b9cf16fd';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u252-b09/OpenJDK8U-jre_arm_linux_hotspot_8u252b09.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='fbc559e8f75107f3c2ef92b33938dd48aee5728d471774d04fa3f68ed3b992fe';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u252-b09/OpenJDK8U-jre_ppc64le_linux_hotspot_8u252b09.tar.gz';          ;;        s390x)          ESUM='23daa316ebcd965197e74dff011708a050516cd108a27a40e5b5cfa3c88beaba';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u252-b09/OpenJDK8U-jre_s390x_linux_hotspot_8u252b09.tar.gz';          ;;        amd64|x86_64)          ESUM='a93be303ed62398dba9acb0376fb3caf8f488fcde80dc62d0a8e46256b3adfb1';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u252-b09/OpenJDK8U-jre_x64_linux_hotspot_8u252b09.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 17 Jun 2020 02:23:01 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
```

-	Layers:
	-	`sha256:2d63ac53d1bca136340c80fe8b64c0b8e2d9a62eddb6fcb794c489840dc027d6`  
		Last Modified: Sat, 30 May 2020 09:27:47 GMT  
		Size: 22.3 MB (22275987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30e03e3a8e7321c64d7a483fc9cc0054ce81e5b230b32300b7c68d21001f661a`  
		Last Modified: Wed, 17 Jun 2020 02:05:28 GMT  
		Size: 35.5 KB (35459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee0e8090890c513488a0f67683f23dcfcfbf2b67e5be854edf1323ad87a60b26`  
		Last Modified: Wed, 17 Jun 2020 02:05:28 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b801ccb19e43939aa60383f674f0e1f65ab062890870d42d0fa7a7a62fc5b708`  
		Last Modified: Wed, 17 Jun 2020 02:05:28 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2017d9990116042cb5263605aec3eea45f40a52df7fe3e4125aab0afc62fafb5`  
		Last Modified: Wed, 17 Jun 2020 02:26:17 GMT  
		Size: 12.3 MB (12253416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:108216c7825758332ebec96e23ba29e1ed6d6a0d5c8fdc7ed0a850d99b00f886`  
		Last Modified: Wed, 17 Jun 2020 02:26:48 GMT  
		Size: 38.2 MB (38217773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adoptopenjdk:8-jre-hotspot-bionic` - linux; arm64 variant v8

```console
$ docker pull adoptopenjdk@sha256:9d9781c9a9ce807b8e8ab9c28876d0377da8b805cceca266eaa01a717396371e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **78.0 MB (78004787 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:62adde0bba4352b9b98a12de71156236b49ae970155a1d093cbc9b230e8a4eca`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 17 Jun 2020 01:42:33 GMT
ADD file:7dc8819fd3d4b84ad19fb836e5bfda64a5ffefc371166f70d4d41dff6b22d450 in / 
# Wed, 17 Jun 2020 01:42:37 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 17 Jun 2020 01:42:41 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 17 Jun 2020 01:42:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 17 Jun 2020 01:42:45 GMT
CMD ["/bin/bash"]
# Wed, 17 Jun 2020 02:01:31 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 17 Jun 2020 02:02:15 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 17 Jun 2020 02:02:16 GMT
ENV JAVA_VERSION=jdk8u252-b09
# Wed, 17 Jun 2020 02:02:51 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='30bba4425497f5b4aabcba7b45db69d582d278fb17357d64c22c9dc6b2d29ca1';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u252-b09/OpenJDK8U-jre_aarch64_linux_hotspot_8u252b09.tar.gz';          ;;        armhf|armv7l)          ESUM='107699a88f611e0c2d57816be25821ef9b17db860b14402c4e9e5bf0b9cf16fd';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u252-b09/OpenJDK8U-jre_arm_linux_hotspot_8u252b09.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='fbc559e8f75107f3c2ef92b33938dd48aee5728d471774d04fa3f68ed3b992fe';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u252-b09/OpenJDK8U-jre_ppc64le_linux_hotspot_8u252b09.tar.gz';          ;;        s390x)          ESUM='23daa316ebcd965197e74dff011708a050516cd108a27a40e5b5cfa3c88beaba';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u252-b09/OpenJDK8U-jre_s390x_linux_hotspot_8u252b09.tar.gz';          ;;        amd64|x86_64)          ESUM='a93be303ed62398dba9acb0376fb3caf8f488fcde80dc62d0a8e46256b3adfb1';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u252-b09/OpenJDK8U-jre_x64_linux_hotspot_8u252b09.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 17 Jun 2020 02:02:53 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
```

-	Layers:
	-	`sha256:2e8bea8b22f8f5a4fd5aa85019945dd8ae04f283a4ba2a7aeb4536fe2f1d1ec2`  
		Last Modified: Tue, 26 May 2020 16:25:25 GMT  
		Size: 23.7 MB (23721687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc90876b9c9a7343ae432eaec7c8dc8859c1e84b6193da8d386815fde165a70e`  
		Last Modified: Wed, 17 Jun 2020 01:44:48 GMT  
		Size: 35.2 KB (35192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27bfc658a5210a9f0c9cfcda5f504e720da9268e9f3f3bf48e3a9a7af360c959`  
		Last Modified: Wed, 17 Jun 2020 01:44:49 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ef0f1b06b2142ff2bf35cc565f019ed9e4efe0d8f332825167538c2337bac8a`  
		Last Modified: Wed, 17 Jun 2020 01:44:49 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de2f160cb2104283349d8893782d7f4379a3036ec17d63d467db1663360840cd`  
		Last Modified: Wed, 17 Jun 2020 02:06:13 GMT  
		Size: 12.7 MB (12722860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a80e5184266600995e6004e0216cf2520a8b9dde7c477096c7527ccef5b7498`  
		Last Modified: Wed, 17 Jun 2020 02:06:46 GMT  
		Size: 41.5 MB (41524007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adoptopenjdk:8-jre-hotspot-bionic` - linux; ppc64le

```console
$ docker pull adoptopenjdk@sha256:f712cd09ae1907208f799d1ebc0920ef98b4e433eddd0a849e552aaff43f5903
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.9 MB (84921724 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0766fd6c5a90124fd445c9886111214175c3074a795a006a8806e8ae7e4467cc`
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
# Wed, 17 Jun 2020 03:27:02 GMT
ENV JAVA_VERSION=jdk8u252-b09
# Wed, 17 Jun 2020 03:28:04 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='30bba4425497f5b4aabcba7b45db69d582d278fb17357d64c22c9dc6b2d29ca1';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u252-b09/OpenJDK8U-jre_aarch64_linux_hotspot_8u252b09.tar.gz';          ;;        armhf|armv7l)          ESUM='107699a88f611e0c2d57816be25821ef9b17db860b14402c4e9e5bf0b9cf16fd';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u252-b09/OpenJDK8U-jre_arm_linux_hotspot_8u252b09.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='fbc559e8f75107f3c2ef92b33938dd48aee5728d471774d04fa3f68ed3b992fe';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u252-b09/OpenJDK8U-jre_ppc64le_linux_hotspot_8u252b09.tar.gz';          ;;        s390x)          ESUM='23daa316ebcd965197e74dff011708a050516cd108a27a40e5b5cfa3c88beaba';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u252-b09/OpenJDK8U-jre_s390x_linux_hotspot_8u252b09.tar.gz';          ;;        amd64|x86_64)          ESUM='a93be303ed62398dba9acb0376fb3caf8f488fcde80dc62d0a8e46256b3adfb1';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u252-b09/OpenJDK8U-jre_x64_linux_hotspot_8u252b09.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 17 Jun 2020 03:28:11 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
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
	-	`sha256:90739ca271e82feff463d6af0e29086f490f7edbabf11442d42c6716eb1d7793`  
		Last Modified: Wed, 17 Jun 2020 03:39:38 GMT  
		Size: 40.5 MB (40529112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adoptopenjdk:8-jre-hotspot-bionic` - linux; s390x

```console
$ docker pull adoptopenjdk@sha256:838fafa473cca58b9823ca1bfd79b2d8715bfedb51a36406567ce9cf6ebf3e9e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.6 MB (77596629 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:59590d76468721e8272e26d5835973670cc1284c67b7d7e32fc4fdb4ef7ca87e`
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
# Wed, 17 Jun 2020 02:58:01 GMT
ENV JAVA_VERSION=jdk8u252-b09
# Wed, 17 Jun 2020 02:58:23 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='30bba4425497f5b4aabcba7b45db69d582d278fb17357d64c22c9dc6b2d29ca1';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u252-b09/OpenJDK8U-jre_aarch64_linux_hotspot_8u252b09.tar.gz';          ;;        armhf|armv7l)          ESUM='107699a88f611e0c2d57816be25821ef9b17db860b14402c4e9e5bf0b9cf16fd';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u252-b09/OpenJDK8U-jre_arm_linux_hotspot_8u252b09.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='fbc559e8f75107f3c2ef92b33938dd48aee5728d471774d04fa3f68ed3b992fe';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u252-b09/OpenJDK8U-jre_ppc64le_linux_hotspot_8u252b09.tar.gz';          ;;        s390x)          ESUM='23daa316ebcd965197e74dff011708a050516cd108a27a40e5b5cfa3c88beaba';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u252-b09/OpenJDK8U-jre_s390x_linux_hotspot_8u252b09.tar.gz';          ;;        amd64|x86_64)          ESUM='a93be303ed62398dba9acb0376fb3caf8f488fcde80dc62d0a8e46256b3adfb1';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u252-b09/OpenJDK8U-jre_x64_linux_hotspot_8u252b09.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 17 Jun 2020 02:58:24 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
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
	-	`sha256:aee46b9fe182d21365e8cdc34cb6193109e0a28fb642d936c3076a65c954e59b`  
		Last Modified: Wed, 17 Jun 2020 03:03:14 GMT  
		Size: 39.2 MB (39161268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
