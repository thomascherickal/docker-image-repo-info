## `telegraf:alpine`

```console
$ docker pull telegraf@sha256:36b91f1582e5135cf7b364254c58f5b1089279c9aada634da80be47cc89a96df
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `telegraf:alpine` - linux; amd64

```console
$ docker pull telegraf@sha256:7e38484d276e49516ca195d478859650659d0057d2fdfdd34a4c139167db8a1d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.7 MB (31650834 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b3e24cbd9987bbf706e6ce8bdb7a9bfc02622bb77af5e2ebfccbfc500b83909a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Wed, 31 Mar 2021 20:10:13 GMT
ADD file:f77db8e5b937d8ebb7e254eccd4d311798ea9f4dd5081ea2a7e2b1d3790300c2 in / 
# Wed, 31 Mar 2021 20:10:13 GMT
CMD ["/bin/sh"]
# Wed, 31 Mar 2021 22:08:42 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 31 Mar 2021 22:46:56 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata &&     update-ca-certificates
# Wed, 31 Mar 2021 22:47:44 GMT
ENV TELEGRAF_VERSION=1.18.0
# Wed, 31 Mar 2021 22:47:48 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Wed, 31 Mar 2021 22:47:49 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 31 Mar 2021 22:47:49 GMT
COPY file:a8a66b0d8dac2aee66897c63ce9b7a3d282bb5d7b796ffb12c2cd9227fed341b in /entrypoint.sh 
# Wed, 31 Mar 2021 22:47:49 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 31 Mar 2021 22:47:49 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:532819f3e44cebad88c82f5393801acb876b7a61d36b84bce646561789bb2018`  
		Last Modified: Wed, 31 Mar 2021 20:11:03 GMT  
		Size: 2.8 MB (2799712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b38a141eb441d0521693dd710eb5a2a3ceae66767667e8820f152011f8f8a1de`  
		Last Modified: Wed, 31 Mar 2021 22:12:27 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e3d7ca742af0ce468e2012708013276fbd53bc83cbfbc6067bee7576dfc77fd`  
		Last Modified: Wed, 31 Mar 2021 22:48:32 GMT  
		Size: 3.3 MB (3300612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3416fc49face30e14e2ca552ea8a524ab14963560a5ee9f61b4decba732d7868`  
		Last Modified: Wed, 31 Mar 2021 22:49:45 GMT  
		Size: 25.6 MB (25550173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:322d29285336a8ea82c427137430dce78b0018e178ee228df76215f4e6536815`  
		Last Modified: Wed, 31 Mar 2021 22:49:39 GMT  
		Size: 182.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
