## `influxdb:data-alpine`

```console
$ docker pull influxdb@sha256:fc6d916dc0e8e0dc8e35dd8b569f2e672af9219fbd63c0daa34637c4cba6f4ac
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `influxdb:data-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:e42328040adac22e4e7895c654eb37235277b08ad61fa38799731cb0100ba62e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.2 MB (70173301 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0423dd66da6accc89eb4214f453956f19c3ba6c0e44b7af1f7df3c2368bfd88b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:35 GMT
ADD file:a0afd0b0db7f9ee9496186ead087ec00edd1386ea8c018557d15720053f7308e in / 
# Fri, 24 Apr 2020 01:05:35 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 14:15:54 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Fri, 24 Apr 2020 15:28:09 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Wed, 15 Jul 2020 00:21:11 GMT
ENV INFLUXDB_VERSION=1.8.1-c1.8.1
# Wed, 15 Jul 2020 00:21:18 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Wed, 15 Jul 2020 00:21:18 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Wed, 15 Jul 2020 00:21:19 GMT
EXPOSE 8086
# Wed, 15 Jul 2020 00:21:19 GMT
VOLUME [/var/lib/influxdb]
# Wed, 15 Jul 2020 00:21:19 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Wed, 15 Jul 2020 00:21:19 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Wed, 15 Jul 2020 00:21:19 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 15 Jul 2020 00:21:20 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:31603596830fc7e56753139f9c2c6bd3759e48a850659506ebfb885d1cf3aef5`  
		Last Modified: Fri, 24 Apr 2020 01:06:12 GMT  
		Size: 2.8 MB (2773413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:321996f3080d1a7516b5914e27460b495eb04950d0190554844f395e7be9c793`  
		Last Modified: Fri, 24 Apr 2020 14:16:40 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9984b0a697389d40ad58252364c9cbb4e4a5258602767230a8f149134746718`  
		Last Modified: Fri, 24 Apr 2020 15:30:04 GMT  
		Size: 1.9 MB (1863602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5ff18872a887bf990e02501bbd33e315b94ae545b55f4d285bbeeb610a7ef72`  
		Last Modified: Wed, 15 Jul 2020 00:22:48 GMT  
		Size: 65.5 MB (65534361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbf3a27e97265ff02cd0fccbfc01f3147517b9a3c7375960675e9bfb38c60765`  
		Last Modified: Wed, 15 Jul 2020 00:22:38 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a027b0bd7f86077fd5e75a3da497d00f3c332d33a0d33500d72111e2e31c2b9a`  
		Last Modified: Wed, 15 Jul 2020 00:22:38 GMT  
		Size: 252.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aef61dc5578ad7509620181765e9f485bc80ca56b3a7de05a9780eaabe870ef5`  
		Last Modified: Wed, 15 Jul 2020 00:22:38 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
