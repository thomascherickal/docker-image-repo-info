## `chronograf:alpine`

```console
$ docker pull chronograf@sha256:cf92fc3cc4691bd74be8d509e1daca31c444deeda4f588d763a6dbf938b01403
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `chronograf:alpine` - linux; amd64

```console
$ docker pull chronograf@sha256:38373234e15d1c93f102793597e9bf12e862d1c6aa7585a0bcba9c07ebc77621
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.8 MB (22808785 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ced3757bcaca9904d45cc79b6978e0aa53759fa9d16a4fb13fa24be010091f25`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:07 GMT
ADD file:b9bd10cf83356cb7281baa0fbaca5186cf27491f59eda87abe57f83a5aaf5ec1 in / 
# Tue, 09 Aug 2022 17:20:08 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 18:17:07 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Tue, 09 Aug 2022 18:17:08 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Tue, 09 Aug 2022 18:17:38 GMT
ENV CHRONOGRAF_VERSION=1.9.4
# Tue, 09 Aug 2022 18:17:43 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/chronograf-*/chronograf.conf &&     chmod +x /usr/src/chronograf-*/* &&     cp -a /usr/src/chronograf-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Tue, 09 Aug 2022 18:17:43 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 09 Aug 2022 18:17:43 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 09 Aug 2022 18:17:43 GMT
EXPOSE 8888
# Tue, 09 Aug 2022 18:17:43 GMT
VOLUME [/var/lib/chronograf]
# Tue, 09 Aug 2022 18:17:43 GMT
COPY file:91fe01086b7984524af1eeb6657c6aea15ce5e169fd42a42e1ef2c54374d30a2 in /entrypoint.sh 
# Tue, 09 Aug 2022 18:17:43 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 09 Aug 2022 18:17:43 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:c7ed990a2339ee598662849de4f56e2241399f5a32340c8c4a7bbd5378a12b5f`  
		Last Modified: Tue, 09 Aug 2022 17:21:06 GMT  
		Size: 2.8 MB (2827489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86b667f667e0d162df357cbdea46ee3457fd45395b451ccad50381f4665f8149`  
		Last Modified: Tue, 09 Aug 2022 18:18:09 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86aedf0b86f2f672427bd99edb4d53285ee3f072fdd5e4ea92fd315f1f9d2bb8`  
		Last Modified: Tue, 09 Aug 2022 18:18:07 GMT  
		Size: 284.6 KB (284571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e63ea984c81d9a176e87bff3e349d81ffb7375a5fbb71f461b755a13a4e2ab17`  
		Last Modified: Tue, 09 Aug 2022 18:18:51 GMT  
		Size: 19.7 MB (19672179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8828c26e16c48e93e2262d948136dc8b4f87b0a28d6a7b29b71e7a18844c1a34`  
		Last Modified: Tue, 09 Aug 2022 18:18:47 GMT  
		Size: 12.3 KB (12263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:015194f0f71e31bae9c869e9a3a8d1ceca19267c54f9cc06ac3e2a9236a89f57`  
		Last Modified: Tue, 09 Aug 2022 18:18:47 GMT  
		Size: 11.9 KB (11893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0585391111ba79d1f1c74c4c722494c1e3378ab7694b9df14300c55ff270fe0`  
		Last Modified: Tue, 09 Aug 2022 18:18:47 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
