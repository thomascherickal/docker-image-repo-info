## `kapacitor:alpine`

```console
$ docker pull kapacitor@sha256:9d1fea13f74037a873977f35976edc7f524287c85ee2ca78798443311d8e1794
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `kapacitor:alpine` - linux; amd64

```console
$ docker pull kapacitor@sha256:7b80b18e0b03667ed5646cbb8f99ac28757a4f4740a2dc65d3b7d53f3e4e5b61
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.4 MB (61448749 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:deab38f6e54c02a09af803e498e85900c59830648fc96707b475abc2e857902c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Thu, 17 Mar 2022 15:19:26 GMT
ADD file:8ec3735d4b1b4b070607b94e3bd360117b07dc26e1baf5dd485b49b3413e8fff in / 
# Thu, 17 Mar 2022 15:19:26 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 18:05:42 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 17 Mar 2022 18:05:43 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Thu, 17 Mar 2022 18:06:24 GMT
ENV KAPACITOR_VERSION=1.6.3
# Thu, 17 Mar 2022 18:06:52 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor-${KAPACITOR_VERSION}_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor-${KAPACITOR_VERSION}_linux_amd64.tar.gz &&     gpg --batch --verify kapacitor-${KAPACITOR_VERSION}_linux_amd64.tar.gz.asc kapacitor-${KAPACITOR_VERSION}_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf kapacitor-${KAPACITOR_VERSION}_linux_amd64.tar.gz &&     cp -ar /usr/src/kapacitor-*/* / &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Thu, 17 Mar 2022 18:06:53 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Thu, 17 Mar 2022 18:06:53 GMT
EXPOSE 9092
# Thu, 17 Mar 2022 18:06:53 GMT
VOLUME [/var/lib/kapacitor]
# Thu, 17 Mar 2022 18:06:53 GMT
COPY file:a64543022a380a96e18ddc4e841e034238df340064743d570fa109d5086b123a in /entrypoint.sh 
# Thu, 17 Mar 2022 18:06:53 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Mar 2022 18:06:53 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:36ccefbf3d8a9a1b18baaa9cbf0f3ad50e8a7b751656c74df359900a318cbffc`  
		Last Modified: Thu, 17 Mar 2022 15:20:13 GMT  
		Size: 2.8 MB (2816169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffa1326b35d047e371043a2411e65bd818c27909ab1ecf1ce37b55741744e890`  
		Last Modified: Thu, 17 Mar 2022 18:07:13 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85eb6277290b589d592446e2f538670a432e8a6e60772ee08f89a2055bef71ec`  
		Last Modified: Thu, 17 Mar 2022 18:07:13 GMT  
		Size: 271.7 KB (271670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b4ad12656fe460f674ab7f5ec540772003d0372d5fd248843987826b0977f2f`  
		Last Modified: Thu, 17 Mar 2022 18:07:36 GMT  
		Size: 58.4 MB (58360302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:641a70ee4993f9c1c1c87380e01bb51c766fdcfbb98fd0f4bedefdacd566b962`  
		Last Modified: Thu, 17 Mar 2022 18:07:28 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbb68c806ef27ef0b5cf3bdbba4fa0c5d9ec667945ee6da1ba24571ab50e7be3`  
		Last Modified: Thu, 17 Mar 2022 18:07:28 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
