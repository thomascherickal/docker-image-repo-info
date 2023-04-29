## `kapacitor:alpine`

```console
$ docker pull kapacitor@sha256:ae18d242a2c3e38dab667b058e6e1c1c32db3985089eb07bbff7a1124749fc48
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `kapacitor:alpine` - linux; amd64

```console
$ docker pull kapacitor@sha256:73bb692306ea33eecba6040c0e63819c1ae048c49186a6f2c80c7d3eb6cc2c0a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.7 MB (68673446 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:084421861cb41acf17a0a5c19fa524a1cd1b2233e96cbb6554bcae217c7543b0`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:28 GMT
ADD file:970e6b2578ef73457ffed1189e8ba128b0211cabd3174b8c7d3afd8fb58ad614 in / 
# Wed, 29 Mar 2023 18:19:28 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 22:13:55 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 29 Mar 2023 22:13:56 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Fri, 28 Apr 2023 23:23:01 GMT
ENV KAPACITOR_VERSION=1.6.6
# Fri, 28 Apr 2023 23:23:12 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor-${KAPACITOR_VERSION}_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor-${KAPACITOR_VERSION}_linux_amd64.tar.gz &&     gpg --batch --verify kapacitor-${KAPACITOR_VERSION}_linux_amd64.tar.gz.asc kapacitor-${KAPACITOR_VERSION}_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf kapacitor-${KAPACITOR_VERSION}_linux_amd64.tar.gz &&     cp -ar /usr/src/kapacitor-*/* / &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Fri, 28 Apr 2023 23:23:12 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Fri, 28 Apr 2023 23:23:12 GMT
EXPOSE 9092
# Fri, 28 Apr 2023 23:23:12 GMT
VOLUME [/var/lib/kapacitor]
# Fri, 28 Apr 2023 23:23:12 GMT
COPY file:a64543022a380a96e18ddc4e841e034238df340064743d570fa109d5086b123a in /entrypoint.sh 
# Fri, 28 Apr 2023 23:23:12 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 28 Apr 2023 23:23:13 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:91d30c5bc19582de1415b18f1ec5bcbf52a558b62cf6cc201c9669df9f748c22`  
		Last Modified: Wed, 29 Mar 2023 18:20:09 GMT  
		Size: 2.8 MB (2807803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:562ec21068704bb8efd8a6db94153756f2ea649fc15b7a3d8c5ae495403deaff`  
		Last Modified: Fri, 28 Apr 2023 23:24:06 GMT  
		Size: 281.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d500101053a8592e41f90d59292cd74a1d55daea7ae9ae255f54f3c3b0bafa0`  
		Last Modified: Fri, 28 Apr 2023 23:24:07 GMT  
		Size: 284.8 KB (284768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33f632df2bffbd0c0aef5f148bd642609bbd3769c3a2f68af212c24569fe3059`  
		Last Modified: Fri, 28 Apr 2023 23:24:14 GMT  
		Size: 65.6 MB (65580141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fe03849db0a97866932a7b703905538b0d9190b841dbc50e49d72d1840cf605`  
		Last Modified: Fri, 28 Apr 2023 23:24:07 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f533d079920207448963e4c621b57d4b0faad5d7eabc65bf0171e777ec58e465`  
		Last Modified: Fri, 28 Apr 2023 23:24:07 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
