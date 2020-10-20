## `adoptopenjdk:15_36-jre-hotspot`

```console
$ docker pull adoptopenjdk@sha256:958fc05fb32c82f00d46db4e3c368231eae021737f96bdeb4d497b16bbc268eb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; s390x
	-	windows version 10.0.17763.1518; amd64
	-	windows version 10.0.14393.3986; amd64

### `adoptopenjdk:15_36-jre-hotspot` - linux; amd64

```console
$ docker pull adoptopenjdk@sha256:05558695b478684760afcedbe576ad379b5e0fd69ed3949f273334e61744d34f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.4 MB (99437791 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ca6a74fa8285e2689027fac77fe8073095532a771c8b6e207e2de3a1de216bb`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 25 Sep 2020 22:33:49 GMT
ADD file:4974bb5483c392fb54a35f3799802d623d14632747493dce5feb4d435634b4ac in / 
# Fri, 25 Sep 2020 22:33:50 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 25 Sep 2020 22:33:51 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 25 Sep 2020 22:33:52 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 25 Sep 2020 22:33:52 GMT
CMD ["/bin/bash"]
# Fri, 25 Sep 2020 23:10:55 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 25 Sep 2020 23:11:26 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 20 Oct 2020 17:04:16 GMT
ENV JAVA_VERSION=jdk-15+36
# Tue, 20 Oct 2020 17:04:39 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='318f50bae6652d4468ee262ce0fd6569adbc461bea0d1ecce77ce2843efee8d4';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15%2B36/OpenJDK15U-jre_aarch64_linux_hotspot_15_36.tar.gz';          ;;        armhf|armv7l)          ESUM='09c1ba3636e7899d8b43795d7988bcc4b1e1be2919764d94f6d4a1a855ce774f';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15%2B36/OpenJDK15U-jre_arm_linux_hotspot_15_36.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='6ea692c7e43bee201a56313bd9f4ddcdea43bed1dfe203c49316ac4d08a4cdd3';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15%2B36/OpenJDK15U-jre_ppc64le_linux_hotspot_15_36.tar.gz';          ;;        s390x)          ESUM='e1e124a29e2bf892d267eb63d00dd136558b4e276bcb6741ea676c995b2fff51';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15%2B36/OpenJDK15U-jre_s390x_linux_hotspot_15_36.tar.gz';          ;;        amd64|x86_64)          ESUM='230d97a6b16a0735f15013a91f7582a22282ec12bdfaec291ab63274cc075efb';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15%2B36/OpenJDK15U-jre_x64_linux_hotspot_15_36.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 20 Oct 2020 17:04:40 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
```

-	Layers:
	-	`sha256:171857c49d0f5e2ebf623e6cb36a8bcad585ed0c2aa99c87a055df034c1e5848`  
		Last Modified: Tue, 22 Sep 2020 12:21:27 GMT  
		Size: 26.7 MB (26701612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:419640447d267f068d2f84a093cb13a56ce77e130877f5b8bdb4294f4a90a84f`  
		Last Modified: Fri, 25 Sep 2020 22:36:49 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61e52f862619ab016d3bcfbd78e5c7aaaa1989b4c295e6dbcacddd2d7b93e1f5`  
		Last Modified: Fri, 25 Sep 2020 22:36:49 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd4d4e9526b1adecc10515315b09e75d88526e75fba0552b3fbb933f40d293e9`  
		Last Modified: Fri, 25 Sep 2020 23:16:31 GMT  
		Size: 13.9 MB (13875646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2500549fac1fa4d18eea43c0c3a613a0be99fa4938f7a0c1b1c9e4fa4f918b37`  
		Last Modified: Tue, 20 Oct 2020 17:21:25 GMT  
		Size: 58.9 MB (58859519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adoptopenjdk:15_36-jre-hotspot` - linux; arm variant v7

```console
$ docker pull adoptopenjdk@sha256:275616a5dc9d0a2970d881e02a98c96168331adcde7e326f417032aa6ffff157
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **89.4 MB (89389681 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f48ed39417851d9b48e44027fa35826365662abbe10fac4f594aa80750ffa6d`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 25 Sep 2020 23:04:32 GMT
ADD file:0ddc5fefae097a5be4c925fdfc09e4a637b74627a8981f0e6fb9890580adc875 in / 
# Fri, 25 Sep 2020 23:04:35 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 25 Sep 2020 23:04:37 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 25 Sep 2020 23:04:39 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 25 Sep 2020 23:04:40 GMT
CMD ["/bin/bash"]
# Fri, 25 Sep 2020 23:23:09 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 25 Sep 2020 23:23:39 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 20 Oct 2020 17:01:39 GMT
ENV JAVA_VERSION=jdk-15+36
# Tue, 20 Oct 2020 17:02:21 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='318f50bae6652d4468ee262ce0fd6569adbc461bea0d1ecce77ce2843efee8d4';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15%2B36/OpenJDK15U-jre_aarch64_linux_hotspot_15_36.tar.gz';          ;;        armhf|armv7l)          ESUM='09c1ba3636e7899d8b43795d7988bcc4b1e1be2919764d94f6d4a1a855ce774f';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15%2B36/OpenJDK15U-jre_arm_linux_hotspot_15_36.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='6ea692c7e43bee201a56313bd9f4ddcdea43bed1dfe203c49316ac4d08a4cdd3';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15%2B36/OpenJDK15U-jre_ppc64le_linux_hotspot_15_36.tar.gz';          ;;        s390x)          ESUM='e1e124a29e2bf892d267eb63d00dd136558b4e276bcb6741ea676c995b2fff51';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15%2B36/OpenJDK15U-jre_s390x_linux_hotspot_15_36.tar.gz';          ;;        amd64|x86_64)          ESUM='230d97a6b16a0735f15013a91f7582a22282ec12bdfaec291ab63274cc075efb';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15%2B36/OpenJDK15U-jre_x64_linux_hotspot_15_36.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 20 Oct 2020 17:02:23 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
```

-	Layers:
	-	`sha256:20e126218ac644f56ef7147c3363108a0814d921e6016af54a1b4c964159f1a9`  
		Last Modified: Fri, 25 Sep 2020 23:06:39 GMT  
		Size: 22.3 MB (22279517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d156c2b31482935ec0363b6e3f1cb6fc56da57e61fc80078914918fe53f8fa5`  
		Last Modified: Fri, 25 Sep 2020 23:06:34 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93c1a0dbe2162972438aa89d4f90dca5db0e4cee58819ba354ea1c0031101b7a`  
		Last Modified: Fri, 25 Sep 2020 23:06:34 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b333d1b8f5fe5303d427301eecab31e2fb825ddfe9ed1f96b70bc80a74f9fa44`  
		Last Modified: Fri, 25 Sep 2020 23:27:19 GMT  
		Size: 12.8 MB (12817173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caca04f9411fa11c37ece5fc7dc59b3dc49eceb4cc7706827a3f4cdc5177d736`  
		Last Modified: Tue, 20 Oct 2020 17:05:31 GMT  
		Size: 54.3 MB (54291953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adoptopenjdk:15_36-jre-hotspot` - linux; arm64 variant v8

```console
$ docker pull adoptopenjdk@sha256:52e7f0417cc7d61fb46bf286007df286ae39269c545686ce40d0bdba981883f3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.7 MB (94655475 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ab9bd29cbd9c7245c39c4d20cf81122ea58e3f4769664f18ae8e12340095a71`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 25 Sep 2020 22:47:32 GMT
ADD file:d2c57bfbb29f6de3b29050a2c50c3806e0c8caa26f6d8dea47f479c923d72e3e in / 
# Fri, 25 Sep 2020 22:47:35 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 25 Sep 2020 22:47:36 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 25 Sep 2020 22:47:38 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 25 Sep 2020 22:47:39 GMT
CMD ["/bin/bash"]
# Fri, 25 Sep 2020 23:06:10 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 25 Sep 2020 23:06:39 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 20 Oct 2020 16:40:46 GMT
ENV JAVA_VERSION=jdk-15+36
# Tue, 20 Oct 2020 16:41:17 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='318f50bae6652d4468ee262ce0fd6569adbc461bea0d1ecce77ce2843efee8d4';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15%2B36/OpenJDK15U-jre_aarch64_linux_hotspot_15_36.tar.gz';          ;;        armhf|armv7l)          ESUM='09c1ba3636e7899d8b43795d7988bcc4b1e1be2919764d94f6d4a1a855ce774f';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15%2B36/OpenJDK15U-jre_arm_linux_hotspot_15_36.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='6ea692c7e43bee201a56313bd9f4ddcdea43bed1dfe203c49316ac4d08a4cdd3';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15%2B36/OpenJDK15U-jre_ppc64le_linux_hotspot_15_36.tar.gz';          ;;        s390x)          ESUM='e1e124a29e2bf892d267eb63d00dd136558b4e276bcb6741ea676c995b2fff51';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15%2B36/OpenJDK15U-jre_s390x_linux_hotspot_15_36.tar.gz';          ;;        amd64|x86_64)          ESUM='230d97a6b16a0735f15013a91f7582a22282ec12bdfaec291ab63274cc075efb';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15%2B36/OpenJDK15U-jre_x64_linux_hotspot_15_36.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 20 Oct 2020 16:41:18 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
```

-	Layers:
	-	`sha256:296c9ad75beec603486f1373addae8e2c509e94c4adda44c1289792c91624acc`  
		Last Modified: Tue, 22 Sep 2020 00:25:11 GMT  
		Size: 23.7 MB (23722853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0533d1393025aa8c38e0823a6546a0d4e5dec6b8b670758c25494c35783668d`  
		Last Modified: Fri, 25 Sep 2020 22:49:19 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c11bb34abc87247c6a70c928b7a5ef4cd48093642eb0c4b8121a674d3e278c6`  
		Last Modified: Fri, 25 Sep 2020 22:49:19 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2ba57826dc24dd7e679051972f0a6da7be0dff04d2354108e340a12813e9ff9`  
		Last Modified: Fri, 25 Sep 2020 23:09:59 GMT  
		Size: 13.3 MB (13284869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2286e97cf94639c740a0076578ab750ab56dd9d75a45bce46d4826b731c7d738`  
		Last Modified: Tue, 20 Oct 2020 16:48:20 GMT  
		Size: 57.6 MB (57646714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adoptopenjdk:15_36-jre-hotspot` - linux; s390x

```console
$ docker pull adoptopenjdk@sha256:2af77ba1451d5eab30039cea538b086b979dfeb11390d1dbb1a9e5994fc84bcc
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.9 MB (91897653 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4924adb7fa0905f887748d7f2e1fd3943adc5253eb6e8cfb9a4a7d0ca7bff69a`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 25 Sep 2020 22:44:45 GMT
ADD file:0a8ec4fb62616b6605197e20e0a7b511dc5b03d4af0e04c929dfd9fb457d2065 in / 
# Fri, 25 Sep 2020 22:44:47 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 25 Sep 2020 22:44:48 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 25 Sep 2020 22:44:48 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 25 Sep 2020 22:44:48 GMT
CMD ["/bin/bash"]
# Fri, 25 Sep 2020 23:07:22 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 25 Sep 2020 23:07:34 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 20 Oct 2020 16:42:16 GMT
ENV JAVA_VERSION=jdk-15+36
# Tue, 20 Oct 2020 16:42:42 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='318f50bae6652d4468ee262ce0fd6569adbc461bea0d1ecce77ce2843efee8d4';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15%2B36/OpenJDK15U-jre_aarch64_linux_hotspot_15_36.tar.gz';          ;;        armhf|armv7l)          ESUM='09c1ba3636e7899d8b43795d7988bcc4b1e1be2919764d94f6d4a1a855ce774f';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15%2B36/OpenJDK15U-jre_arm_linux_hotspot_15_36.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='6ea692c7e43bee201a56313bd9f4ddcdea43bed1dfe203c49316ac4d08a4cdd3';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15%2B36/OpenJDK15U-jre_ppc64le_linux_hotspot_15_36.tar.gz';          ;;        s390x)          ESUM='e1e124a29e2bf892d267eb63d00dd136558b4e276bcb6741ea676c995b2fff51';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15%2B36/OpenJDK15U-jre_s390x_linux_hotspot_15_36.tar.gz';          ;;        amd64|x86_64)          ESUM='230d97a6b16a0735f15013a91f7582a22282ec12bdfaec291ab63274cc075efb';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15%2B36/OpenJDK15U-jre_x64_linux_hotspot_15_36.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 20 Oct 2020 16:42:44 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
```

-	Layers:
	-	`sha256:dd2de95b9a1c45e92bcc791d469201229b58d68187c99de6b08b00a13fa33393`  
		Last Modified: Fri, 25 Sep 2020 22:45:52 GMT  
		Size: 25.4 MB (25371975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c38a48ef4dfab2bd639d381d11b3390b6bf8860b2ef3356e9bb55f7cb8c775f9`  
		Last Modified: Fri, 25 Sep 2020 22:45:51 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eced51184728468b347a6e3f143c356cd174c4a54be3cc10ec5aeddb402765fd`  
		Last Modified: Fri, 25 Sep 2020 22:45:49 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62eb688908dd55f188cb3c2b3bb83efc30566ace847ab51ba28adbed5d30266b`  
		Last Modified: Fri, 25 Sep 2020 23:12:47 GMT  
		Size: 13.6 MB (13595725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79611366ecdbd8e854009508a25425f8311bc5d7010f71762a8fe4c7d5e576f6`  
		Last Modified: Tue, 20 Oct 2020 16:58:37 GMT  
		Size: 52.9 MB (52928916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adoptopenjdk:15_36-jre-hotspot` - windows version 10.0.17763.1518; amd64

```console
$ docker pull adoptopenjdk@sha256:2c23536bd9acd126e7e9c4bea2c4e6ca1f4dea56e759daca2cff6ee638f025b0
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2474485813 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c9a5f758a75ba4ad5b2402428b3a43b22607967b93ed7d93b3a75820cb1bcc4`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 01 Oct 2020 02:26:38 GMT
RUN Install update 1809-amd64
# Wed, 14 Oct 2020 12:27:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Sat, 17 Oct 2020 01:04:29 GMT
ENV JAVA_VERSION=jdk-15+36
# Sat, 17 Oct 2020 01:12:19 GMT
RUN Write-Host ('Downloading https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15%2B36/OpenJDK15U-jre_x64_windows_hotspot_15_36.msi ...');     [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     wget https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15%2B36/OpenJDK15U-jre_x64_windows_hotspot_15_36.msi -O 'openjdk.msi';     Write-Host ('Verifying sha256 (d14250fb3ed06d6421c6b2e04ae266b436138213eea2fe4ddc3640df8064d9bc) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne 'd14250fb3ed06d6421c6b2e04ae266b436138213eea2fe4ddc3640df8064d9bc') {             Write-Host 'FAILED!';             exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome' -Wait -Passthru;     Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:406ffb8432a757e84f7594e85c676620dec6955e0475ac271aa4dd5c0531190d`  
		Size: 655.8 MB (655757265 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5e61fff845eda39f31bdf5d797254fdf656ee79d8c294c1713007864bc4c2535`  
		Last Modified: Wed, 14 Oct 2020 12:50:32 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14b6dd39a83ed26a547d74d22f7b9c4578c03229e9c114023e02de836b3d8b95`  
		Last Modified: Sat, 17 Oct 2020 02:10:02 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:636ec7c93ecd0fc88e26e6f545a6e55975f771b2fe3a22ca11a9963cdb352f12`  
		Last Modified: Sat, 17 Oct 2020 02:12:22 GMT  
		Size: 100.4 MB (100393386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adoptopenjdk:15_36-jre-hotspot` - windows version 10.0.14393.3986; amd64

```console
$ docker pull adoptopenjdk@sha256:88d0bcc11cb31897cdce5c2d24f8450090d0b3fa910aea721be77d7bd7265509
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5842374377 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e701a32be792ae63c3e0f947f39da6445f9b45bd15770c0f52b45b3e1e53a2d`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Fri, 02 Oct 2020 17:07:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 14 Oct 2020 12:31:45 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Sat, 17 Oct 2020 01:07:26 GMT
ENV JAVA_VERSION=jdk-15+36
# Sat, 17 Oct 2020 01:14:41 GMT
RUN Write-Host ('Downloading https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15%2B36/OpenJDK15U-jre_x64_windows_hotspot_15_36.msi ...');     [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     wget https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15%2B36/OpenJDK15U-jre_x64_windows_hotspot_15_36.msi -O 'openjdk.msi';     Write-Host ('Verifying sha256 (d14250fb3ed06d6421c6b2e04ae266b436138213eea2fe4ddc3640df8064d9bc) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne 'd14250fb3ed06d6421c6b2e04ae266b436138213eea2fe4ddc3640df8064d9bc') {             Write-Host 'FAILED!';             exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome' -Wait -Passthru;     Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:17a32268498b2feefa5457f0423ac15473596d514e48c694ef54d740a9a5067d`  
		Size: 1.7 GB (1671365753 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e300a13db0fbbf48a676ace9db3b0de292c825dfa01e6d82979d96ebc23d3675`  
		Last Modified: Wed, 14 Oct 2020 12:51:34 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85d9ebae6a3c407b87dcad974e7425d2e65f43587d3b21c2ab9129e020030dcf`  
		Last Modified: Sat, 17 Oct 2020 02:11:15 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0161ded81e6014c55948f1b717229dfb2673219dda672ff3b5690a8571599e6`  
		Last Modified: Sat, 17 Oct 2020 02:12:57 GMT  
		Size: 101.0 MB (101020441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
