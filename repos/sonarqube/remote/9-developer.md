## `sonarqube:9-developer`

```console
$ docker pull sonarqube@sha256:5b9d53eec8fbf366977ef704ed1337a2333b9ffcb14f31b16d4a39f38d7e80ca
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `sonarqube:9-developer` - linux; amd64

```console
$ docker pull sonarqube@sha256:202d8ee45abb82913f2d52d40de004467b3c7c308dc413c9210d14ccc484768b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **420.3 MB (420338469 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ecd8f7609cae835b2748a99cabc458a448d9e4426e428854071f729b5cba9ef`
-	Entrypoint: `["bin\/run.sh"]`
-	Default Command: `["bin\/sonar.sh"]`

```dockerfile
# Fri, 06 Aug 2021 17:19:45 GMT
ADD file:34eb5c40aa00028921a224d1764ae1b1f3ef710d191e4dfc7df55e0594aa7217 in / 
# Fri, 06 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 06 Aug 2021 21:00:05 GMT
ENV JAVA_VERSION=jdk-11.0.11+9 LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 06 Aug 2021 21:00:19 GMT
RUN set -eux;     apk add --no-cache tzdata --virtual .build-deps curl binutils zstd;     GLIBC_VER="2.33-r0";     ALPINE_GLIBC_REPO="https://github.com/sgerrand/alpine-pkg-glibc/releases/download";     GCC_LIBS_URL="https://archive.archlinux.org/packages/g/gcc-libs/gcc-libs-10.2.0-6-x86_64.pkg.tar.zst";     GCC_LIBS_SHA256="e33b45e4a10ef26259d6acf8e7b5dd6dc63800641e41eb67fa6588d061f79c1c";     ZLIB_URL="https://archive.archlinux.org/packages/z/zlib/zlib-1%3A1.2.11-4-x86_64.pkg.tar.xz";     ZLIB_SHA256=43a17987d348e0b395cb6e28d2ece65fb3b5a0fe433714762780d18c0451c149;     curl -LfsS https://alpine-pkgs.sgerrand.com/sgerrand.rsa.pub -o /etc/apk/keys/sgerrand.rsa.pub;     SGERRAND_RSA_SHA256="823b54589c93b02497f1ba4dc622eaef9c813e6b0f0ebbb2f771e32adf9f4ef2";     echo "${SGERRAND_RSA_SHA256} */etc/apk/keys/sgerrand.rsa.pub" | sha256sum -c - ;     curl -LfsS ${ALPINE_GLIBC_REPO}/${GLIBC_VER}/glibc-${GLIBC_VER}.apk > /tmp/glibc-${GLIBC_VER}.apk;     apk add --no-cache /tmp/glibc-${GLIBC_VER}.apk;     curl -LfsS ${ALPINE_GLIBC_REPO}/${GLIBC_VER}/glibc-bin-${GLIBC_VER}.apk > /tmp/glibc-bin-${GLIBC_VER}.apk;     apk add --no-cache /tmp/glibc-bin-${GLIBC_VER}.apk;     curl -Ls ${ALPINE_GLIBC_REPO}/${GLIBC_VER}/glibc-i18n-${GLIBC_VER}.apk > /tmp/glibc-i18n-${GLIBC_VER}.apk;     apk add --no-cache /tmp/glibc-i18n-${GLIBC_VER}.apk;     /usr/glibc-compat/bin/localedef --inputfile en_US --charmap UTF-8 "$LANG" || true ;    echo "export LANG=$LANG" > /etc/profile.d/locale.sh;     curl -LfsS ${GCC_LIBS_URL} -o /tmp/gcc-libs.tar.zst;     echo "${GCC_LIBS_SHA256} */tmp/gcc-libs.tar.zst" | sha256sum -c - ;     mkdir /tmp/gcc;     zstd -d /tmp/gcc-libs.tar.zst --output-dir-flat /tmp;     tar -xf /tmp/gcc-libs.tar -C /tmp/gcc;     mv /tmp/gcc/usr/lib/libgcc* /tmp/gcc/usr/lib/libstdc++* /usr/glibc-compat/lib;     strip /usr/glibc-compat/lib/libgcc_s.so.* /usr/glibc-compat/lib/libstdc++.so*;     curl -LfsS ${ZLIB_URL} -o /tmp/libz.tar.xz;     echo "${ZLIB_SHA256} */tmp/libz.tar.xz" | sha256sum -c - ;    mkdir /tmp/libz;     tar -xf /tmp/libz.tar.xz -C /tmp/libz;     mv /tmp/libz/usr/lib/libz.so* /usr/glibc-compat/lib;     apk del --purge .build-deps glibc-i18n;     rm -rf /tmp/*.apk /tmp/gcc /tmp/gcc-libs.tar* /tmp/libz /tmp/libz.tar.xz /var/cache/apk/*;
# Fri, 06 Aug 2021 21:00:24 GMT
RUN set -eux;     apk add --no-cache --virtual .fetch-deps curl;     ARCH="$(apk --print-arch)";     case "${ARCH}" in        aarch64|arm64)          ESUM='fde6b29df23b6e7ed6e16a237a0f44273fb9e267fdfbd0b3de5add98e55649f6';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.11%2B9/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.11_9.tar.gz';          ;;        armhf|armv7l)          ESUM='ad02656f800fd64c2b090b23ad24a099d9cd1054948ecb0e9851bc39c51c8be8';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.11%2B9/OpenJDK11U-jre_arm_linux_hotspot_11.0.11_9.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='37c19c7c2d1cea627b854a475ef1a765d30357d765d20cf3f96590037e79d0f3';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.11%2B9/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.11_9.tar.gz';          ;;        s390x)          ESUM='f18101fc50aad795a41b4d3bbc591308c83664fd2390bf2bc007fd9b3d531e6c';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.11%2B9/OpenJDK11U-jre_s390x_linux_hotspot_11.0.11_9.tar.gz';          ;;        amd64|x86_64)          ESUM='144f2c6bcf64faa32016f2474b6c01031be75d25325e9c3097aed6589bc5d548';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.11%2B9/OpenJDK11U-jre_x64_linux_hotspot_11.0.11_9.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     apk del --purge .fetch-deps;     rm -rf /var/cache/apk/*;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 06 Aug 2021 21:00:24 GMT
ARG SONARQUBE_VERSION=9.0.1.46107
# Fri, 06 Aug 2021 21:01:16 GMT
ARG SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/CommercialDistribution/sonarqube-developer/sonarqube-developer-9.0.1.46107.zip
# Fri, 06 Aug 2021 21:01:17 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SONARQUBE_HOME=/opt/sonarqube SONAR_VERSION=9.0.1.46107 SQ_DATA_DIR=/opt/sonarqube/data SQ_EXTENSIONS_DIR=/opt/sonarqube/extensions SQ_LOGS_DIR=/opt/sonarqube/logs SQ_TEMP_DIR=/opt/sonarqube/temp
# Fri, 06 Aug 2021 21:02:16 GMT
# ARGS: SONARQUBE_VERSION=9.0.1.46107 SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/CommercialDistribution/sonarqube-developer/sonarqube-developer-9.0.1.46107.zip
RUN set -eux;     addgroup -S -g 1000 sonarqube;     adduser -S -D -u 1000 -G sonarqube sonarqube;     apk add --no-cache --virtual build-dependencies gnupg unzip curl;     apk add --no-cache bash su-exec ttf-dejavu;     echo "networkaddress.cache.ttl=5" >> "${JAVA_HOME}/conf/security/java.security";     sed --in-place --expression="s?securerandom.source=file:/dev/random?securerandom.source=file:/dev/urandom?g" "${JAVA_HOME}/conf/security/java.security";     for server in $(shuf -e ha.pool.sks-keyservers.net                             hkp://p80.pool.sks-keyservers.net:80                             keyserver.ubuntu.com                             hkp://keyserver.ubuntu.com:80                             pgp.mit.edu) ; do         gpg --batch --keyserver "${server}" --recv-keys 679F1EE92B19609DE816FDE81DB198F93525EC1A && break || : ;     done;     mkdir --parents /opt;     cd /opt;     curl --fail --location --output sonarqube.zip --silent --show-error "${SONARQUBE_ZIP_URL}";     curl --fail --location --output sonarqube.zip.asc --silent --show-error "${SONARQUBE_ZIP_URL}.asc";     gpg --batch --verify sonarqube.zip.asc sonarqube.zip;     unzip -q sonarqube.zip;     mv "sonarqube-${SONARQUBE_VERSION}" sonarqube;     rm sonarqube.zip*;     rm -rf ${SONARQUBE_HOME}/bin/*;     chown -R sonarqube:sonarqube ${SONARQUBE_HOME} ;     chmod -R 777 "${SQ_DATA_DIR}" "${SQ_EXTENSIONS_DIR}" "${SQ_LOGS_DIR}" "${SQ_TEMP_DIR}" ;     apk del --purge build-dependencies;
# Fri, 06 Aug 2021 21:02:18 GMT
COPY --chown=sonarqube:sonarqubemulti:aed345498324cc768d63aba16bd3b3de027a0213cb3a62a9a3b27799dbf88552 in /opt/sonarqube/bin/ 
# Fri, 06 Aug 2021 21:02:18 GMT
WORKDIR /opt/sonarqube
# Fri, 06 Aug 2021 21:02:18 GMT
EXPOSE 9000
# Fri, 06 Aug 2021 21:02:19 GMT
ENTRYPOINT ["bin/run.sh"]
# Fri, 06 Aug 2021 21:02:19 GMT
CMD ["bin/sonar.sh"]
```

-	Layers:
	-	`sha256:29291e31a76a7e560b9b7ad3cada56e8c18d50a96cca8a2573e4f4689d7aca77`  
		Last Modified: Thu, 05 Aug 2021 15:56:25 GMT  
		Size: 2.8 MB (2813006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b090d1ada32d1d8704f038381d4ef66083a366545066110d8ec0e8b69e2e95e`  
		Last Modified: Fri, 06 Aug 2021 21:07:04 GMT  
		Size: 7.3 MB (7348223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:346893427c7107fca36fd0640a68b2bc7b1e5a1e053d42eba0e97c80fd39a987`  
		Last Modified: Fri, 06 Aug 2021 21:07:10 GMT  
		Size: 43.3 MB (43299129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dc9cfbec58f5fbd551b30a04b3d85114b1816b2a3e9168060d82b24c52462ff`  
		Last Modified: Fri, 06 Aug 2021 21:07:59 GMT  
		Size: 366.9 MB (366877011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6cb5b8975acabfb9985850eccabe5fc7fd71e57860b0789ff40658c8af94053`  
		Last Modified: Fri, 06 Aug 2021 21:07:40 GMT  
		Size: 1.1 KB (1100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
