## `sonarqube:datacenter-app`

```console
$ docker pull sonarqube@sha256:85d10e61435d16cab308c210a3a7b198734b0c65ee8453d00ec9263c282ad73d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `sonarqube:datacenter-app` - linux; amd64

```console
$ docker pull sonarqube@sha256:17c2bd6cb99bb18daa028dc81f0cfa0f3503574304bcbc98d413588acddd2a90
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **509.5 MB (509528207 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c5f11a9f4c82fceea5fd008ff6077ab489e3da27809ed234d40684b8cda1233`
-	Entrypoint: `["\/opt\/sonarqube\/bin\/run.sh"]`
-	Default Command: `["\/opt\/sonarqube\/bin\/sonar.sh"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:44 GMT
ADD file:762c899ec0505d1a32930ee804c5b008825f41611161be104076cba33b7e5b2b in / 
# Fri, 12 Nov 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 22:10:12 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Mon, 29 Nov 2021 21:30:44 GMT
ARG SONARQUBE_VERSION=9.2.1.49989
# Mon, 29 Nov 2021 23:41:41 GMT
ARG SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/CommercialDistribution/sonarqube-datacenter/sonarqube-datacenter-9.2.1.49989.zip
# Mon, 29 Nov 2021 23:41:41 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-11-openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SONARQUBE_HOME=/opt/sonarqube SONAR_VERSION=9.2.1.49989 SQ_DATA_DIR=/opt/sonarqube/data SQ_EXTENSIONS_DIR=/opt/sonarqube/extensions SQ_LOGS_DIR=/opt/sonarqube/logs SQ_TEMP_DIR=/opt/sonarqube/temp SONAR_CLUSTER_NODE_TYPE=application SONAR_CLUSTER_ENABLED=true
# Mon, 29 Nov 2021 23:46:44 GMT
# ARGS: SONARQUBE_VERSION=9.2.1.49989 SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/CommercialDistribution/sonarqube-datacenter/sonarqube-datacenter-9.2.1.49989.zip
RUN set -eux;     addgroup -S -g 1000 sonarqube;     adduser -S -D -u 1000 -G sonarqube sonarqube;     apk add --no-cache --virtual build-dependencies gnupg unzip curl;     apk add --no-cache bash su-exec ttf-dejavu openjdk11-jre;     echo "networkaddress.cache.ttl=5" >> "${JAVA_HOME}/conf/security/java.security";     sed --in-place --expression="s?securerandom.source=file:/dev/random?securerandom.source=file:/dev/urandom?g" "${JAVA_HOME}/conf/security/java.security";     for server in $(shuf -e ha.pool.sks-keyservers.net                             hkp://p80.pool.sks-keyservers.net:80                             keyserver.ubuntu.com                             hkp://keyserver.ubuntu.com:80                             pgp.mit.edu) ; do         gpg --batch --keyserver "${server}" --recv-keys 679F1EE92B19609DE816FDE81DB198F93525EC1A && break || : ;     done;     mkdir --parents /opt ;    cd /opt;     curl --fail --location --output sonarqube.zip --silent --show-error "${SONARQUBE_ZIP_URL}";     curl --fail --location --output sonarqube.zip.asc --silent --show-error "${SONARQUBE_ZIP_URL}.asc";     gpg --batch --verify sonarqube.zip.asc sonarqube.zip;     unzip -q sonarqube.zip;     mv "sonarqube-${SONARQUBE_VERSION}" sonarqube;     rm sonarqube.zip*;     rm -rf ${SONARQUBE_HOME}/bin/*;     chown -R sonarqube:sonarqube ${SONARQUBE_HOME} ;     chmod -R 777 "${SQ_DATA_DIR}" "${SQ_EXTENSIONS_DIR}" "${SQ_LOGS_DIR}" "${SQ_TEMP_DIR}" ;     apk del --purge build-dependencies;
# Mon, 29 Nov 2021 23:46:46 GMT
COPY --chown=sonarqube:sonarqubemulti:b3583528dc7e1c8c3d5b50dfbb55820aeec61ed9bbc812d0d58f5c5875189ea8 in /opt/sonarqube/bin/ 
# Mon, 29 Nov 2021 23:46:46 GMT
WORKDIR /opt/sonarqube
# Mon, 29 Nov 2021 23:46:47 GMT
EXPOSE 9000
# Mon, 29 Nov 2021 23:46:47 GMT
STOPSIGNAL SIGINT
# Mon, 29 Nov 2021 23:46:47 GMT
ENTRYPOINT ["/opt/sonarqube/bin/run.sh"]
# Mon, 29 Nov 2021 23:46:47 GMT
CMD ["/opt/sonarqube/bin/sonar.sh"]
```

-	Layers:
	-	`sha256:97518928ae5f3d52d4164b314a7e73654eb686ecd8aafa0b79acd980773a740d`  
		Last Modified: Fri, 12 Nov 2021 17:20:39 GMT  
		Size: 2.8 MB (2822981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c8f47c095183df09f6fde61fdce7d880798031be38d243c1f363d0903c90dbd`  
		Last Modified: Tue, 30 Nov 2021 00:53:47 GMT  
		Size: 506.7 MB (506703705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bd98b3480c9bdf15e87acaa24c89cd621fda767cde492bc806e46b03db5dbeb`  
		Last Modified: Tue, 30 Nov 2021 00:53:18 GMT  
		Size: 1.5 KB (1521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
