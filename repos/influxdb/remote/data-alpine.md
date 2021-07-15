## `influxdb:data-alpine`

```console
$ docker pull influxdb@sha256:5d7984b19ebeae696e3a72d0d3be4d8f8ae98a26a059c30cd514d7327b328a1e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:data-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:e84363979b5ea93eb60066bdc93d41b14d17c4f34b1f9f01f64b5fbe726df1cf
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.7 MB (70748308 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e4a2b986dd07e77d8096bc74a754722028e44638e034361d54b091bf393c3cf`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:49 GMT
ADD file:4f526aa99067d82b341f7ca538f7826b7c23a628f1b615eea2883a2d434c1b90 in / 
# Wed, 14 Apr 2021 19:19:49 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:12:38 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 14 Apr 2021 22:56:19 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Mon, 24 May 2021 19:21:17 GMT
ENV INFLUXDB_VERSION=1.8.6-c1.8.6
# Tue, 29 Jun 2021 02:47:56 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Tue, 29 Jun 2021 02:47:57 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Tue, 29 Jun 2021 02:47:57 GMT
EXPOSE 8086
# Tue, 29 Jun 2021 02:47:58 GMT
VOLUME [/var/lib/influxdb]
# Tue, 29 Jun 2021 02:47:59 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Tue, 29 Jun 2021 02:47:59 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Tue, 29 Jun 2021 02:47:59 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 29 Jun 2021 02:48:00 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:339de151aab4bc06eed8409daae147c408478cb538dacb90cc63f19ad4eba80b`  
		Last Modified: Wed, 14 Apr 2021 19:20:51 GMT  
		Size: 2.8 MB (2800567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4496f95da0ff203c55ba4ff45e6cc518bfd24507a21516931244d25e8db7d14`  
		Last Modified: Wed, 14 Apr 2021 20:13:37 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e1699ff2fb9d4dfb68fba8d9ca2ddea7f21d9a1e0b3e92a61555bec3b1f2369`  
		Last Modified: Wed, 14 Apr 2021 22:58:41 GMT  
		Size: 1.4 MB (1430783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a97a8d8f09c90b1a78add4731e617075475228aa15ebd842f786082506157d4b`  
		Last Modified: Tue, 29 Jun 2021 02:53:33 GMT  
		Size: 66.5 MB (66515006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b888d7236b6084c80f45090dcc6b19a6c5ea223bb98fabfe8c28c1f1720e016`  
		Last Modified: Tue, 29 Jun 2021 02:53:23 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0257283109ba2c40cae5ec75d6b30432c2b68de3ff5d79273c97cde6a6cc9c1`  
		Last Modified: Tue, 29 Jun 2021 02:53:23 GMT  
		Size: 252.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:446dae2e30b64005cca683af402f69f5c94573556a3ec08cd3784bd7069f74df`  
		Last Modified: Tue, 29 Jun 2021 02:53:23 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
