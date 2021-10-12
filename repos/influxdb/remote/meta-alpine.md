## `influxdb:meta-alpine`

```console
$ docker pull influxdb@sha256:c14412e9051e84e8d6bb2e73147dd79eb5381d2d47fdecd19524d20af54f1359
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:meta-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:46bb24530636472e50b1b9ccf517430905a4e773437983218a6f57cc0c8c93ed
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.6 MB (27572254 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a2535ab47162451d3c3d50f3236ace5eb8e52a9cfc616ff8af833f51de51875`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Thu, 16 Sep 2021 21:20:06 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 16 Sep 2021 21:20:08 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Mon, 11 Oct 2021 23:20:37 GMT
ENV INFLUXDB_VERSION=1.8.10-c1.8.10
# Mon, 11 Oct 2021 23:21:14 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb-meta.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Mon, 11 Oct 2021 23:21:15 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Mon, 11 Oct 2021 23:21:15 GMT
EXPOSE 8091
# Mon, 11 Oct 2021 23:21:15 GMT
VOLUME [/var/lib/influxdb]
# Mon, 11 Oct 2021 23:21:15 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Mon, 11 Oct 2021 23:21:15 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 11 Oct 2021 23:21:16 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e8cf55ffd68f3512245522356168367182cfdaeb0a0d11bbd5328472d4c0761`  
		Last Modified: Thu, 16 Sep 2021 21:24:04 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7457db31b732bcfa93e8a40c987909364acc021b8a962de6d8f77e9a46830fee`  
		Last Modified: Thu, 16 Sep 2021 21:24:02 GMT  
		Size: 1.5 MB (1464176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae1969092b409f910536cd2ae2b8d930b0b3bd9a62c4edc0eb306ceaad9d8723`  
		Last Modified: Mon, 11 Oct 2021 23:23:53 GMT  
		Size: 23.3 MB (23292882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f3a46cc6cbfd7f616c01f2861ef1b1905b452913950566d4470641bb31c871b`  
		Last Modified: Mon, 11 Oct 2021 23:23:50 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:926287724a1fc5ec8210568eaf0f15438481e47e302691e6ff9921b200ff6f9e`  
		Last Modified: Mon, 11 Oct 2021 23:23:50 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
