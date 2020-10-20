## `adoptopenjdk:8-jdk-hotspot-bionic`

```console
$ docker pull adoptopenjdk@sha256:cf64763f2d104cc33f95eba72c4710ebff08ac0c4badbef72bc9bc0b18660d6e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `adoptopenjdk:8-jdk-hotspot-bionic` - linux; amd64

```console
$ docker pull adoptopenjdk@sha256:5724a7f635ad4e1c0bde19fde3125a20c55994fa4a10f1134ec633f6027fb5de
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **144.3 MB (144279654 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0e8d5a185cdc289088add05904525948fdc33c628941ae7910f8fe51e1a4cde`
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
# Tue, 20 Oct 2020 17:03:29 GMT
ENV JAVA_VERSION=jdk8u265-b01
# Tue, 20 Oct 2020 17:03:37 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='87d16dac293d2a9abbb559a277bfaded702f28d1bfdc526f8613bb9cfed84a12';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u265-b01/OpenJDK8U-jdk_aarch64_linux_hotspot_8u265b01.tar.gz';          ;;        armhf|armv7l)          ESUM='dc3405aab81f422b7721f665c76371bd7b03c291eea89cd110a82d8bcf07809a';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u265-b01/OpenJDK8U-jdk_arm_linux_hotspot_8u265b01.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='7bbb9d76458ee29bc5e2458b32a91b8c032ecffe6cb8500734ca41d2d8f5c9f3';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u265-b01/OpenJDK8U-jdk_ppc64le_linux_hotspot_8u265b01.tar.gz';          ;;        s390x)          ESUM='aca50f02d59169cb428d54501846b518edc9fff6a6f428459c72b4faa2b4abb0';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u265-b01/OpenJDK8U-jdk_s390x_linux_hotspot_8u265b01.tar.gz';          ;;        amd64|x86_64)          ESUM='1285da6278f2d38a790a21148d7e683f20de0799c44b937043830ef6b57f58c4';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u265-b01/OpenJDK8U-jdk_x64_linux_hotspot_8u265b01.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 20 Oct 2020 17:03:37 GMT
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
	-	`sha256:a63377c6269c8f4a292ba54e080dc65c728dd6aee8ee4c2133c06dfccf5edda9`  
		Last Modified: Tue, 20 Oct 2020 17:20:09 GMT  
		Size: 103.7 MB (103701382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adoptopenjdk:8-jdk-hotspot-bionic` - linux; arm variant v7

```console
$ docker pull adoptopenjdk@sha256:cba374b70f56dc636292189605ce7c866901a48b1d5ed9ea9cbcea8f64c47a1d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.3 MB (133277057 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6036e24a50e32ecb376b00b31662be9776969826075815be9b197167886f7bd0`
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
# Tue, 20 Oct 2020 17:00:24 GMT
ENV JAVA_VERSION=jdk8u265-b01
# Tue, 20 Oct 2020 17:00:38 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='87d16dac293d2a9abbb559a277bfaded702f28d1bfdc526f8613bb9cfed84a12';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u265-b01/OpenJDK8U-jdk_aarch64_linux_hotspot_8u265b01.tar.gz';          ;;        armhf|armv7l)          ESUM='dc3405aab81f422b7721f665c76371bd7b03c291eea89cd110a82d8bcf07809a';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u265-b01/OpenJDK8U-jdk_arm_linux_hotspot_8u265b01.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='7bbb9d76458ee29bc5e2458b32a91b8c032ecffe6cb8500734ca41d2d8f5c9f3';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u265-b01/OpenJDK8U-jdk_ppc64le_linux_hotspot_8u265b01.tar.gz';          ;;        s390x)          ESUM='aca50f02d59169cb428d54501846b518edc9fff6a6f428459c72b4faa2b4abb0';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u265-b01/OpenJDK8U-jdk_s390x_linux_hotspot_8u265b01.tar.gz';          ;;        amd64|x86_64)          ESUM='1285da6278f2d38a790a21148d7e683f20de0799c44b937043830ef6b57f58c4';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u265-b01/OpenJDK8U-jdk_x64_linux_hotspot_8u265b01.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 20 Oct 2020 17:00:43 GMT
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
	-	`sha256:b98cd0e06d4aa392d4642f2ac01a346abecad7b77a0d7f57f0e619dfbe5599d3`  
		Last Modified: Tue, 20 Oct 2020 17:03:25 GMT  
		Size: 98.2 MB (98179329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adoptopenjdk:8-jdk-hotspot-bionic` - linux; arm64 variant v8

```console
$ docker pull adoptopenjdk@sha256:369dffe2b9dfda9a6921c01cfaa597182b68dd7009cc315f534709e3d1214189
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **140.9 MB (140851112 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8105c4702c2de15459cac0bd7857371f4c9e9d620245d19ef58cb090a453a8b0`
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
# Tue, 20 Oct 2020 16:39:39 GMT
ENV JAVA_VERSION=jdk8u265-b01
# Tue, 20 Oct 2020 16:39:47 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='87d16dac293d2a9abbb559a277bfaded702f28d1bfdc526f8613bb9cfed84a12';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u265-b01/OpenJDK8U-jdk_aarch64_linux_hotspot_8u265b01.tar.gz';          ;;        armhf|armv7l)          ESUM='dc3405aab81f422b7721f665c76371bd7b03c291eea89cd110a82d8bcf07809a';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u265-b01/OpenJDK8U-jdk_arm_linux_hotspot_8u265b01.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='7bbb9d76458ee29bc5e2458b32a91b8c032ecffe6cb8500734ca41d2d8f5c9f3';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u265-b01/OpenJDK8U-jdk_ppc64le_linux_hotspot_8u265b01.tar.gz';          ;;        s390x)          ESUM='aca50f02d59169cb428d54501846b518edc9fff6a6f428459c72b4faa2b4abb0';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u265-b01/OpenJDK8U-jdk_s390x_linux_hotspot_8u265b01.tar.gz';          ;;        amd64|x86_64)          ESUM='1285da6278f2d38a790a21148d7e683f20de0799c44b937043830ef6b57f58c4';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u265-b01/OpenJDK8U-jdk_x64_linux_hotspot_8u265b01.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 20 Oct 2020 16:39:49 GMT
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
	-	`sha256:73bfd889f6ffd99fe97ee773c01238b1b25cfb538dced26beefe4018a008fea4`  
		Last Modified: Tue, 20 Oct 2020 16:46:19 GMT  
		Size: 103.8 MB (103842351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adoptopenjdk:8-jdk-hotspot-bionic` - linux; ppc64le

```console
$ docker pull adoptopenjdk@sha256:f00d9fe9dd878fdbec5db34e631e90d71e0ab8ac8f1125372e7fae26bc5ad68d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **151.4 MB (151360158 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b8a1d9745532a74db42c6ed7fa480742a10a03d5595bd2f33a0cf6e7580f84b8`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 25 Sep 2020 23:53:28 GMT
ADD file:5479628763eb7f8cd884270bc1e9bb40ce39f1fb3427e863b086511696fa8107 in / 
# Fri, 25 Sep 2020 23:53:48 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 25 Sep 2020 23:54:03 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 25 Sep 2020 23:54:24 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 25 Sep 2020 23:54:31 GMT
CMD ["/bin/bash"]
# Sat, 17 Oct 2020 21:53:08 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Sat, 17 Oct 2020 21:55:52 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Sat, 17 Oct 2020 21:56:02 GMT
ENV JAVA_VERSION=jdk8u265-b01
# Sun, 18 Oct 2020 10:17:34 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='87d16dac293d2a9abbb559a277bfaded702f28d1bfdc526f8613bb9cfed84a12';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u265-b01/OpenJDK8U-jdk_aarch64_linux_hotspot_8u265b01.tar.gz';          ;;        armhf|armv7l)          ESUM='dc3405aab81f422b7721f665c76371bd7b03c291eea89cd110a82d8bcf07809a';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u265-b01/OpenJDK8U-jdk_arm_linux_hotspot_8u265b01.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='7bbb9d76458ee29bc5e2458b32a91b8c032ecffe6cb8500734ca41d2d8f5c9f3';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u265-b01/OpenJDK8U-jdk_ppc64le_linux_hotspot_8u265b01.tar.gz';          ;;        s390x)          ESUM='aca50f02d59169cb428d54501846b518edc9fff6a6f428459c72b4faa2b4abb0';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u265-b01/OpenJDK8U-jdk_s390x_linux_hotspot_8u265b01.tar.gz';          ;;        amd64|x86_64)          ESUM='1285da6278f2d38a790a21148d7e683f20de0799c44b937043830ef6b57f58c4';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u265-b01/OpenJDK8U-jdk_x64_linux_hotspot_8u265b01.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Sun, 18 Oct 2020 10:17:47 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
```

-	Layers:
	-	`sha256:af5e190551614a549619ca2cb11a237bf566e7b0942eac80adaf05e21644ad12`  
		Last Modified: Sat, 26 Sep 2020 00:06:58 GMT  
		Size: 33.3 MB (33278058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9dd7d43fa9f545a3f69e66ff00d1a2773213cdfc18d0c99a71bb1c40bbb1f8c`  
		Last Modified: Sat, 26 Sep 2020 00:06:13 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1feb93b9aa176877a7ec845345f281fe28c37605e03363dd0fa489bf0bf10ee`  
		Last Modified: Sat, 26 Sep 2020 00:06:13 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:552ff917e16f44b016f2a729c4f39d038bb390da36dbe4f02681940c113b6530`  
		Last Modified: Sat, 17 Oct 2020 22:27:52 GMT  
		Size: 17.2 MB (17189876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b824efe7a8c1961398d14ae2727bc5c61101a60293bf72873546464d67f44ec7`  
		Last Modified: Sun, 18 Oct 2020 10:38:26 GMT  
		Size: 100.9 MB (100891186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adoptopenjdk:8-jdk-hotspot-bionic` - linux; s390x

```console
$ docker pull adoptopenjdk@sha256:7055ac9961970b84f957d98ec7b188c7acb45405d7d78151864228279d6cd243
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.7 MB (137724762 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3651d1a1778f01313bf9a010a7bf2914a06dca16346ff4ba9ea7b36c77a99ca2`
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
# Tue, 20 Oct 2020 16:41:24 GMT
ENV JAVA_VERSION=jdk8u265-b01
# Tue, 20 Oct 2020 16:41:31 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='87d16dac293d2a9abbb559a277bfaded702f28d1bfdc526f8613bb9cfed84a12';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u265-b01/OpenJDK8U-jdk_aarch64_linux_hotspot_8u265b01.tar.gz';          ;;        armhf|armv7l)          ESUM='dc3405aab81f422b7721f665c76371bd7b03c291eea89cd110a82d8bcf07809a';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u265-b01/OpenJDK8U-jdk_arm_linux_hotspot_8u265b01.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='7bbb9d76458ee29bc5e2458b32a91b8c032ecffe6cb8500734ca41d2d8f5c9f3';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u265-b01/OpenJDK8U-jdk_ppc64le_linux_hotspot_8u265b01.tar.gz';          ;;        s390x)          ESUM='aca50f02d59169cb428d54501846b518edc9fff6a6f428459c72b4faa2b4abb0';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u265-b01/OpenJDK8U-jdk_s390x_linux_hotspot_8u265b01.tar.gz';          ;;        amd64|x86_64)          ESUM='1285da6278f2d38a790a21148d7e683f20de0799c44b937043830ef6b57f58c4';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u265-b01/OpenJDK8U-jdk_x64_linux_hotspot_8u265b01.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 20 Oct 2020 16:41:33 GMT
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
	-	`sha256:32503c54505c22490a2d0d5e7616868d41990951d61ba6958d67d9fbf4dae391`  
		Last Modified: Tue, 20 Oct 2020 16:57:18 GMT  
		Size: 98.8 MB (98756025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
