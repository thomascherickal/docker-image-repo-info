## `adoptopenjdk:15_36-jdk-hotspot-bionic`

```console
$ docker pull adoptopenjdk@sha256:c0647c2da1272d55140a6a0f53ca52c12340cb006fb2a5c9cedcfaf1e76f71c6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; s390x

### `adoptopenjdk:15_36-jdk-hotspot-bionic` - linux; amd64

```console
$ docker pull adoptopenjdk@sha256:271c80808bec975bcdac0f62bcbe6c8332a060bf648a483009aa0d81f33fbe83
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **248.3 MB (248297431 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f8203f79caac1ca27a235648e1bb7cb68d9db0a84194d9c646cd57f33f3d97e4`
-	Default Command: `["jshell"]`

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
# Tue, 20 Oct 2020 17:04:29 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='44c8cd580f6e828f8fbb431a59b3c8f694da8c75adb7c311f7b6b9ed81c19c54';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15%2B36/OpenJDK15U-jdk_aarch64_linux_hotspot_15_36.tar.gz';          ;;        armhf|armv7l)          ESUM='d7de37fee91fe098791d48ea2a880cf2789949665d6bc9a232380738f99c16a9';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15%2B36/OpenJDK15U-jdk_arm_linux_hotspot_15_36.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='537eb289a0fc56915078ff92616574b00b8ad0119543f5e4a817ede0e52c4030';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15%2B36/OpenJDK15U-jdk_ppc64le_linux_hotspot_15_36.tar.gz';          ;;        s390x)          ESUM='3e238ea4924f4dd2a8167c911a99b96ffdfb51e12f3969cffbdc0791a58d0cf2';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15%2B36/OpenJDK15U-jdk_s390x_linux_hotspot_15_36.tar.gz';          ;;        amd64|x86_64)          ESUM='c198593d1b5188ee3570e2ca33c3bc004aaefbda2c11e68e58ae7296cf5c3982';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15%2B36/OpenJDK15U-jdk_x64_linux_hotspot_15_36.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 20 Oct 2020 17:04:29 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 20 Oct 2020 17:04:29 GMT
CMD ["jshell"]
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
	-	`sha256:d4f522eb0363ddb6adedf7608260a017819ad882ddbf888b21f19d269b429687`  
		Last Modified: Tue, 20 Oct 2020 17:21:06 GMT  
		Size: 207.7 MB (207719159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adoptopenjdk:15_36-jdk-hotspot-bionic` - linux; arm variant v7

```console
$ docker pull adoptopenjdk@sha256:8cd7fb8c48d6ab9203228af6b2b8f0f1acf2c4140e1e1562f3fb968d12a43f0f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **226.4 MB (226370360 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c825a168cead38f21cce38980b9fbdbbd96ef42840ee61c53b0075bb320959b`
-	Default Command: `["jshell"]`

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
# Tue, 20 Oct 2020 17:02:00 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='44c8cd580f6e828f8fbb431a59b3c8f694da8c75adb7c311f7b6b9ed81c19c54';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15%2B36/OpenJDK15U-jdk_aarch64_linux_hotspot_15_36.tar.gz';          ;;        armhf|armv7l)          ESUM='d7de37fee91fe098791d48ea2a880cf2789949665d6bc9a232380738f99c16a9';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15%2B36/OpenJDK15U-jdk_arm_linux_hotspot_15_36.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='537eb289a0fc56915078ff92616574b00b8ad0119543f5e4a817ede0e52c4030';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15%2B36/OpenJDK15U-jdk_ppc64le_linux_hotspot_15_36.tar.gz';          ;;        s390x)          ESUM='3e238ea4924f4dd2a8167c911a99b96ffdfb51e12f3969cffbdc0791a58d0cf2';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15%2B36/OpenJDK15U-jdk_s390x_linux_hotspot_15_36.tar.gz';          ;;        amd64|x86_64)          ESUM='c198593d1b5188ee3570e2ca33c3bc004aaefbda2c11e68e58ae7296cf5c3982';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15%2B36/OpenJDK15U-jdk_x64_linux_hotspot_15_36.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 20 Oct 2020 17:02:03 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 20 Oct 2020 17:02:04 GMT
CMD ["jshell"]
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
	-	`sha256:41f8fb78844beb8674f91d3bdfef79d319263f4b8330cd228d322c8c0bc985bf`  
		Last Modified: Tue, 20 Oct 2020 17:05:00 GMT  
		Size: 191.3 MB (191272632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adoptopenjdk:15_36-jdk-hotspot-bionic` - linux; arm64 variant v8

```console
$ docker pull adoptopenjdk@sha256:82945b251c6bd3665b873612905b663fcb3c344912fe081919e1c2c95e5416b5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **242.3 MB (242298993 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c9be860d6aba0de4b3d100f8e5dce0466fdc034c8c58f5610d734e2329b2fb75`
-	Default Command: `["jshell"]`

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
# Tue, 20 Oct 2020 16:41:01 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='44c8cd580f6e828f8fbb431a59b3c8f694da8c75adb7c311f7b6b9ed81c19c54';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15%2B36/OpenJDK15U-jdk_aarch64_linux_hotspot_15_36.tar.gz';          ;;        armhf|armv7l)          ESUM='d7de37fee91fe098791d48ea2a880cf2789949665d6bc9a232380738f99c16a9';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15%2B36/OpenJDK15U-jdk_arm_linux_hotspot_15_36.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='537eb289a0fc56915078ff92616574b00b8ad0119543f5e4a817ede0e52c4030';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15%2B36/OpenJDK15U-jdk_ppc64le_linux_hotspot_15_36.tar.gz';          ;;        s390x)          ESUM='3e238ea4924f4dd2a8167c911a99b96ffdfb51e12f3969cffbdc0791a58d0cf2';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15%2B36/OpenJDK15U-jdk_s390x_linux_hotspot_15_36.tar.gz';          ;;        amd64|x86_64)          ESUM='c198593d1b5188ee3570e2ca33c3bc004aaefbda2c11e68e58ae7296cf5c3982';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15%2B36/OpenJDK15U-jdk_x64_linux_hotspot_15_36.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 20 Oct 2020 16:41:02 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 20 Oct 2020 16:41:03 GMT
CMD ["jshell"]
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
	-	`sha256:a029b119a873449d46bf2354022f7cd6fc7bac9401787a530d8e0a49faaafbf8`  
		Last Modified: Tue, 20 Oct 2020 16:47:50 GMT  
		Size: 205.3 MB (205290232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adoptopenjdk:15_36-jdk-hotspot-bionic` - linux; s390x

```console
$ docker pull adoptopenjdk@sha256:4835578b755b12984b9eb4e12ac7968f59a17b636c4facfe1f5ac19fa95b3243
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **220.3 MB (220348506 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e9c1cc3bcf33118032c1fa84a06f8d1a7912c3813757261edd12ec2f6ffa18e`
-	Default Command: `["jshell"]`

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
# Tue, 20 Oct 2020 16:42:26 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='44c8cd580f6e828f8fbb431a59b3c8f694da8c75adb7c311f7b6b9ed81c19c54';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15%2B36/OpenJDK15U-jdk_aarch64_linux_hotspot_15_36.tar.gz';          ;;        armhf|armv7l)          ESUM='d7de37fee91fe098791d48ea2a880cf2789949665d6bc9a232380738f99c16a9';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15%2B36/OpenJDK15U-jdk_arm_linux_hotspot_15_36.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='537eb289a0fc56915078ff92616574b00b8ad0119543f5e4a817ede0e52c4030';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15%2B36/OpenJDK15U-jdk_ppc64le_linux_hotspot_15_36.tar.gz';          ;;        s390x)          ESUM='3e238ea4924f4dd2a8167c911a99b96ffdfb51e12f3969cffbdc0791a58d0cf2';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15%2B36/OpenJDK15U-jdk_s390x_linux_hotspot_15_36.tar.gz';          ;;        amd64|x86_64)          ESUM='c198593d1b5188ee3570e2ca33c3bc004aaefbda2c11e68e58ae7296cf5c3982';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15%2B36/OpenJDK15U-jdk_x64_linux_hotspot_15_36.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 20 Oct 2020 16:42:31 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 20 Oct 2020 16:42:31 GMT
CMD ["jshell"]
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
	-	`sha256:71917e95758aba96d7af44bada1286de41dd9f20857e0646ff777120b9b606c8`  
		Last Modified: Tue, 20 Oct 2020 16:58:20 GMT  
		Size: 181.4 MB (181379769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
