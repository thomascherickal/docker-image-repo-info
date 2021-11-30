## `sonarqube:9-datacenter-search`

```console
$ docker pull sonarqube@sha256:5ca377b85584951ab3719d20269bfc76e1ce1809b9461a2efa5548de16687258
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `sonarqube:9-datacenter-search` - linux; amd64

```console
$ docker pull sonarqube@sha256:d996fec2d96f32bcb037688497c37c6bc9a2ba9293f568b3554a6bb6a36d8e06
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **509.5 MB (509528034 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a8e0a867ae3e3ce6f7dac63c253b4dff7daf8d1829178218795f321edfbf151a`
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
# Mon, 29 Nov 2021 23:47:04 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-11-openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SONARQUBE_HOME=/opt/sonarqube SONAR_VERSION=9.2.1.49989 SQ_DATA_DIR=/opt/sonarqube/data SQ_EXTENSIONS_DIR=/opt/sonarqube/extensions SQ_LOGS_DIR=/opt/sonarqube/logs SQ_TEMP_DIR=/opt/sonarqube/temp SONAR_CLUSTER_NODE_TYPE=search SONAR_CLUSTER_ENABLED=true
# Tue, 30 Nov 2021 00:50:04 GMT
# ARGS: SONARQUBE_VERSION=9.2.1.49989 SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/CommercialDistribution/sonarqube-datacenter/sonarqube-datacenter-9.2.1.49989.zip
RUN set -eux;     addgroup -S -g 1000 sonarqube;     adduser -S -D -u 1000 -G sonarqube sonarqube;     apk add --no-cache --virtual build-dependencies gnupg unzip curl;     apk add --no-cache bash su-exec ttf-dejavu openjdk11-jre;     echo "networkaddress.cache.ttl=5" >> "${JAVA_HOME}/conf/security/java.security";     sed --in-place --expression="s?securerandom.source=file:/dev/random?securerandom.source=file:/dev/urandom?g" "${JAVA_HOME}/conf/security/java.security";     for server in $(shuf -e ha.pool.sks-keyservers.net                             hkp://p80.pool.sks-keyservers.net:80                             keyserver.ubuntu.com                             hkp://keyserver.ubuntu.com:80                             pgp.mit.edu) ; do         gpg --batch --keyserver "${server}" --recv-keys 679F1EE92B19609DE816FDE81DB198F93525EC1A && break || : ;     done;     mkdir --parents /opt ;    cd /opt;     curl --fail --location --output sonarqube.zip --silent --show-error "${SONARQUBE_ZIP_URL}";     curl --fail --location --output sonarqube.zip.asc --silent --show-error "${SONARQUBE_ZIP_URL}.asc";     gpg --batch --verify sonarqube.zip.asc sonarqube.zip;     unzip -q sonarqube.zip;     mv "sonarqube-${SONARQUBE_VERSION}" sonarqube;     rm sonarqube.zip*;     rm -rf ${SONARQUBE_HOME}/bin/*;     chown -R sonarqube:sonarqube ${SONARQUBE_HOME} ;     chmod -R 777 "${SQ_DATA_DIR}" "${SQ_EXTENSIONS_DIR}" "${SQ_LOGS_DIR}" "${SQ_TEMP_DIR}" ;     apk del --purge build-dependencies;
# Tue, 30 Nov 2021 00:50:06 GMT
COPY --chown=sonarqube:sonarqubemulti:8997cda09b77db3cd2004e36d485c5b54ddd96e9993642921bc6be78ee8af554 in /opt/sonarqube/bin/ 
# Tue, 30 Nov 2021 00:50:06 GMT
WORKDIR /opt/sonarqube
# Tue, 30 Nov 2021 00:50:06 GMT
EXPOSE 9000
# Tue, 30 Nov 2021 00:50:06 GMT
STOPSIGNAL SIGINT
# Tue, 30 Nov 2021 00:50:07 GMT
ENTRYPOINT ["/opt/sonarqube/bin/run.sh"]
# Tue, 30 Nov 2021 00:50:07 GMT
CMD ["/opt/sonarqube/bin/sonar.sh"]
```

-	Layers:
	-	`sha256:97518928ae5f3d52d4164b314a7e73654eb686ecd8aafa0b79acd980773a740d`  
		Last Modified: Fri, 12 Nov 2021 17:20:39 GMT  
		Size: 2.8 MB (2822981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf766528714d55cd3401caca2530cf058dd147c2950a1699ee27440465fd106f`  
		Last Modified: Tue, 30 Nov 2021 00:54:32 GMT  
		Size: 506.7 MB (506703541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f00b61e003b4feb5ab604f158301a68aceffbb5579b489cdc7d1281c915eddeb`  
		Last Modified: Tue, 30 Nov 2021 00:54:02 GMT  
		Size: 1.5 KB (1512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
