<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `influxdb`

-	[`influxdb:1.10-data`](#influxdb110-data)
-	[`influxdb:1.10-data-alpine`](#influxdb110-data-alpine)
-	[`influxdb:1.10-meta`](#influxdb110-meta)
-	[`influxdb:1.10-meta-alpine`](#influxdb110-meta-alpine)
-	[`influxdb:1.10.0-data`](#influxdb1100-data)
-	[`influxdb:1.10.0-data-alpine`](#influxdb1100-data-alpine)
-	[`influxdb:1.10.0-meta`](#influxdb1100-meta)
-	[`influxdb:1.10.0-meta-alpine`](#influxdb1100-meta-alpine)
-	[`influxdb:1.8`](#influxdb18)
-	[`influxdb:1.8-alpine`](#influxdb18-alpine)
-	[`influxdb:1.8-data`](#influxdb18-data)
-	[`influxdb:1.8-data-alpine`](#influxdb18-data-alpine)
-	[`influxdb:1.8-meta`](#influxdb18-meta)
-	[`influxdb:1.8-meta-alpine`](#influxdb18-meta-alpine)
-	[`influxdb:1.8.10`](#influxdb1810)
-	[`influxdb:1.8.10-alpine`](#influxdb1810-alpine)
-	[`influxdb:1.8.10-data`](#influxdb1810-data)
-	[`influxdb:1.8.10-data-alpine`](#influxdb1810-data-alpine)
-	[`influxdb:1.8.10-meta`](#influxdb1810-meta)
-	[`influxdb:1.8.10-meta-alpine`](#influxdb1810-meta-alpine)
-	[`influxdb:1.9-data`](#influxdb19-data)
-	[`influxdb:1.9-data-alpine`](#influxdb19-data-alpine)
-	[`influxdb:1.9-meta`](#influxdb19-meta)
-	[`influxdb:1.9-meta-alpine`](#influxdb19-meta-alpine)
-	[`influxdb:1.9.9-data`](#influxdb199-data)
-	[`influxdb:1.9.9-data-alpine`](#influxdb199-data-alpine)
-	[`influxdb:1.9.9-meta`](#influxdb199-meta)
-	[`influxdb:1.9.9-meta-alpine`](#influxdb199-meta-alpine)
-	[`influxdb:2.4`](#influxdb24)
-	[`influxdb:2.4-alpine`](#influxdb24-alpine)
-	[`influxdb:2.4.0`](#influxdb240)
-	[`influxdb:2.4.0-alpine`](#influxdb240-alpine)
-	[`influxdb:2.5`](#influxdb25)
-	[`influxdb:2.5-alpine`](#influxdb25-alpine)
-	[`influxdb:2.5.1`](#influxdb251)
-	[`influxdb:2.5.1-alpine`](#influxdb251-alpine)
-	[`influxdb:2.6`](#influxdb26)
-	[`influxdb:2.6-alpine`](#influxdb26-alpine)
-	[`influxdb:2.6.1`](#influxdb261)
-	[`influxdb:2.6.1-alpine`](#influxdb261-alpine)
-	[`influxdb:alpine`](#influxdbalpine)
-	[`influxdb:data`](#influxdbdata)
-	[`influxdb:data-alpine`](#influxdbdata-alpine)
-	[`influxdb:latest`](#influxdblatest)
-	[`influxdb:meta`](#influxdbmeta)
-	[`influxdb:meta-alpine`](#influxdbmeta-alpine)

## `influxdb:1.10-data`

```console
$ docker pull influxdb@sha256:dfd85723f2e810672f18cef91d0dff50378978b5a7fbb18ad9f55067d0261fe4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.10-data` - linux; amd64

```console
$ docker pull influxdb@sha256:eb16a94be743d181c01420d57887dfdc007fa57ba7783bdb4d6937dbf036dac8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.8 MB (101786160 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:85b0c19025aaa219dbebc1246955ea52f1379c3375b6e57e0922bdd34b72d869`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 01 Mar 2023 04:09:45 GMT
ADD file:513c5d5e501279c21a05c1d8b66e5f0b02ee4b27f0b928706d92fd9ce11c1be6 in / 
# Wed, 01 Mar 2023 04:09:46 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 04:42:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 04:42:43 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Mar 2023 00:54:43 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 16 Mar 2023 00:56:11 GMT
ENV INFLUXDB_VERSION=1.10.0-c1.10.0
# Thu, 16 Mar 2023 00:56:14 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-data_${INFLUXDB_VERSION}_amd64.deb*
# Thu, 16 Mar 2023 00:56:14 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Thu, 16 Mar 2023 00:56:14 GMT
EXPOSE 8086
# Thu, 16 Mar 2023 00:56:14 GMT
VOLUME [/var/lib/influxdb]
# Thu, 16 Mar 2023 00:56:14 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Thu, 16 Mar 2023 00:56:14 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Thu, 16 Mar 2023 00:56:14 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 16 Mar 2023 00:56:14 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:32fb02163b6bb519a30f909008e852354dae10bdfd6b34190dbdfe8f15403ea0`  
		Last Modified: Wed, 01 Mar 2023 04:13:58 GMT  
		Size: 55.0 MB (55045922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:167c7feebee855d117e192389484ea8367be1ba84e7ee35f4e5e5663195facbf`  
		Last Modified: Wed, 01 Mar 2023 04:50:15 GMT  
		Size: 5.2 MB (5166586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6dfff1f6f3ddd2194ea0775f199572e8b2d75c38713eef0444d6b1fd0ac7604`  
		Last Modified: Wed, 01 Mar 2023 04:50:15 GMT  
		Size: 10.9 MB (10876729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a90f0187c37c44f2ad04f9d930d40ee0b886fc8d783b914b10a620683739873`  
		Last Modified: Thu, 16 Mar 2023 00:58:47 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8d4f0618bce2be1d9d071eaa7c7ef778206d6649dc4ea276634549829ae2f6e`  
		Last Modified: Thu, 16 Mar 2023 01:01:25 GMT  
		Size: 30.7 MB (30693353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f56cee2eda3477486b153b5a4b1363c33585dda4994881006d24b37919a24a2`  
		Last Modified: Thu, 16 Mar 2023 01:01:20 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11d6d34e6091ad1ce6896443686fd609c10f0d42667b93179be9b50fe3c152f4`  
		Last Modified: Thu, 16 Mar 2023 01:01:20 GMT  
		Size: 252.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a4203c953cd30a830833c56193a9b2078e1b29da4783783ede56d22ec100f60`  
		Last Modified: Thu, 16 Mar 2023 01:01:20 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.10-data-alpine`

```console
$ docker pull influxdb@sha256:440bd99e9114c717bf88c877f9f08e0d826cf8ec8b61f32f2e850a18217c0243
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.10-data-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:f8534f7b2174c74fc2dad95fe8a3052dd3e79eb34b78e720214baa1a72432676
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.5 MB (35500417 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:01bd67316e73444e27787910facf83492fa4d07a08edb3cd780704e40953d074`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:42 GMT
ADD file:40887ab7c06977737e63c215c9bd297c0c74de8d12d16ebdf1c3d40ac392f62d in / 
# Sat, 11 Feb 2023 04:46:42 GMT
CMD ["/bin/sh"]
# Mon, 13 Mar 2023 23:20:24 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 16 Mar 2023 00:54:52 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Thu, 16 Mar 2023 00:56:17 GMT
ENV INFLUXDB_VERSION=1.10.0-c1.10.0
# Thu, 16 Mar 2023 00:56:25 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb.conf &&     chmod +x /usr/src/influxdb-*/usr/bin/* &&     cp -a /usr/src/influxdb-*/usr/bin/. /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Thu, 16 Mar 2023 00:56:26 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Thu, 16 Mar 2023 00:56:26 GMT
EXPOSE 8086
# Thu, 16 Mar 2023 00:56:26 GMT
VOLUME [/var/lib/influxdb]
# Thu, 16 Mar 2023 00:56:26 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Thu, 16 Mar 2023 00:56:26 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Thu, 16 Mar 2023 00:56:26 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 16 Mar 2023 00:56:26 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:63b65145d645c1250c391b2d16ebe53b3747c295ca8ba2fcb6b0cf064a4dc21c`  
		Last Modified: Fri, 10 Feb 2023 22:41:31 GMT  
		Size: 3.4 MB (3374446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69b7a2cbfc2f3b3305293d689573f3c9651d6053e5f780a9ba42a4c836d8d6c9`  
		Last Modified: Mon, 13 Mar 2023 23:21:18 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5b0a9605b8bc1c4f3b877c51f73e8d0cc4b02403f8f9d18c276f012b604c038`  
		Last Modified: Thu, 16 Mar 2023 00:59:03 GMT  
		Size: 1.5 MB (1472712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf0f10c7988b3fb97c7aad83f461a16463e4d142712e018cb590ec70569c805a`  
		Last Modified: Thu, 16 Mar 2023 01:01:38 GMT  
		Size: 30.7 MB (30651183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61b7f7e2d370084336be005363edd68862e66496ade1edd0d46f9508447a27ad`  
		Last Modified: Thu, 16 Mar 2023 01:01:33 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b802d11efa85aafe96a391b20f7f72c41cee1a2cdcdaade5438709ed354c8900`  
		Last Modified: Thu, 16 Mar 2023 01:01:33 GMT  
		Size: 252.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8fb3c196e555a953e72f39f796432c6d96af0b51adcf0f75670b67e737e9b24`  
		Last Modified: Thu, 16 Mar 2023 01:01:33 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.10-meta`

```console
$ docker pull influxdb@sha256:0400963cc6ac96953384ddbe9107d1fb7f12864d8df6a289954e822f0df77230
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.10-meta` - linux; amd64

```console
$ docker pull influxdb@sha256:dfa9c58632e19d799c6e2ab9d11696d050fb6284b7446497a4688f3f725d0d08
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.0 MB (82998826 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:61fcd04f9c9dd697a1bc8c56ecc97fe15b42137df310aa5522e98a9684d18c42`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Wed, 01 Mar 2023 04:09:45 GMT
ADD file:513c5d5e501279c21a05c1d8b66e5f0b02ee4b27f0b928706d92fd9ce11c1be6 in / 
# Wed, 01 Mar 2023 04:09:46 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 04:42:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 04:42:43 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Mar 2023 00:54:43 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 16 Mar 2023 00:56:11 GMT
ENV INFLUXDB_VERSION=1.10.0-c1.10.0
# Thu, 16 Mar 2023 00:56:31 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-meta_${INFLUXDB_VERSION}_amd64.deb*
# Thu, 16 Mar 2023 00:56:31 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Thu, 16 Mar 2023 00:56:31 GMT
EXPOSE 8091
# Thu, 16 Mar 2023 00:56:31 GMT
VOLUME [/var/lib/influxdb]
# Thu, 16 Mar 2023 00:56:31 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Thu, 16 Mar 2023 00:56:31 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 16 Mar 2023 00:56:31 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:32fb02163b6bb519a30f909008e852354dae10bdfd6b34190dbdfe8f15403ea0`  
		Last Modified: Wed, 01 Mar 2023 04:13:58 GMT  
		Size: 55.0 MB (55045922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:167c7feebee855d117e192389484ea8367be1ba84e7ee35f4e5e5663195facbf`  
		Last Modified: Wed, 01 Mar 2023 04:50:15 GMT  
		Size: 5.2 MB (5166586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6dfff1f6f3ddd2194ea0775f199572e8b2d75c38713eef0444d6b1fd0ac7604`  
		Last Modified: Wed, 01 Mar 2023 04:50:15 GMT  
		Size: 10.9 MB (10876729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a90f0187c37c44f2ad04f9d930d40ee0b886fc8d783b914b10a620683739873`  
		Last Modified: Thu, 16 Mar 2023 00:58:47 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e1b5e504a28132b86e2f51133d89248f25def13b663951e20d25679992f5e51`  
		Last Modified: Thu, 16 Mar 2023 01:01:48 GMT  
		Size: 11.9 MB (11907227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85e3633ae29520b0e78828fd892816296780bac6596517e603229e68bedef0ab`  
		Last Modified: Thu, 16 Mar 2023 01:01:46 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c44d2cc57cf88a2b99f5c30df2cb651b2829922810f549dee2a413207a430ed`  
		Last Modified: Thu, 16 Mar 2023 01:01:46 GMT  
		Size: 371.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.10-meta-alpine`

```console
$ docker pull influxdb@sha256:4355131382f0a33ebbb7795e70ee2907f0c2f9329e43fb7c78eb3f425275ad1b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.10-meta-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:3bc62e0f4f5f03ec7e23973867c8526b13f7c1f8fe1546bef8711144808b235a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.7 MB (16719836 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a241efb62d89b90a8152a80cedafdcc9b0f4b69a127e80bf2126a421481a8e6`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:42 GMT
ADD file:40887ab7c06977737e63c215c9bd297c0c74de8d12d16ebdf1c3d40ac392f62d in / 
# Sat, 11 Feb 2023 04:46:42 GMT
CMD ["/bin/sh"]
# Mon, 13 Mar 2023 23:20:24 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 16 Mar 2023 00:54:52 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Thu, 16 Mar 2023 00:56:17 GMT
ENV INFLUXDB_VERSION=1.10.0-c1.10.0
# Thu, 16 Mar 2023 00:56:39 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb-meta.conf &&     chmod +x /usr/src/influxdb-*/usr/bin/* &&     cp -a /usr/src/influxdb-*/usr/bin/. /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Thu, 16 Mar 2023 00:56:39 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Thu, 16 Mar 2023 00:56:39 GMT
EXPOSE 8091
# Thu, 16 Mar 2023 00:56:39 GMT
VOLUME [/var/lib/influxdb]
# Thu, 16 Mar 2023 00:56:40 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Thu, 16 Mar 2023 00:56:40 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 16 Mar 2023 00:56:40 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:63b65145d645c1250c391b2d16ebe53b3747c295ca8ba2fcb6b0cf064a4dc21c`  
		Last Modified: Fri, 10 Feb 2023 22:41:31 GMT  
		Size: 3.4 MB (3374446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69b7a2cbfc2f3b3305293d689573f3c9651d6053e5f780a9ba42a4c836d8d6c9`  
		Last Modified: Mon, 13 Mar 2023 23:21:18 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5b0a9605b8bc1c4f3b877c51f73e8d0cc4b02403f8f9d18c276f012b604c038`  
		Last Modified: Thu, 16 Mar 2023 00:59:03 GMT  
		Size: 1.5 MB (1472712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63c65c40f13a77c7bea58b8e3b25b6ccf85efb3013c2afee3ab0ae9ed41b1db8`  
		Last Modified: Thu, 16 Mar 2023 01:01:58 GMT  
		Size: 11.9 MB (11871807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:533a22a1ae9ecd3298347cd2c0325db7854ea450f785c2e0027a48c50bcbae6c`  
		Last Modified: Thu, 16 Mar 2023 01:01:56 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f4f6b9e57ab967c9a3052623511f84d434a0dd45ce32a0d239dcc44c58cdcac`  
		Last Modified: Thu, 16 Mar 2023 01:01:56 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.10.0-data`

```console
$ docker pull influxdb@sha256:dfd85723f2e810672f18cef91d0dff50378978b5a7fbb18ad9f55067d0261fe4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.10.0-data` - linux; amd64

```console
$ docker pull influxdb@sha256:eb16a94be743d181c01420d57887dfdc007fa57ba7783bdb4d6937dbf036dac8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.8 MB (101786160 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:85b0c19025aaa219dbebc1246955ea52f1379c3375b6e57e0922bdd34b72d869`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 01 Mar 2023 04:09:45 GMT
ADD file:513c5d5e501279c21a05c1d8b66e5f0b02ee4b27f0b928706d92fd9ce11c1be6 in / 
# Wed, 01 Mar 2023 04:09:46 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 04:42:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 04:42:43 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Mar 2023 00:54:43 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 16 Mar 2023 00:56:11 GMT
ENV INFLUXDB_VERSION=1.10.0-c1.10.0
# Thu, 16 Mar 2023 00:56:14 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-data_${INFLUXDB_VERSION}_amd64.deb*
# Thu, 16 Mar 2023 00:56:14 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Thu, 16 Mar 2023 00:56:14 GMT
EXPOSE 8086
# Thu, 16 Mar 2023 00:56:14 GMT
VOLUME [/var/lib/influxdb]
# Thu, 16 Mar 2023 00:56:14 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Thu, 16 Mar 2023 00:56:14 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Thu, 16 Mar 2023 00:56:14 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 16 Mar 2023 00:56:14 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:32fb02163b6bb519a30f909008e852354dae10bdfd6b34190dbdfe8f15403ea0`  
		Last Modified: Wed, 01 Mar 2023 04:13:58 GMT  
		Size: 55.0 MB (55045922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:167c7feebee855d117e192389484ea8367be1ba84e7ee35f4e5e5663195facbf`  
		Last Modified: Wed, 01 Mar 2023 04:50:15 GMT  
		Size: 5.2 MB (5166586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6dfff1f6f3ddd2194ea0775f199572e8b2d75c38713eef0444d6b1fd0ac7604`  
		Last Modified: Wed, 01 Mar 2023 04:50:15 GMT  
		Size: 10.9 MB (10876729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a90f0187c37c44f2ad04f9d930d40ee0b886fc8d783b914b10a620683739873`  
		Last Modified: Thu, 16 Mar 2023 00:58:47 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8d4f0618bce2be1d9d071eaa7c7ef778206d6649dc4ea276634549829ae2f6e`  
		Last Modified: Thu, 16 Mar 2023 01:01:25 GMT  
		Size: 30.7 MB (30693353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f56cee2eda3477486b153b5a4b1363c33585dda4994881006d24b37919a24a2`  
		Last Modified: Thu, 16 Mar 2023 01:01:20 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11d6d34e6091ad1ce6896443686fd609c10f0d42667b93179be9b50fe3c152f4`  
		Last Modified: Thu, 16 Mar 2023 01:01:20 GMT  
		Size: 252.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a4203c953cd30a830833c56193a9b2078e1b29da4783783ede56d22ec100f60`  
		Last Modified: Thu, 16 Mar 2023 01:01:20 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.10.0-data-alpine`

```console
$ docker pull influxdb@sha256:440bd99e9114c717bf88c877f9f08e0d826cf8ec8b61f32f2e850a18217c0243
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.10.0-data-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:f8534f7b2174c74fc2dad95fe8a3052dd3e79eb34b78e720214baa1a72432676
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.5 MB (35500417 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:01bd67316e73444e27787910facf83492fa4d07a08edb3cd780704e40953d074`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:42 GMT
ADD file:40887ab7c06977737e63c215c9bd297c0c74de8d12d16ebdf1c3d40ac392f62d in / 
# Sat, 11 Feb 2023 04:46:42 GMT
CMD ["/bin/sh"]
# Mon, 13 Mar 2023 23:20:24 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 16 Mar 2023 00:54:52 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Thu, 16 Mar 2023 00:56:17 GMT
ENV INFLUXDB_VERSION=1.10.0-c1.10.0
# Thu, 16 Mar 2023 00:56:25 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb.conf &&     chmod +x /usr/src/influxdb-*/usr/bin/* &&     cp -a /usr/src/influxdb-*/usr/bin/. /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Thu, 16 Mar 2023 00:56:26 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Thu, 16 Mar 2023 00:56:26 GMT
EXPOSE 8086
# Thu, 16 Mar 2023 00:56:26 GMT
VOLUME [/var/lib/influxdb]
# Thu, 16 Mar 2023 00:56:26 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Thu, 16 Mar 2023 00:56:26 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Thu, 16 Mar 2023 00:56:26 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 16 Mar 2023 00:56:26 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:63b65145d645c1250c391b2d16ebe53b3747c295ca8ba2fcb6b0cf064a4dc21c`  
		Last Modified: Fri, 10 Feb 2023 22:41:31 GMT  
		Size: 3.4 MB (3374446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69b7a2cbfc2f3b3305293d689573f3c9651d6053e5f780a9ba42a4c836d8d6c9`  
		Last Modified: Mon, 13 Mar 2023 23:21:18 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5b0a9605b8bc1c4f3b877c51f73e8d0cc4b02403f8f9d18c276f012b604c038`  
		Last Modified: Thu, 16 Mar 2023 00:59:03 GMT  
		Size: 1.5 MB (1472712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf0f10c7988b3fb97c7aad83f461a16463e4d142712e018cb590ec70569c805a`  
		Last Modified: Thu, 16 Mar 2023 01:01:38 GMT  
		Size: 30.7 MB (30651183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61b7f7e2d370084336be005363edd68862e66496ade1edd0d46f9508447a27ad`  
		Last Modified: Thu, 16 Mar 2023 01:01:33 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b802d11efa85aafe96a391b20f7f72c41cee1a2cdcdaade5438709ed354c8900`  
		Last Modified: Thu, 16 Mar 2023 01:01:33 GMT  
		Size: 252.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8fb3c196e555a953e72f39f796432c6d96af0b51adcf0f75670b67e737e9b24`  
		Last Modified: Thu, 16 Mar 2023 01:01:33 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.10.0-meta`

```console
$ docker pull influxdb@sha256:0400963cc6ac96953384ddbe9107d1fb7f12864d8df6a289954e822f0df77230
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.10.0-meta` - linux; amd64

```console
$ docker pull influxdb@sha256:dfa9c58632e19d799c6e2ab9d11696d050fb6284b7446497a4688f3f725d0d08
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.0 MB (82998826 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:61fcd04f9c9dd697a1bc8c56ecc97fe15b42137df310aa5522e98a9684d18c42`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Wed, 01 Mar 2023 04:09:45 GMT
ADD file:513c5d5e501279c21a05c1d8b66e5f0b02ee4b27f0b928706d92fd9ce11c1be6 in / 
# Wed, 01 Mar 2023 04:09:46 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 04:42:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 04:42:43 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Mar 2023 00:54:43 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 16 Mar 2023 00:56:11 GMT
ENV INFLUXDB_VERSION=1.10.0-c1.10.0
# Thu, 16 Mar 2023 00:56:31 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-meta_${INFLUXDB_VERSION}_amd64.deb*
# Thu, 16 Mar 2023 00:56:31 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Thu, 16 Mar 2023 00:56:31 GMT
EXPOSE 8091
# Thu, 16 Mar 2023 00:56:31 GMT
VOLUME [/var/lib/influxdb]
# Thu, 16 Mar 2023 00:56:31 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Thu, 16 Mar 2023 00:56:31 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 16 Mar 2023 00:56:31 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:32fb02163b6bb519a30f909008e852354dae10bdfd6b34190dbdfe8f15403ea0`  
		Last Modified: Wed, 01 Mar 2023 04:13:58 GMT  
		Size: 55.0 MB (55045922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:167c7feebee855d117e192389484ea8367be1ba84e7ee35f4e5e5663195facbf`  
		Last Modified: Wed, 01 Mar 2023 04:50:15 GMT  
		Size: 5.2 MB (5166586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6dfff1f6f3ddd2194ea0775f199572e8b2d75c38713eef0444d6b1fd0ac7604`  
		Last Modified: Wed, 01 Mar 2023 04:50:15 GMT  
		Size: 10.9 MB (10876729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a90f0187c37c44f2ad04f9d930d40ee0b886fc8d783b914b10a620683739873`  
		Last Modified: Thu, 16 Mar 2023 00:58:47 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e1b5e504a28132b86e2f51133d89248f25def13b663951e20d25679992f5e51`  
		Last Modified: Thu, 16 Mar 2023 01:01:48 GMT  
		Size: 11.9 MB (11907227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85e3633ae29520b0e78828fd892816296780bac6596517e603229e68bedef0ab`  
		Last Modified: Thu, 16 Mar 2023 01:01:46 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c44d2cc57cf88a2b99f5c30df2cb651b2829922810f549dee2a413207a430ed`  
		Last Modified: Thu, 16 Mar 2023 01:01:46 GMT  
		Size: 371.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.10.0-meta-alpine`

```console
$ docker pull influxdb@sha256:4355131382f0a33ebbb7795e70ee2907f0c2f9329e43fb7c78eb3f425275ad1b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.10.0-meta-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:3bc62e0f4f5f03ec7e23973867c8526b13f7c1f8fe1546bef8711144808b235a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.7 MB (16719836 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a241efb62d89b90a8152a80cedafdcc9b0f4b69a127e80bf2126a421481a8e6`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:42 GMT
ADD file:40887ab7c06977737e63c215c9bd297c0c74de8d12d16ebdf1c3d40ac392f62d in / 
# Sat, 11 Feb 2023 04:46:42 GMT
CMD ["/bin/sh"]
# Mon, 13 Mar 2023 23:20:24 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 16 Mar 2023 00:54:52 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Thu, 16 Mar 2023 00:56:17 GMT
ENV INFLUXDB_VERSION=1.10.0-c1.10.0
# Thu, 16 Mar 2023 00:56:39 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb-meta.conf &&     chmod +x /usr/src/influxdb-*/usr/bin/* &&     cp -a /usr/src/influxdb-*/usr/bin/. /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Thu, 16 Mar 2023 00:56:39 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Thu, 16 Mar 2023 00:56:39 GMT
EXPOSE 8091
# Thu, 16 Mar 2023 00:56:39 GMT
VOLUME [/var/lib/influxdb]
# Thu, 16 Mar 2023 00:56:40 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Thu, 16 Mar 2023 00:56:40 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 16 Mar 2023 00:56:40 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:63b65145d645c1250c391b2d16ebe53b3747c295ca8ba2fcb6b0cf064a4dc21c`  
		Last Modified: Fri, 10 Feb 2023 22:41:31 GMT  
		Size: 3.4 MB (3374446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69b7a2cbfc2f3b3305293d689573f3c9651d6053e5f780a9ba42a4c836d8d6c9`  
		Last Modified: Mon, 13 Mar 2023 23:21:18 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5b0a9605b8bc1c4f3b877c51f73e8d0cc4b02403f8f9d18c276f012b604c038`  
		Last Modified: Thu, 16 Mar 2023 00:59:03 GMT  
		Size: 1.5 MB (1472712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63c65c40f13a77c7bea58b8e3b25b6ccf85efb3013c2afee3ab0ae9ed41b1db8`  
		Last Modified: Thu, 16 Mar 2023 01:01:58 GMT  
		Size: 11.9 MB (11871807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:533a22a1ae9ecd3298347cd2c0325db7854ea450f785c2e0027a48c50bcbae6c`  
		Last Modified: Thu, 16 Mar 2023 01:01:56 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f4f6b9e57ab967c9a3052623511f84d434a0dd45ce32a0d239dcc44c58cdcac`  
		Last Modified: Thu, 16 Mar 2023 01:01:56 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.8`

```console
$ docker pull influxdb@sha256:dfdff063429b612af16a09a4d64c0971b39427ca8def47df9aa25dfadb17a109
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `influxdb:1.8` - linux; amd64

```console
$ docker pull influxdb@sha256:62058532a6a46c42b7abe920ee9f37e22bcaf5755a7c6c1de4c2538d2c412bb8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.0 MB (125978540 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2dfef349b0709348b4756b8deeb072d87e085cb278c3d1b300a096aa5645f7ce`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 01 Mar 2023 04:09:45 GMT
ADD file:513c5d5e501279c21a05c1d8b66e5f0b02ee4b27f0b928706d92fd9ce11c1be6 in / 
# Wed, 01 Mar 2023 04:09:46 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 04:42:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 04:42:43 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Mar 2023 00:54:43 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 16 Mar 2023 00:54:43 GMT
ENV INFLUXDB_VERSION=1.8.10
# Thu, 16 Mar 2023 00:54:47 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Thu, 16 Mar 2023 00:54:47 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Thu, 16 Mar 2023 00:54:47 GMT
EXPOSE 8086
# Thu, 16 Mar 2023 00:54:47 GMT
VOLUME [/var/lib/influxdb]
# Thu, 16 Mar 2023 00:54:47 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Thu, 16 Mar 2023 00:54:48 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Thu, 16 Mar 2023 00:54:48 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 16 Mar 2023 00:54:48 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:32fb02163b6bb519a30f909008e852354dae10bdfd6b34190dbdfe8f15403ea0`  
		Last Modified: Wed, 01 Mar 2023 04:13:58 GMT  
		Size: 55.0 MB (55045922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:167c7feebee855d117e192389484ea8367be1ba84e7ee35f4e5e5663195facbf`  
		Last Modified: Wed, 01 Mar 2023 04:50:15 GMT  
		Size: 5.2 MB (5166586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6dfff1f6f3ddd2194ea0775f199572e8b2d75c38713eef0444d6b1fd0ac7604`  
		Last Modified: Wed, 01 Mar 2023 04:50:15 GMT  
		Size: 10.9 MB (10876729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a90f0187c37c44f2ad04f9d930d40ee0b886fc8d783b914b10a620683739873`  
		Last Modified: Thu, 16 Mar 2023 00:58:47 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c128af0cbea60d53679d68899e21837db22b0a33bcc3d784bc3078ec82a21b14`  
		Last Modified: Thu, 16 Mar 2023 00:58:54 GMT  
		Size: 54.9 MB (54885788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab1c5b1e67e3b4077d8347087057f3fbfe6af8f802cfc13cfa6cd09e4df0e27e`  
		Last Modified: Thu, 16 Mar 2023 00:58:47 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c90a3a48a8dbb0ebdbf08dfe9e98fa49cb5327e71d363dc79fe82a7d8547b1a`  
		Last Modified: Thu, 16 Mar 2023 00:58:47 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4afddee92301ed98d05269bd72440bf970f13cf4d633bd0a715ea62d1072b0f6`  
		Last Modified: Thu, 16 Mar 2023 00:58:47 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:1.8` - linux; arm variant v7

```console
$ docker pull influxdb@sha256:7281259eb21091766a8ef439b7fbfdfb5c0e02c58f9838e391b26012c16960e8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.0 MB (116981093 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:137547145e2d0395ba59d168f758a35e3769d93009a0a1b1be0a032c0f445d3b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 01 Mar 2023 01:57:45 GMT
ADD file:95a5e178e353a9a46c230d78b0ef83309dd487651c34e47e972ed3dae08ea00b in / 
# Wed, 01 Mar 2023 01:57:45 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 02:32:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:32:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Mar 2023 01:12:02 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 16 Mar 2023 01:12:02 GMT
ENV INFLUXDB_VERSION=1.8.10
# Thu, 16 Mar 2023 01:12:09 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Thu, 16 Mar 2023 01:12:10 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Thu, 16 Mar 2023 01:12:10 GMT
EXPOSE 8086
# Thu, 16 Mar 2023 01:12:10 GMT
VOLUME [/var/lib/influxdb]
# Thu, 16 Mar 2023 01:12:10 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Thu, 16 Mar 2023 01:12:10 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Thu, 16 Mar 2023 01:12:10 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 16 Mar 2023 01:12:10 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:30bee4bd8986478b5a9ecaaaba83525049f0b9b5a63ca88de878568bb6b83292`  
		Last Modified: Wed, 01 Mar 2023 02:02:32 GMT  
		Size: 50.2 MB (50212046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90c2a83a9963df1d0618a3bef56d5f278e39b96940e18347e3575f30d199fb89`  
		Last Modified: Wed, 01 Mar 2023 03:09:13 GMT  
		Size: 4.9 MB (4934569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5b6953f57698d5630bc57919975af4718f7e2eae8d6489d17ceab15dd2ab6e6`  
		Last Modified: Wed, 01 Mar 2023 03:09:13 GMT  
		Size: 10.2 MB (10217796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56125a83a182ac2a7dd2778c8b8d42c237bd1cc20d61d0e029ebc2a0c0ae4a34`  
		Last Modified: Thu, 16 Mar 2023 01:12:21 GMT  
		Size: 1.8 KB (1806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf117165440d382fffb174c87ac625463ad1148e02599368ed886fb0320e0d06`  
		Last Modified: Thu, 16 Mar 2023 01:12:27 GMT  
		Size: 51.6 MB (51613159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9b5c4b3ca8df24519c1c37f742c728f421945384e2f22251c7325d8f55e6913`  
		Last Modified: Thu, 16 Mar 2023 01:12:20 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ed04ffea67135ce8c2fdeaf48d487ccb105879e4544cf35fd056948321eab10`  
		Last Modified: Thu, 16 Mar 2023 01:12:20 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a52a6b46df0f243a7a3926450359dbf57524077090507c19093633981c8cddab`  
		Last Modified: Thu, 16 Mar 2023 01:12:21 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:1.8` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:eb2bf53c91620300960df75dc31a33d2fef8081315ef492af675230ca873a0da
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.0 MB (120963098 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4cd0112a484f28e345f3a592fbf207989be8284f50962e09663f7c39d88a8453`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 01 Mar 2023 02:20:30 GMT
ADD file:a6a1df499d0d5b07fb366d776a11c42ddee6261e2425a921041b38e868192770 in / 
# Wed, 01 Mar 2023 02:20:30 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 02:49:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:49:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 15 Mar 2023 23:40:51 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 15 Mar 2023 23:40:51 GMT
ENV INFLUXDB_VERSION=1.8.10
# Wed, 15 Mar 2023 23:40:55 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Wed, 15 Mar 2023 23:40:56 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Wed, 15 Mar 2023 23:40:56 GMT
EXPOSE 8086
# Wed, 15 Mar 2023 23:40:56 GMT
VOLUME [/var/lib/influxdb]
# Wed, 15 Mar 2023 23:40:56 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Wed, 15 Mar 2023 23:40:57 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Wed, 15 Mar 2023 23:40:57 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 15 Mar 2023 23:40:57 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:0f5fe16b1836feccd4765ac5685fc7a7b9c73445cac94fc595d2ffbc3cb59a7a`  
		Last Modified: Wed, 01 Mar 2023 02:23:53 GMT  
		Size: 53.7 MB (53703215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b8a090f23f28b92f40160bc1a686e3bd5cd4bbd00713a7133631cb2189575f2`  
		Last Modified: Wed, 01 Mar 2023 02:56:19 GMT  
		Size: 5.2 MB (5152682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec29ff8525a3f037f4cc74d2925846a9a8c985469b4ae98fa34099110288987c`  
		Last Modified: Wed, 01 Mar 2023 02:56:19 GMT  
		Size: 10.9 MB (10873588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b013131325e2152822bdcb983af0a7ed52c388d4a9895b9452696ae3f0f6ff0`  
		Last Modified: Wed, 15 Mar 2023 23:42:41 GMT  
		Size: 1.8 KB (1808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e6c517483645f291e5a12abc11190eadb2b7220b366c3925640db8ed5fd0879`  
		Last Modified: Wed, 15 Mar 2023 23:42:46 GMT  
		Size: 51.2 MB (51230087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f16aa915bea5b239472db8db252e3fd246d1a75948c816e3352a821f256b828`  
		Last Modified: Wed, 15 Mar 2023 23:42:41 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80cc5861cf808d7be0a5458cb80d4df9024460ecea35fdb869a2e1ae95f04130`  
		Last Modified: Wed, 15 Mar 2023 23:42:41 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0008ba35232ea0642fe3edfb7ee7317bcd2c60f321d9608edc5f98966b21a175`  
		Last Modified: Wed, 15 Mar 2023 23:42:41 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.8-alpine`

```console
$ docker pull influxdb@sha256:21e0d5823bc4fce17e52dbd29cffb95a166ca158aae355b174673f6b9b443bd3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.8-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:4c9173385396546a26fec70d377d7d390ebd9cb95b5cde2c0bb0ca3877429f49
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.5 MB (59495819 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a5a098361117e7f3d9735ff09a0b81f0ded1ca2ad68912bb6607939da19c8f6`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:42 GMT
ADD file:40887ab7c06977737e63c215c9bd297c0c74de8d12d16ebdf1c3d40ac392f62d in / 
# Sat, 11 Feb 2023 04:46:42 GMT
CMD ["/bin/sh"]
# Mon, 13 Mar 2023 23:20:24 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 16 Mar 2023 00:54:52 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Thu, 16 Mar 2023 00:54:52 GMT
ENV INFLUXDB_VERSION=1.8.10
# Thu, 16 Mar 2023 00:54:57 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     chmod +x /usr/src/influxdb-*/influx              /usr/src/influxdb-*/influx_inspect              /usr/src/influxdb-*/influx_stress              /usr/src/influxdb-*/influxd &&    mv /usr/src/influxdb-*/influx        /usr/src/influxdb-*/influx_inspect        /usr/src/influxdb-*/influx_stress         /usr/src/influxdb-*/influxd        /usr/bin/ &&    gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Thu, 16 Mar 2023 00:54:58 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Thu, 16 Mar 2023 00:54:58 GMT
EXPOSE 8086
# Thu, 16 Mar 2023 00:54:58 GMT
VOLUME [/var/lib/influxdb]
# Thu, 16 Mar 2023 00:54:58 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Thu, 16 Mar 2023 00:54:58 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Thu, 16 Mar 2023 00:54:58 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 16 Mar 2023 00:54:58 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:63b65145d645c1250c391b2d16ebe53b3747c295ca8ba2fcb6b0cf064a4dc21c`  
		Last Modified: Fri, 10 Feb 2023 22:41:31 GMT  
		Size: 3.4 MB (3374446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69b7a2cbfc2f3b3305293d689573f3c9651d6053e5f780a9ba42a4c836d8d6c9`  
		Last Modified: Mon, 13 Mar 2023 23:21:18 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5b0a9605b8bc1c4f3b877c51f73e8d0cc4b02403f8f9d18c276f012b604c038`  
		Last Modified: Thu, 16 Mar 2023 00:59:03 GMT  
		Size: 1.5 MB (1472712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01ee1e350f60a3acd3e7be8caee319e15ac494e7da1f7e0147a1b9236e8ceb39`  
		Last Modified: Thu, 16 Mar 2023 00:59:09 GMT  
		Size: 54.6 MB (54646645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b09053a557d12b97b8b6441e7433c917dab5dbc940a8c7d9d1c0728d52a00ac`  
		Last Modified: Thu, 16 Mar 2023 00:59:02 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0baf052a3360fa2c99ab3a28adda1bf8e1359021cf0c625b46adfa4c3823d67e`  
		Last Modified: Thu, 16 Mar 2023 00:59:03 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d3bc0b58f48b546685d8aff251be8bb3dc8a5bc25fb1d03a99a7b7de06626da`  
		Last Modified: Thu, 16 Mar 2023 00:59:02 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.8-data`

```console
$ docker pull influxdb@sha256:d70a44306e5c0a3774d8cfa978fdb119a9864f1844e3e85d374b4c93584fed64
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.8-data` - linux; amd64

```console
$ docker pull influxdb@sha256:894aa6fecfd3f4a9f87f8d72086e1f8b409a85112afab30ca34b3952602080fb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.8 MB (127797922 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d8e09311c7aa581a42b2643e4b1bb5f9f80decf1c37482ee4e9e087fd9a10dd`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 01 Mar 2023 04:09:45 GMT
ADD file:513c5d5e501279c21a05c1d8b66e5f0b02ee4b27f0b928706d92fd9ce11c1be6 in / 
# Wed, 01 Mar 2023 04:09:46 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 04:42:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 04:42:43 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Mar 2023 00:54:43 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 16 Mar 2023 00:55:02 GMT
ENV INFLUXDB_VERSION=1.8.10-c1.8.10
# Thu, 16 Mar 2023 00:55:08 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-data_${INFLUXDB_VERSION}_amd64.deb*
# Thu, 16 Mar 2023 00:55:08 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Thu, 16 Mar 2023 00:55:08 GMT
EXPOSE 8086
# Thu, 16 Mar 2023 00:55:08 GMT
VOLUME [/var/lib/influxdb]
# Thu, 16 Mar 2023 00:55:09 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Thu, 16 Mar 2023 00:55:09 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Thu, 16 Mar 2023 00:55:09 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 16 Mar 2023 00:55:09 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:32fb02163b6bb519a30f909008e852354dae10bdfd6b34190dbdfe8f15403ea0`  
		Last Modified: Wed, 01 Mar 2023 04:13:58 GMT  
		Size: 55.0 MB (55045922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:167c7feebee855d117e192389484ea8367be1ba84e7ee35f4e5e5663195facbf`  
		Last Modified: Wed, 01 Mar 2023 04:50:15 GMT  
		Size: 5.2 MB (5166586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6dfff1f6f3ddd2194ea0775f199572e8b2d75c38713eef0444d6b1fd0ac7604`  
		Last Modified: Wed, 01 Mar 2023 04:50:15 GMT  
		Size: 10.9 MB (10876729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a90f0187c37c44f2ad04f9d930d40ee0b886fc8d783b914b10a620683739873`  
		Last Modified: Thu, 16 Mar 2023 00:58:47 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4924ec9dc809c1730e7c63922a8e5165926ba2c739cef19170759a0d114745cc`  
		Last Modified: Thu, 16 Mar 2023 00:59:25 GMT  
		Size: 56.7 MB (56705114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8db089179f3c59891770a09bb5a9039cdedf7ffa9452abb94320eca049ff512`  
		Last Modified: Thu, 16 Mar 2023 00:59:18 GMT  
		Size: 242.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1dc009f87cbeaf772c33446fed5360fc8f2edc94895aa45fb77b68751462fd1`  
		Last Modified: Thu, 16 Mar 2023 00:59:18 GMT  
		Size: 252.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8e9a069b786cd091e09d7a579e3d9a77cccb94fa2c895d3724ec882a2c209ef`  
		Last Modified: Thu, 16 Mar 2023 00:59:18 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.8-data-alpine`

```console
$ docker pull influxdb@sha256:261d1655b8cc2dc5404af459329701d0b8245717caadd711036a2e2a36888e36
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.8-data-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:4062b21acf2700f04d0da13c37ecf473b0a75ac6de7b03c3f7fd4c3df2ce7524
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.4 MB (61352861 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f18f1dce311ade7a5bc787e5cc41b48cb635fb2e249b34189c63fbc882712b7`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:42 GMT
ADD file:40887ab7c06977737e63c215c9bd297c0c74de8d12d16ebdf1c3d40ac392f62d in / 
# Sat, 11 Feb 2023 04:46:42 GMT
CMD ["/bin/sh"]
# Mon, 13 Mar 2023 23:20:24 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 16 Mar 2023 00:54:52 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Thu, 16 Mar 2023 00:55:13 GMT
ENV INFLUXDB_VERSION=1.8.10-c1.8.10
# Thu, 16 Mar 2023 00:55:21 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Thu, 16 Mar 2023 00:55:21 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Thu, 16 Mar 2023 00:55:21 GMT
EXPOSE 8086
# Thu, 16 Mar 2023 00:55:22 GMT
VOLUME [/var/lib/influxdb]
# Thu, 16 Mar 2023 00:55:22 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Thu, 16 Mar 2023 00:55:22 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Thu, 16 Mar 2023 00:55:22 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 16 Mar 2023 00:55:22 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:63b65145d645c1250c391b2d16ebe53b3747c295ca8ba2fcb6b0cf064a4dc21c`  
		Last Modified: Fri, 10 Feb 2023 22:41:31 GMT  
		Size: 3.4 MB (3374446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69b7a2cbfc2f3b3305293d689573f3c9651d6053e5f780a9ba42a4c836d8d6c9`  
		Last Modified: Mon, 13 Mar 2023 23:21:18 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5b0a9605b8bc1c4f3b877c51f73e8d0cc4b02403f8f9d18c276f012b604c038`  
		Last Modified: Thu, 16 Mar 2023 00:59:03 GMT  
		Size: 1.5 MB (1472712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61bad459754475dfd8621019d72d1bd32ca2b9be86fb936ab64308888ee0073a`  
		Last Modified: Thu, 16 Mar 2023 00:59:43 GMT  
		Size: 56.5 MB (56503629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0fdd4464dd3872545334e618c0323eef93811cc622aa2409dc50a984d042034`  
		Last Modified: Thu, 16 Mar 2023 00:59:36 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aeb71d6736a13e612d2dc8a667133647ee9099895936ffa258569114cc772086`  
		Last Modified: Thu, 16 Mar 2023 00:59:36 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a34548e01d2f855e58fb7674a9102ca3878dda447d78e6060033d7827d27589f`  
		Last Modified: Thu, 16 Mar 2023 00:59:36 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.8-meta`

```console
$ docker pull influxdb@sha256:f2cc8820fb7d417f8284255f4edf73326e75b1b1f8b3f0db0a869f5fd93cb5a6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.8-meta` - linux; amd64

```console
$ docker pull influxdb@sha256:9949b62ba091bf1e0c6d555a0d62f9c0e3f111d34468c12790701841607c2054
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.5 MB (94504419 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c421d7d950d23de67391a03fa05758737a2990ed39e0371b765c58cfe8d49d27`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Wed, 01 Mar 2023 04:09:45 GMT
ADD file:513c5d5e501279c21a05c1d8b66e5f0b02ee4b27f0b928706d92fd9ce11c1be6 in / 
# Wed, 01 Mar 2023 04:09:46 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 04:42:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 04:42:43 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Mar 2023 00:54:43 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 16 Mar 2023 00:55:02 GMT
ENV INFLUXDB_VERSION=1.8.10-c1.8.10
# Thu, 16 Mar 2023 00:55:28 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-meta_${INFLUXDB_VERSION}_amd64.deb*
# Thu, 16 Mar 2023 00:55:28 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Thu, 16 Mar 2023 00:55:28 GMT
EXPOSE 8091
# Thu, 16 Mar 2023 00:55:28 GMT
VOLUME [/var/lib/influxdb]
# Thu, 16 Mar 2023 00:55:28 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Thu, 16 Mar 2023 00:55:28 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 16 Mar 2023 00:55:28 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:32fb02163b6bb519a30f909008e852354dae10bdfd6b34190dbdfe8f15403ea0`  
		Last Modified: Wed, 01 Mar 2023 04:13:58 GMT  
		Size: 55.0 MB (55045922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:167c7feebee855d117e192389484ea8367be1ba84e7ee35f4e5e5663195facbf`  
		Last Modified: Wed, 01 Mar 2023 04:50:15 GMT  
		Size: 5.2 MB (5166586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6dfff1f6f3ddd2194ea0775f199572e8b2d75c38713eef0444d6b1fd0ac7604`  
		Last Modified: Wed, 01 Mar 2023 04:50:15 GMT  
		Size: 10.9 MB (10876729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a90f0187c37c44f2ad04f9d930d40ee0b886fc8d783b914b10a620683739873`  
		Last Modified: Thu, 16 Mar 2023 00:58:47 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4da79a67cea3e0423fbd017b960736725ee1a9d645259e5e116f7b80f65e3ffb`  
		Last Modified: Thu, 16 Mar 2023 00:59:57 GMT  
		Size: 23.4 MB (23412815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:467317e0fc8b77b1ea7e470e0bb2acd70c9fbc0666761d3a46c639cf1a4bd57a`  
		Last Modified: Thu, 16 Mar 2023 00:59:54 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2476469e17a280c1a07bbbe66a0c405e79e95fe2a45baf4f259f8d0942389de`  
		Last Modified: Thu, 16 Mar 2023 00:59:54 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.8-meta-alpine`

```console
$ docker pull influxdb@sha256:b332bb7ba17ea35119db932b2f532aba89d7cf9008f3c53ca0cb572e1b465492
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.8-meta-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:d47c4b7d73fe4dab3506b30191fb878ff88e235e33a57ec221fc5243f1de5229
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.1 MB (28141489 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3401b5ccad79633922a0201457f58a455907b6280a3aa68c53a079dff96d0220`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:42 GMT
ADD file:40887ab7c06977737e63c215c9bd297c0c74de8d12d16ebdf1c3d40ac392f62d in / 
# Sat, 11 Feb 2023 04:46:42 GMT
CMD ["/bin/sh"]
# Mon, 13 Mar 2023 23:20:24 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 16 Mar 2023 00:54:52 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Thu, 16 Mar 2023 00:55:13 GMT
ENV INFLUXDB_VERSION=1.8.10-c1.8.10
# Thu, 16 Mar 2023 00:55:36 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb-meta.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Thu, 16 Mar 2023 00:55:37 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Thu, 16 Mar 2023 00:55:37 GMT
EXPOSE 8091
# Thu, 16 Mar 2023 00:55:37 GMT
VOLUME [/var/lib/influxdb]
# Thu, 16 Mar 2023 00:55:37 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Thu, 16 Mar 2023 00:55:37 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 16 Mar 2023 00:55:37 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:63b65145d645c1250c391b2d16ebe53b3747c295ca8ba2fcb6b0cf064a4dc21c`  
		Last Modified: Fri, 10 Feb 2023 22:41:31 GMT  
		Size: 3.4 MB (3374446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69b7a2cbfc2f3b3305293d689573f3c9651d6053e5f780a9ba42a4c836d8d6c9`  
		Last Modified: Mon, 13 Mar 2023 23:21:18 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5b0a9605b8bc1c4f3b877c51f73e8d0cc4b02403f8f9d18c276f012b604c038`  
		Last Modified: Thu, 16 Mar 2023 00:59:03 GMT  
		Size: 1.5 MB (1472712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9765a5f3bc0d01c3d573bd99fa2c9c6b278d99a9738cd4da9bf3dadb610b22ce`  
		Last Modified: Thu, 16 Mar 2023 01:00:19 GMT  
		Size: 23.3 MB (23293461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ca8edc79b71d358c7eeb599969087beb75b17b94b72e37e85056251578cf1ac`  
		Last Modified: Thu, 16 Mar 2023 01:00:16 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9ab6bb76bc121d5c9b2d774be4fcc78dd5b2b36148a3599db35a72a0861a51f`  
		Last Modified: Thu, 16 Mar 2023 01:00:16 GMT  
		Size: 373.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.8.10`

```console
$ docker pull influxdb@sha256:dfdff063429b612af16a09a4d64c0971b39427ca8def47df9aa25dfadb17a109
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `influxdb:1.8.10` - linux; amd64

```console
$ docker pull influxdb@sha256:62058532a6a46c42b7abe920ee9f37e22bcaf5755a7c6c1de4c2538d2c412bb8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.0 MB (125978540 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2dfef349b0709348b4756b8deeb072d87e085cb278c3d1b300a096aa5645f7ce`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 01 Mar 2023 04:09:45 GMT
ADD file:513c5d5e501279c21a05c1d8b66e5f0b02ee4b27f0b928706d92fd9ce11c1be6 in / 
# Wed, 01 Mar 2023 04:09:46 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 04:42:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 04:42:43 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Mar 2023 00:54:43 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 16 Mar 2023 00:54:43 GMT
ENV INFLUXDB_VERSION=1.8.10
# Thu, 16 Mar 2023 00:54:47 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Thu, 16 Mar 2023 00:54:47 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Thu, 16 Mar 2023 00:54:47 GMT
EXPOSE 8086
# Thu, 16 Mar 2023 00:54:47 GMT
VOLUME [/var/lib/influxdb]
# Thu, 16 Mar 2023 00:54:47 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Thu, 16 Mar 2023 00:54:48 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Thu, 16 Mar 2023 00:54:48 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 16 Mar 2023 00:54:48 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:32fb02163b6bb519a30f909008e852354dae10bdfd6b34190dbdfe8f15403ea0`  
		Last Modified: Wed, 01 Mar 2023 04:13:58 GMT  
		Size: 55.0 MB (55045922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:167c7feebee855d117e192389484ea8367be1ba84e7ee35f4e5e5663195facbf`  
		Last Modified: Wed, 01 Mar 2023 04:50:15 GMT  
		Size: 5.2 MB (5166586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6dfff1f6f3ddd2194ea0775f199572e8b2d75c38713eef0444d6b1fd0ac7604`  
		Last Modified: Wed, 01 Mar 2023 04:50:15 GMT  
		Size: 10.9 MB (10876729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a90f0187c37c44f2ad04f9d930d40ee0b886fc8d783b914b10a620683739873`  
		Last Modified: Thu, 16 Mar 2023 00:58:47 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c128af0cbea60d53679d68899e21837db22b0a33bcc3d784bc3078ec82a21b14`  
		Last Modified: Thu, 16 Mar 2023 00:58:54 GMT  
		Size: 54.9 MB (54885788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab1c5b1e67e3b4077d8347087057f3fbfe6af8f802cfc13cfa6cd09e4df0e27e`  
		Last Modified: Thu, 16 Mar 2023 00:58:47 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c90a3a48a8dbb0ebdbf08dfe9e98fa49cb5327e71d363dc79fe82a7d8547b1a`  
		Last Modified: Thu, 16 Mar 2023 00:58:47 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4afddee92301ed98d05269bd72440bf970f13cf4d633bd0a715ea62d1072b0f6`  
		Last Modified: Thu, 16 Mar 2023 00:58:47 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:1.8.10` - linux; arm variant v7

```console
$ docker pull influxdb@sha256:7281259eb21091766a8ef439b7fbfdfb5c0e02c58f9838e391b26012c16960e8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.0 MB (116981093 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:137547145e2d0395ba59d168f758a35e3769d93009a0a1b1be0a032c0f445d3b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 01 Mar 2023 01:57:45 GMT
ADD file:95a5e178e353a9a46c230d78b0ef83309dd487651c34e47e972ed3dae08ea00b in / 
# Wed, 01 Mar 2023 01:57:45 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 02:32:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:32:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Mar 2023 01:12:02 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 16 Mar 2023 01:12:02 GMT
ENV INFLUXDB_VERSION=1.8.10
# Thu, 16 Mar 2023 01:12:09 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Thu, 16 Mar 2023 01:12:10 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Thu, 16 Mar 2023 01:12:10 GMT
EXPOSE 8086
# Thu, 16 Mar 2023 01:12:10 GMT
VOLUME [/var/lib/influxdb]
# Thu, 16 Mar 2023 01:12:10 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Thu, 16 Mar 2023 01:12:10 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Thu, 16 Mar 2023 01:12:10 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 16 Mar 2023 01:12:10 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:30bee4bd8986478b5a9ecaaaba83525049f0b9b5a63ca88de878568bb6b83292`  
		Last Modified: Wed, 01 Mar 2023 02:02:32 GMT  
		Size: 50.2 MB (50212046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90c2a83a9963df1d0618a3bef56d5f278e39b96940e18347e3575f30d199fb89`  
		Last Modified: Wed, 01 Mar 2023 03:09:13 GMT  
		Size: 4.9 MB (4934569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5b6953f57698d5630bc57919975af4718f7e2eae8d6489d17ceab15dd2ab6e6`  
		Last Modified: Wed, 01 Mar 2023 03:09:13 GMT  
		Size: 10.2 MB (10217796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56125a83a182ac2a7dd2778c8b8d42c237bd1cc20d61d0e029ebc2a0c0ae4a34`  
		Last Modified: Thu, 16 Mar 2023 01:12:21 GMT  
		Size: 1.8 KB (1806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf117165440d382fffb174c87ac625463ad1148e02599368ed886fb0320e0d06`  
		Last Modified: Thu, 16 Mar 2023 01:12:27 GMT  
		Size: 51.6 MB (51613159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9b5c4b3ca8df24519c1c37f742c728f421945384e2f22251c7325d8f55e6913`  
		Last Modified: Thu, 16 Mar 2023 01:12:20 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ed04ffea67135ce8c2fdeaf48d487ccb105879e4544cf35fd056948321eab10`  
		Last Modified: Thu, 16 Mar 2023 01:12:20 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a52a6b46df0f243a7a3926450359dbf57524077090507c19093633981c8cddab`  
		Last Modified: Thu, 16 Mar 2023 01:12:21 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:1.8.10` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:eb2bf53c91620300960df75dc31a33d2fef8081315ef492af675230ca873a0da
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.0 MB (120963098 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4cd0112a484f28e345f3a592fbf207989be8284f50962e09663f7c39d88a8453`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 01 Mar 2023 02:20:30 GMT
ADD file:a6a1df499d0d5b07fb366d776a11c42ddee6261e2425a921041b38e868192770 in / 
# Wed, 01 Mar 2023 02:20:30 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 02:49:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:49:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 15 Mar 2023 23:40:51 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 15 Mar 2023 23:40:51 GMT
ENV INFLUXDB_VERSION=1.8.10
# Wed, 15 Mar 2023 23:40:55 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Wed, 15 Mar 2023 23:40:56 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Wed, 15 Mar 2023 23:40:56 GMT
EXPOSE 8086
# Wed, 15 Mar 2023 23:40:56 GMT
VOLUME [/var/lib/influxdb]
# Wed, 15 Mar 2023 23:40:56 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Wed, 15 Mar 2023 23:40:57 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Wed, 15 Mar 2023 23:40:57 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 15 Mar 2023 23:40:57 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:0f5fe16b1836feccd4765ac5685fc7a7b9c73445cac94fc595d2ffbc3cb59a7a`  
		Last Modified: Wed, 01 Mar 2023 02:23:53 GMT  
		Size: 53.7 MB (53703215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b8a090f23f28b92f40160bc1a686e3bd5cd4bbd00713a7133631cb2189575f2`  
		Last Modified: Wed, 01 Mar 2023 02:56:19 GMT  
		Size: 5.2 MB (5152682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec29ff8525a3f037f4cc74d2925846a9a8c985469b4ae98fa34099110288987c`  
		Last Modified: Wed, 01 Mar 2023 02:56:19 GMT  
		Size: 10.9 MB (10873588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b013131325e2152822bdcb983af0a7ed52c388d4a9895b9452696ae3f0f6ff0`  
		Last Modified: Wed, 15 Mar 2023 23:42:41 GMT  
		Size: 1.8 KB (1808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e6c517483645f291e5a12abc11190eadb2b7220b366c3925640db8ed5fd0879`  
		Last Modified: Wed, 15 Mar 2023 23:42:46 GMT  
		Size: 51.2 MB (51230087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f16aa915bea5b239472db8db252e3fd246d1a75948c816e3352a821f256b828`  
		Last Modified: Wed, 15 Mar 2023 23:42:41 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80cc5861cf808d7be0a5458cb80d4df9024460ecea35fdb869a2e1ae95f04130`  
		Last Modified: Wed, 15 Mar 2023 23:42:41 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0008ba35232ea0642fe3edfb7ee7317bcd2c60f321d9608edc5f98966b21a175`  
		Last Modified: Wed, 15 Mar 2023 23:42:41 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.8.10-alpine`

```console
$ docker pull influxdb@sha256:21e0d5823bc4fce17e52dbd29cffb95a166ca158aae355b174673f6b9b443bd3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.8.10-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:4c9173385396546a26fec70d377d7d390ebd9cb95b5cde2c0bb0ca3877429f49
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.5 MB (59495819 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a5a098361117e7f3d9735ff09a0b81f0ded1ca2ad68912bb6607939da19c8f6`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:42 GMT
ADD file:40887ab7c06977737e63c215c9bd297c0c74de8d12d16ebdf1c3d40ac392f62d in / 
# Sat, 11 Feb 2023 04:46:42 GMT
CMD ["/bin/sh"]
# Mon, 13 Mar 2023 23:20:24 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 16 Mar 2023 00:54:52 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Thu, 16 Mar 2023 00:54:52 GMT
ENV INFLUXDB_VERSION=1.8.10
# Thu, 16 Mar 2023 00:54:57 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     chmod +x /usr/src/influxdb-*/influx              /usr/src/influxdb-*/influx_inspect              /usr/src/influxdb-*/influx_stress              /usr/src/influxdb-*/influxd &&    mv /usr/src/influxdb-*/influx        /usr/src/influxdb-*/influx_inspect        /usr/src/influxdb-*/influx_stress         /usr/src/influxdb-*/influxd        /usr/bin/ &&    gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Thu, 16 Mar 2023 00:54:58 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Thu, 16 Mar 2023 00:54:58 GMT
EXPOSE 8086
# Thu, 16 Mar 2023 00:54:58 GMT
VOLUME [/var/lib/influxdb]
# Thu, 16 Mar 2023 00:54:58 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Thu, 16 Mar 2023 00:54:58 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Thu, 16 Mar 2023 00:54:58 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 16 Mar 2023 00:54:58 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:63b65145d645c1250c391b2d16ebe53b3747c295ca8ba2fcb6b0cf064a4dc21c`  
		Last Modified: Fri, 10 Feb 2023 22:41:31 GMT  
		Size: 3.4 MB (3374446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69b7a2cbfc2f3b3305293d689573f3c9651d6053e5f780a9ba42a4c836d8d6c9`  
		Last Modified: Mon, 13 Mar 2023 23:21:18 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5b0a9605b8bc1c4f3b877c51f73e8d0cc4b02403f8f9d18c276f012b604c038`  
		Last Modified: Thu, 16 Mar 2023 00:59:03 GMT  
		Size: 1.5 MB (1472712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01ee1e350f60a3acd3e7be8caee319e15ac494e7da1f7e0147a1b9236e8ceb39`  
		Last Modified: Thu, 16 Mar 2023 00:59:09 GMT  
		Size: 54.6 MB (54646645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b09053a557d12b97b8b6441e7433c917dab5dbc940a8c7d9d1c0728d52a00ac`  
		Last Modified: Thu, 16 Mar 2023 00:59:02 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0baf052a3360fa2c99ab3a28adda1bf8e1359021cf0c625b46adfa4c3823d67e`  
		Last Modified: Thu, 16 Mar 2023 00:59:03 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d3bc0b58f48b546685d8aff251be8bb3dc8a5bc25fb1d03a99a7b7de06626da`  
		Last Modified: Thu, 16 Mar 2023 00:59:02 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.8.10-data`

```console
$ docker pull influxdb@sha256:d70a44306e5c0a3774d8cfa978fdb119a9864f1844e3e85d374b4c93584fed64
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.8.10-data` - linux; amd64

```console
$ docker pull influxdb@sha256:894aa6fecfd3f4a9f87f8d72086e1f8b409a85112afab30ca34b3952602080fb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.8 MB (127797922 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d8e09311c7aa581a42b2643e4b1bb5f9f80decf1c37482ee4e9e087fd9a10dd`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 01 Mar 2023 04:09:45 GMT
ADD file:513c5d5e501279c21a05c1d8b66e5f0b02ee4b27f0b928706d92fd9ce11c1be6 in / 
# Wed, 01 Mar 2023 04:09:46 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 04:42:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 04:42:43 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Mar 2023 00:54:43 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 16 Mar 2023 00:55:02 GMT
ENV INFLUXDB_VERSION=1.8.10-c1.8.10
# Thu, 16 Mar 2023 00:55:08 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-data_${INFLUXDB_VERSION}_amd64.deb*
# Thu, 16 Mar 2023 00:55:08 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Thu, 16 Mar 2023 00:55:08 GMT
EXPOSE 8086
# Thu, 16 Mar 2023 00:55:08 GMT
VOLUME [/var/lib/influxdb]
# Thu, 16 Mar 2023 00:55:09 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Thu, 16 Mar 2023 00:55:09 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Thu, 16 Mar 2023 00:55:09 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 16 Mar 2023 00:55:09 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:32fb02163b6bb519a30f909008e852354dae10bdfd6b34190dbdfe8f15403ea0`  
		Last Modified: Wed, 01 Mar 2023 04:13:58 GMT  
		Size: 55.0 MB (55045922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:167c7feebee855d117e192389484ea8367be1ba84e7ee35f4e5e5663195facbf`  
		Last Modified: Wed, 01 Mar 2023 04:50:15 GMT  
		Size: 5.2 MB (5166586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6dfff1f6f3ddd2194ea0775f199572e8b2d75c38713eef0444d6b1fd0ac7604`  
		Last Modified: Wed, 01 Mar 2023 04:50:15 GMT  
		Size: 10.9 MB (10876729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a90f0187c37c44f2ad04f9d930d40ee0b886fc8d783b914b10a620683739873`  
		Last Modified: Thu, 16 Mar 2023 00:58:47 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4924ec9dc809c1730e7c63922a8e5165926ba2c739cef19170759a0d114745cc`  
		Last Modified: Thu, 16 Mar 2023 00:59:25 GMT  
		Size: 56.7 MB (56705114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8db089179f3c59891770a09bb5a9039cdedf7ffa9452abb94320eca049ff512`  
		Last Modified: Thu, 16 Mar 2023 00:59:18 GMT  
		Size: 242.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1dc009f87cbeaf772c33446fed5360fc8f2edc94895aa45fb77b68751462fd1`  
		Last Modified: Thu, 16 Mar 2023 00:59:18 GMT  
		Size: 252.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8e9a069b786cd091e09d7a579e3d9a77cccb94fa2c895d3724ec882a2c209ef`  
		Last Modified: Thu, 16 Mar 2023 00:59:18 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.8.10-data-alpine`

```console
$ docker pull influxdb@sha256:261d1655b8cc2dc5404af459329701d0b8245717caadd711036a2e2a36888e36
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.8.10-data-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:4062b21acf2700f04d0da13c37ecf473b0a75ac6de7b03c3f7fd4c3df2ce7524
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.4 MB (61352861 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f18f1dce311ade7a5bc787e5cc41b48cb635fb2e249b34189c63fbc882712b7`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:42 GMT
ADD file:40887ab7c06977737e63c215c9bd297c0c74de8d12d16ebdf1c3d40ac392f62d in / 
# Sat, 11 Feb 2023 04:46:42 GMT
CMD ["/bin/sh"]
# Mon, 13 Mar 2023 23:20:24 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 16 Mar 2023 00:54:52 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Thu, 16 Mar 2023 00:55:13 GMT
ENV INFLUXDB_VERSION=1.8.10-c1.8.10
# Thu, 16 Mar 2023 00:55:21 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Thu, 16 Mar 2023 00:55:21 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Thu, 16 Mar 2023 00:55:21 GMT
EXPOSE 8086
# Thu, 16 Mar 2023 00:55:22 GMT
VOLUME [/var/lib/influxdb]
# Thu, 16 Mar 2023 00:55:22 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Thu, 16 Mar 2023 00:55:22 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Thu, 16 Mar 2023 00:55:22 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 16 Mar 2023 00:55:22 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:63b65145d645c1250c391b2d16ebe53b3747c295ca8ba2fcb6b0cf064a4dc21c`  
		Last Modified: Fri, 10 Feb 2023 22:41:31 GMT  
		Size: 3.4 MB (3374446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69b7a2cbfc2f3b3305293d689573f3c9651d6053e5f780a9ba42a4c836d8d6c9`  
		Last Modified: Mon, 13 Mar 2023 23:21:18 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5b0a9605b8bc1c4f3b877c51f73e8d0cc4b02403f8f9d18c276f012b604c038`  
		Last Modified: Thu, 16 Mar 2023 00:59:03 GMT  
		Size: 1.5 MB (1472712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61bad459754475dfd8621019d72d1bd32ca2b9be86fb936ab64308888ee0073a`  
		Last Modified: Thu, 16 Mar 2023 00:59:43 GMT  
		Size: 56.5 MB (56503629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0fdd4464dd3872545334e618c0323eef93811cc622aa2409dc50a984d042034`  
		Last Modified: Thu, 16 Mar 2023 00:59:36 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aeb71d6736a13e612d2dc8a667133647ee9099895936ffa258569114cc772086`  
		Last Modified: Thu, 16 Mar 2023 00:59:36 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a34548e01d2f855e58fb7674a9102ca3878dda447d78e6060033d7827d27589f`  
		Last Modified: Thu, 16 Mar 2023 00:59:36 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.8.10-meta`

```console
$ docker pull influxdb@sha256:f2cc8820fb7d417f8284255f4edf73326e75b1b1f8b3f0db0a869f5fd93cb5a6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.8.10-meta` - linux; amd64

```console
$ docker pull influxdb@sha256:9949b62ba091bf1e0c6d555a0d62f9c0e3f111d34468c12790701841607c2054
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.5 MB (94504419 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c421d7d950d23de67391a03fa05758737a2990ed39e0371b765c58cfe8d49d27`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Wed, 01 Mar 2023 04:09:45 GMT
ADD file:513c5d5e501279c21a05c1d8b66e5f0b02ee4b27f0b928706d92fd9ce11c1be6 in / 
# Wed, 01 Mar 2023 04:09:46 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 04:42:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 04:42:43 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Mar 2023 00:54:43 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 16 Mar 2023 00:55:02 GMT
ENV INFLUXDB_VERSION=1.8.10-c1.8.10
# Thu, 16 Mar 2023 00:55:28 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-meta_${INFLUXDB_VERSION}_amd64.deb*
# Thu, 16 Mar 2023 00:55:28 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Thu, 16 Mar 2023 00:55:28 GMT
EXPOSE 8091
# Thu, 16 Mar 2023 00:55:28 GMT
VOLUME [/var/lib/influxdb]
# Thu, 16 Mar 2023 00:55:28 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Thu, 16 Mar 2023 00:55:28 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 16 Mar 2023 00:55:28 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:32fb02163b6bb519a30f909008e852354dae10bdfd6b34190dbdfe8f15403ea0`  
		Last Modified: Wed, 01 Mar 2023 04:13:58 GMT  
		Size: 55.0 MB (55045922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:167c7feebee855d117e192389484ea8367be1ba84e7ee35f4e5e5663195facbf`  
		Last Modified: Wed, 01 Mar 2023 04:50:15 GMT  
		Size: 5.2 MB (5166586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6dfff1f6f3ddd2194ea0775f199572e8b2d75c38713eef0444d6b1fd0ac7604`  
		Last Modified: Wed, 01 Mar 2023 04:50:15 GMT  
		Size: 10.9 MB (10876729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a90f0187c37c44f2ad04f9d930d40ee0b886fc8d783b914b10a620683739873`  
		Last Modified: Thu, 16 Mar 2023 00:58:47 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4da79a67cea3e0423fbd017b960736725ee1a9d645259e5e116f7b80f65e3ffb`  
		Last Modified: Thu, 16 Mar 2023 00:59:57 GMT  
		Size: 23.4 MB (23412815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:467317e0fc8b77b1ea7e470e0bb2acd70c9fbc0666761d3a46c639cf1a4bd57a`  
		Last Modified: Thu, 16 Mar 2023 00:59:54 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2476469e17a280c1a07bbbe66a0c405e79e95fe2a45baf4f259f8d0942389de`  
		Last Modified: Thu, 16 Mar 2023 00:59:54 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.8.10-meta-alpine`

```console
$ docker pull influxdb@sha256:b332bb7ba17ea35119db932b2f532aba89d7cf9008f3c53ca0cb572e1b465492
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.8.10-meta-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:d47c4b7d73fe4dab3506b30191fb878ff88e235e33a57ec221fc5243f1de5229
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.1 MB (28141489 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3401b5ccad79633922a0201457f58a455907b6280a3aa68c53a079dff96d0220`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:42 GMT
ADD file:40887ab7c06977737e63c215c9bd297c0c74de8d12d16ebdf1c3d40ac392f62d in / 
# Sat, 11 Feb 2023 04:46:42 GMT
CMD ["/bin/sh"]
# Mon, 13 Mar 2023 23:20:24 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 16 Mar 2023 00:54:52 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Thu, 16 Mar 2023 00:55:13 GMT
ENV INFLUXDB_VERSION=1.8.10-c1.8.10
# Thu, 16 Mar 2023 00:55:36 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb-meta.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Thu, 16 Mar 2023 00:55:37 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Thu, 16 Mar 2023 00:55:37 GMT
EXPOSE 8091
# Thu, 16 Mar 2023 00:55:37 GMT
VOLUME [/var/lib/influxdb]
# Thu, 16 Mar 2023 00:55:37 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Thu, 16 Mar 2023 00:55:37 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 16 Mar 2023 00:55:37 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:63b65145d645c1250c391b2d16ebe53b3747c295ca8ba2fcb6b0cf064a4dc21c`  
		Last Modified: Fri, 10 Feb 2023 22:41:31 GMT  
		Size: 3.4 MB (3374446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69b7a2cbfc2f3b3305293d689573f3c9651d6053e5f780a9ba42a4c836d8d6c9`  
		Last Modified: Mon, 13 Mar 2023 23:21:18 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5b0a9605b8bc1c4f3b877c51f73e8d0cc4b02403f8f9d18c276f012b604c038`  
		Last Modified: Thu, 16 Mar 2023 00:59:03 GMT  
		Size: 1.5 MB (1472712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9765a5f3bc0d01c3d573bd99fa2c9c6b278d99a9738cd4da9bf3dadb610b22ce`  
		Last Modified: Thu, 16 Mar 2023 01:00:19 GMT  
		Size: 23.3 MB (23293461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ca8edc79b71d358c7eeb599969087beb75b17b94b72e37e85056251578cf1ac`  
		Last Modified: Thu, 16 Mar 2023 01:00:16 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9ab6bb76bc121d5c9b2d774be4fcc78dd5b2b36148a3599db35a72a0861a51f`  
		Last Modified: Thu, 16 Mar 2023 01:00:16 GMT  
		Size: 373.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.9-data`

```console
$ docker pull influxdb@sha256:38bd41f3e323ee0115ecbe8264d1c2bc201c6fdb58fad417f72c8418bc15f3c4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.9-data` - linux; amd64

```console
$ docker pull influxdb@sha256:487cabb4dd16bf501ac4e07644ce3bb82a4c435118285e96cbf8643f9d34cbab
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **103.9 MB (103949152 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd026e7f0d602c645cc44cc05f8a12dc9a1490d9b3072f60df8e08db25498361`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 01 Mar 2023 04:09:45 GMT
ADD file:513c5d5e501279c21a05c1d8b66e5f0b02ee4b27f0b928706d92fd9ce11c1be6 in / 
# Wed, 01 Mar 2023 04:09:46 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 04:42:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 04:42:43 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Mar 2023 00:54:43 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 16 Mar 2023 00:55:40 GMT
ENV INFLUXDB_VERSION=1.9.9-c1.9.9
# Thu, 16 Mar 2023 00:55:44 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-data_${INFLUXDB_VERSION}_amd64.deb*
# Thu, 16 Mar 2023 00:55:44 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Thu, 16 Mar 2023 00:55:44 GMT
EXPOSE 8086
# Thu, 16 Mar 2023 00:55:44 GMT
VOLUME [/var/lib/influxdb]
# Thu, 16 Mar 2023 00:55:44 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Thu, 16 Mar 2023 00:55:44 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Thu, 16 Mar 2023 00:55:44 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 16 Mar 2023 00:55:45 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:32fb02163b6bb519a30f909008e852354dae10bdfd6b34190dbdfe8f15403ea0`  
		Last Modified: Wed, 01 Mar 2023 04:13:58 GMT  
		Size: 55.0 MB (55045922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:167c7feebee855d117e192389484ea8367be1ba84e7ee35f4e5e5663195facbf`  
		Last Modified: Wed, 01 Mar 2023 04:50:15 GMT  
		Size: 5.2 MB (5166586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6dfff1f6f3ddd2194ea0775f199572e8b2d75c38713eef0444d6b1fd0ac7604`  
		Last Modified: Wed, 01 Mar 2023 04:50:15 GMT  
		Size: 10.9 MB (10876729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a90f0187c37c44f2ad04f9d930d40ee0b886fc8d783b914b10a620683739873`  
		Last Modified: Thu, 16 Mar 2023 00:58:47 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:070b7597564eefee299403e56cb3bdabea7775a74edd530e72271a17044dd49f`  
		Last Modified: Thu, 16 Mar 2023 01:00:35 GMT  
		Size: 32.9 MB (32856344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59b018312f678fb3801e0c6414cf6d1ff76326856c42ef75541ce88a080724ed`  
		Last Modified: Thu, 16 Mar 2023 01:00:30 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f87e0de7ba6781751725d7580b29bd74789bf7ab7b79c0cb54db93329c8ea0a7`  
		Last Modified: Thu, 16 Mar 2023 01:00:30 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2e3792499531b5a00bb695cbe9115f2bb8049e3810a92df4fa0a5587b63c519`  
		Last Modified: Thu, 16 Mar 2023 01:00:30 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.9-data-alpine`

```console
$ docker pull influxdb@sha256:1dc0dc45dfb8565a191482ff12f8ef21abf086d7b3ea80afed3e2760d3b6cfd4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.9-data-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:180f5debe1662fc59e945ce8595ca6c39d50109358c02dc302035a9c6596d628
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.7 MB (37661708 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8379824b3de5e2abeb7c1e053e7342d7f44e2d330dfda7437e77d7f0c1532159`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:42 GMT
ADD file:40887ab7c06977737e63c215c9bd297c0c74de8d12d16ebdf1c3d40ac392f62d in / 
# Sat, 11 Feb 2023 04:46:42 GMT
CMD ["/bin/sh"]
# Mon, 13 Mar 2023 23:20:24 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 16 Mar 2023 00:54:52 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Thu, 16 Mar 2023 00:55:47 GMT
ENV INFLUXDB_VERSION=1.9.9-c1.9.9
# Thu, 16 Mar 2023 00:55:53 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/etc/influxdb/influxdb.conf &&     chmod +x /usr/src/influxdb-*/usr/bin/* &&     cp -a /usr/src/influxdb-*/usr/bin/. /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Thu, 16 Mar 2023 00:55:53 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Thu, 16 Mar 2023 00:55:53 GMT
EXPOSE 8086
# Thu, 16 Mar 2023 00:55:54 GMT
VOLUME [/var/lib/influxdb]
# Thu, 16 Mar 2023 00:55:54 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Thu, 16 Mar 2023 00:55:54 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Thu, 16 Mar 2023 00:55:54 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 16 Mar 2023 00:55:54 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:63b65145d645c1250c391b2d16ebe53b3747c295ca8ba2fcb6b0cf064a4dc21c`  
		Last Modified: Fri, 10 Feb 2023 22:41:31 GMT  
		Size: 3.4 MB (3374446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69b7a2cbfc2f3b3305293d689573f3c9651d6053e5f780a9ba42a4c836d8d6c9`  
		Last Modified: Mon, 13 Mar 2023 23:21:18 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5b0a9605b8bc1c4f3b877c51f73e8d0cc4b02403f8f9d18c276f012b604c038`  
		Last Modified: Thu, 16 Mar 2023 00:59:03 GMT  
		Size: 1.5 MB (1472712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62ba7c0784ed61eca939fe14f9fca623589151b853f30334f72ca0e9b36659a9`  
		Last Modified: Thu, 16 Mar 2023 01:00:50 GMT  
		Size: 32.8 MB (32812476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:433821cacc6957d02fa7385c77f6321fa782bdf57beec08b87215f22a4421531`  
		Last Modified: Thu, 16 Mar 2023 01:00:45 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0083dacac064d2fe5ef51b7c30236bf749162d05e1220935457f408b1c152e10`  
		Last Modified: Thu, 16 Mar 2023 01:00:45 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f714b29738f1da6463e2f95941fbd4f0f54279ddd7b6d9ca0b1f28cfcd072a58`  
		Last Modified: Thu, 16 Mar 2023 01:00:45 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.9-meta`

```console
$ docker pull influxdb@sha256:b1df3ae80c7bd334c4a8b6e2c740e9e6b9bcef3a13a9c3c65fc5649b82b0f2f2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.9-meta` - linux; amd64

```console
$ docker pull influxdb@sha256:490acef35891290e3e46536d01cf5021644d5bf720008333c91ed463004c8a15
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.5 MB (83511617 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d4a13fb1976426aaa2da3c36ac74e5856c68a8a4ae2c415dbb5cb527a24dca5`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Wed, 01 Mar 2023 04:09:45 GMT
ADD file:513c5d5e501279c21a05c1d8b66e5f0b02ee4b27f0b928706d92fd9ce11c1be6 in / 
# Wed, 01 Mar 2023 04:09:46 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 04:42:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 04:42:43 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Mar 2023 00:54:43 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 16 Mar 2023 00:55:40 GMT
ENV INFLUXDB_VERSION=1.9.9-c1.9.9
# Thu, 16 Mar 2023 00:56:00 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-meta_${INFLUXDB_VERSION}_amd64.deb*
# Thu, 16 Mar 2023 00:56:00 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Thu, 16 Mar 2023 00:56:00 GMT
EXPOSE 8091
# Thu, 16 Mar 2023 00:56:00 GMT
VOLUME [/var/lib/influxdb]
# Thu, 16 Mar 2023 00:56:01 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Thu, 16 Mar 2023 00:56:01 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 16 Mar 2023 00:56:01 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:32fb02163b6bb519a30f909008e852354dae10bdfd6b34190dbdfe8f15403ea0`  
		Last Modified: Wed, 01 Mar 2023 04:13:58 GMT  
		Size: 55.0 MB (55045922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:167c7feebee855d117e192389484ea8367be1ba84e7ee35f4e5e5663195facbf`  
		Last Modified: Wed, 01 Mar 2023 04:50:15 GMT  
		Size: 5.2 MB (5166586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6dfff1f6f3ddd2194ea0775f199572e8b2d75c38713eef0444d6b1fd0ac7604`  
		Last Modified: Wed, 01 Mar 2023 04:50:15 GMT  
		Size: 10.9 MB (10876729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a90f0187c37c44f2ad04f9d930d40ee0b886fc8d783b914b10a620683739873`  
		Last Modified: Thu, 16 Mar 2023 00:58:47 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2502402dea139f68a75642daab8657973c27a8cfc94c71340c42437d10818e98`  
		Last Modified: Thu, 16 Mar 2023 01:01:01 GMT  
		Size: 12.4 MB (12420014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03ef60031fca7b6970fc9deb38158fd941fb7e3641b3d34702a6feb1054c3f97`  
		Last Modified: Thu, 16 Mar 2023 01:00:59 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f27706e6d95ef794ecda0a682b96e8bf464a7f297cf8584fbd42381f229ff603`  
		Last Modified: Thu, 16 Mar 2023 01:00:59 GMT  
		Size: 375.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.9-meta-alpine`

```console
$ docker pull influxdb@sha256:6cf6ef32efa823b59fe6f6b5227330e163d73c0b4249bf34b456e5592d5d3959
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.9-meta-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:974de5bb07a09b633b4260a6a4ee6142fb6c966afe9d5c97330729aa2509d3d7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.2 MB (17230133 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97bce6d03c1993977700d4b76e36b90b5fff2be3b8e1c963a2648c7feb6af14c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:42 GMT
ADD file:40887ab7c06977737e63c215c9bd297c0c74de8d12d16ebdf1c3d40ac392f62d in / 
# Sat, 11 Feb 2023 04:46:42 GMT
CMD ["/bin/sh"]
# Mon, 13 Mar 2023 23:20:24 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 16 Mar 2023 00:54:52 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Thu, 16 Mar 2023 00:55:47 GMT
ENV INFLUXDB_VERSION=1.9.9-c1.9.9
# Thu, 16 Mar 2023 00:56:08 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/etc/influxdb/influxdb-meta.conf &&     chmod +x /usr/src/influxdb-*/usr/bin/* &&     cp -a /usr/src/influxdb-*/usr/bin/. /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Thu, 16 Mar 2023 00:56:08 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Thu, 16 Mar 2023 00:56:08 GMT
EXPOSE 8091
# Thu, 16 Mar 2023 00:56:08 GMT
VOLUME [/var/lib/influxdb]
# Thu, 16 Mar 2023 00:56:08 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Thu, 16 Mar 2023 00:56:08 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 16 Mar 2023 00:56:08 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:63b65145d645c1250c391b2d16ebe53b3747c295ca8ba2fcb6b0cf064a4dc21c`  
		Last Modified: Fri, 10 Feb 2023 22:41:31 GMT  
		Size: 3.4 MB (3374446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69b7a2cbfc2f3b3305293d689573f3c9651d6053e5f780a9ba42a4c836d8d6c9`  
		Last Modified: Mon, 13 Mar 2023 23:21:18 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5b0a9605b8bc1c4f3b877c51f73e8d0cc4b02403f8f9d18c276f012b604c038`  
		Last Modified: Thu, 16 Mar 2023 00:59:03 GMT  
		Size: 1.5 MB (1472712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1716fa375af24d9191c5656de727f1ab036095081eeb602f5cf64909006c01b8`  
		Last Modified: Thu, 16 Mar 2023 01:01:12 GMT  
		Size: 12.4 MB (12382103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da5539cffeff417a70ad0e1ed076ee0bd2287365615c945b85d1aabb46b73a05`  
		Last Modified: Thu, 16 Mar 2023 01:01:09 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6483e3e49a69d80955bd72f5c320b94da933ef7cd9241bcb768c474cbafd3e8f`  
		Last Modified: Thu, 16 Mar 2023 01:01:10 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.9.9-data`

```console
$ docker pull influxdb@sha256:38bd41f3e323ee0115ecbe8264d1c2bc201c6fdb58fad417f72c8418bc15f3c4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.9.9-data` - linux; amd64

```console
$ docker pull influxdb@sha256:487cabb4dd16bf501ac4e07644ce3bb82a4c435118285e96cbf8643f9d34cbab
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **103.9 MB (103949152 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd026e7f0d602c645cc44cc05f8a12dc9a1490d9b3072f60df8e08db25498361`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 01 Mar 2023 04:09:45 GMT
ADD file:513c5d5e501279c21a05c1d8b66e5f0b02ee4b27f0b928706d92fd9ce11c1be6 in / 
# Wed, 01 Mar 2023 04:09:46 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 04:42:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 04:42:43 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Mar 2023 00:54:43 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 16 Mar 2023 00:55:40 GMT
ENV INFLUXDB_VERSION=1.9.9-c1.9.9
# Thu, 16 Mar 2023 00:55:44 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-data_${INFLUXDB_VERSION}_amd64.deb*
# Thu, 16 Mar 2023 00:55:44 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Thu, 16 Mar 2023 00:55:44 GMT
EXPOSE 8086
# Thu, 16 Mar 2023 00:55:44 GMT
VOLUME [/var/lib/influxdb]
# Thu, 16 Mar 2023 00:55:44 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Thu, 16 Mar 2023 00:55:44 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Thu, 16 Mar 2023 00:55:44 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 16 Mar 2023 00:55:45 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:32fb02163b6bb519a30f909008e852354dae10bdfd6b34190dbdfe8f15403ea0`  
		Last Modified: Wed, 01 Mar 2023 04:13:58 GMT  
		Size: 55.0 MB (55045922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:167c7feebee855d117e192389484ea8367be1ba84e7ee35f4e5e5663195facbf`  
		Last Modified: Wed, 01 Mar 2023 04:50:15 GMT  
		Size: 5.2 MB (5166586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6dfff1f6f3ddd2194ea0775f199572e8b2d75c38713eef0444d6b1fd0ac7604`  
		Last Modified: Wed, 01 Mar 2023 04:50:15 GMT  
		Size: 10.9 MB (10876729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a90f0187c37c44f2ad04f9d930d40ee0b886fc8d783b914b10a620683739873`  
		Last Modified: Thu, 16 Mar 2023 00:58:47 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:070b7597564eefee299403e56cb3bdabea7775a74edd530e72271a17044dd49f`  
		Last Modified: Thu, 16 Mar 2023 01:00:35 GMT  
		Size: 32.9 MB (32856344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59b018312f678fb3801e0c6414cf6d1ff76326856c42ef75541ce88a080724ed`  
		Last Modified: Thu, 16 Mar 2023 01:00:30 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f87e0de7ba6781751725d7580b29bd74789bf7ab7b79c0cb54db93329c8ea0a7`  
		Last Modified: Thu, 16 Mar 2023 01:00:30 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2e3792499531b5a00bb695cbe9115f2bb8049e3810a92df4fa0a5587b63c519`  
		Last Modified: Thu, 16 Mar 2023 01:00:30 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.9.9-data-alpine`

```console
$ docker pull influxdb@sha256:1dc0dc45dfb8565a191482ff12f8ef21abf086d7b3ea80afed3e2760d3b6cfd4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.9.9-data-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:180f5debe1662fc59e945ce8595ca6c39d50109358c02dc302035a9c6596d628
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.7 MB (37661708 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8379824b3de5e2abeb7c1e053e7342d7f44e2d330dfda7437e77d7f0c1532159`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:42 GMT
ADD file:40887ab7c06977737e63c215c9bd297c0c74de8d12d16ebdf1c3d40ac392f62d in / 
# Sat, 11 Feb 2023 04:46:42 GMT
CMD ["/bin/sh"]
# Mon, 13 Mar 2023 23:20:24 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 16 Mar 2023 00:54:52 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Thu, 16 Mar 2023 00:55:47 GMT
ENV INFLUXDB_VERSION=1.9.9-c1.9.9
# Thu, 16 Mar 2023 00:55:53 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/etc/influxdb/influxdb.conf &&     chmod +x /usr/src/influxdb-*/usr/bin/* &&     cp -a /usr/src/influxdb-*/usr/bin/. /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Thu, 16 Mar 2023 00:55:53 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Thu, 16 Mar 2023 00:55:53 GMT
EXPOSE 8086
# Thu, 16 Mar 2023 00:55:54 GMT
VOLUME [/var/lib/influxdb]
# Thu, 16 Mar 2023 00:55:54 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Thu, 16 Mar 2023 00:55:54 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Thu, 16 Mar 2023 00:55:54 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 16 Mar 2023 00:55:54 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:63b65145d645c1250c391b2d16ebe53b3747c295ca8ba2fcb6b0cf064a4dc21c`  
		Last Modified: Fri, 10 Feb 2023 22:41:31 GMT  
		Size: 3.4 MB (3374446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69b7a2cbfc2f3b3305293d689573f3c9651d6053e5f780a9ba42a4c836d8d6c9`  
		Last Modified: Mon, 13 Mar 2023 23:21:18 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5b0a9605b8bc1c4f3b877c51f73e8d0cc4b02403f8f9d18c276f012b604c038`  
		Last Modified: Thu, 16 Mar 2023 00:59:03 GMT  
		Size: 1.5 MB (1472712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62ba7c0784ed61eca939fe14f9fca623589151b853f30334f72ca0e9b36659a9`  
		Last Modified: Thu, 16 Mar 2023 01:00:50 GMT  
		Size: 32.8 MB (32812476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:433821cacc6957d02fa7385c77f6321fa782bdf57beec08b87215f22a4421531`  
		Last Modified: Thu, 16 Mar 2023 01:00:45 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0083dacac064d2fe5ef51b7c30236bf749162d05e1220935457f408b1c152e10`  
		Last Modified: Thu, 16 Mar 2023 01:00:45 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f714b29738f1da6463e2f95941fbd4f0f54279ddd7b6d9ca0b1f28cfcd072a58`  
		Last Modified: Thu, 16 Mar 2023 01:00:45 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.9.9-meta`

```console
$ docker pull influxdb@sha256:b1df3ae80c7bd334c4a8b6e2c740e9e6b9bcef3a13a9c3c65fc5649b82b0f2f2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.9.9-meta` - linux; amd64

```console
$ docker pull influxdb@sha256:490acef35891290e3e46536d01cf5021644d5bf720008333c91ed463004c8a15
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.5 MB (83511617 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d4a13fb1976426aaa2da3c36ac74e5856c68a8a4ae2c415dbb5cb527a24dca5`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Wed, 01 Mar 2023 04:09:45 GMT
ADD file:513c5d5e501279c21a05c1d8b66e5f0b02ee4b27f0b928706d92fd9ce11c1be6 in / 
# Wed, 01 Mar 2023 04:09:46 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 04:42:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 04:42:43 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Mar 2023 00:54:43 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 16 Mar 2023 00:55:40 GMT
ENV INFLUXDB_VERSION=1.9.9-c1.9.9
# Thu, 16 Mar 2023 00:56:00 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-meta_${INFLUXDB_VERSION}_amd64.deb*
# Thu, 16 Mar 2023 00:56:00 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Thu, 16 Mar 2023 00:56:00 GMT
EXPOSE 8091
# Thu, 16 Mar 2023 00:56:00 GMT
VOLUME [/var/lib/influxdb]
# Thu, 16 Mar 2023 00:56:01 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Thu, 16 Mar 2023 00:56:01 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 16 Mar 2023 00:56:01 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:32fb02163b6bb519a30f909008e852354dae10bdfd6b34190dbdfe8f15403ea0`  
		Last Modified: Wed, 01 Mar 2023 04:13:58 GMT  
		Size: 55.0 MB (55045922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:167c7feebee855d117e192389484ea8367be1ba84e7ee35f4e5e5663195facbf`  
		Last Modified: Wed, 01 Mar 2023 04:50:15 GMT  
		Size: 5.2 MB (5166586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6dfff1f6f3ddd2194ea0775f199572e8b2d75c38713eef0444d6b1fd0ac7604`  
		Last Modified: Wed, 01 Mar 2023 04:50:15 GMT  
		Size: 10.9 MB (10876729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a90f0187c37c44f2ad04f9d930d40ee0b886fc8d783b914b10a620683739873`  
		Last Modified: Thu, 16 Mar 2023 00:58:47 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2502402dea139f68a75642daab8657973c27a8cfc94c71340c42437d10818e98`  
		Last Modified: Thu, 16 Mar 2023 01:01:01 GMT  
		Size: 12.4 MB (12420014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03ef60031fca7b6970fc9deb38158fd941fb7e3641b3d34702a6feb1054c3f97`  
		Last Modified: Thu, 16 Mar 2023 01:00:59 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f27706e6d95ef794ecda0a682b96e8bf464a7f297cf8584fbd42381f229ff603`  
		Last Modified: Thu, 16 Mar 2023 01:00:59 GMT  
		Size: 375.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.9.9-meta-alpine`

```console
$ docker pull influxdb@sha256:6cf6ef32efa823b59fe6f6b5227330e163d73c0b4249bf34b456e5592d5d3959
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.9.9-meta-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:974de5bb07a09b633b4260a6a4ee6142fb6c966afe9d5c97330729aa2509d3d7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.2 MB (17230133 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97bce6d03c1993977700d4b76e36b90b5fff2be3b8e1c963a2648c7feb6af14c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:42 GMT
ADD file:40887ab7c06977737e63c215c9bd297c0c74de8d12d16ebdf1c3d40ac392f62d in / 
# Sat, 11 Feb 2023 04:46:42 GMT
CMD ["/bin/sh"]
# Mon, 13 Mar 2023 23:20:24 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 16 Mar 2023 00:54:52 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Thu, 16 Mar 2023 00:55:47 GMT
ENV INFLUXDB_VERSION=1.9.9-c1.9.9
# Thu, 16 Mar 2023 00:56:08 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/etc/influxdb/influxdb-meta.conf &&     chmod +x /usr/src/influxdb-*/usr/bin/* &&     cp -a /usr/src/influxdb-*/usr/bin/. /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Thu, 16 Mar 2023 00:56:08 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Thu, 16 Mar 2023 00:56:08 GMT
EXPOSE 8091
# Thu, 16 Mar 2023 00:56:08 GMT
VOLUME [/var/lib/influxdb]
# Thu, 16 Mar 2023 00:56:08 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Thu, 16 Mar 2023 00:56:08 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 16 Mar 2023 00:56:08 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:63b65145d645c1250c391b2d16ebe53b3747c295ca8ba2fcb6b0cf064a4dc21c`  
		Last Modified: Fri, 10 Feb 2023 22:41:31 GMT  
		Size: 3.4 MB (3374446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69b7a2cbfc2f3b3305293d689573f3c9651d6053e5f780a9ba42a4c836d8d6c9`  
		Last Modified: Mon, 13 Mar 2023 23:21:18 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5b0a9605b8bc1c4f3b877c51f73e8d0cc4b02403f8f9d18c276f012b604c038`  
		Last Modified: Thu, 16 Mar 2023 00:59:03 GMT  
		Size: 1.5 MB (1472712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1716fa375af24d9191c5656de727f1ab036095081eeb602f5cf64909006c01b8`  
		Last Modified: Thu, 16 Mar 2023 01:01:12 GMT  
		Size: 12.4 MB (12382103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da5539cffeff417a70ad0e1ed076ee0bd2287365615c945b85d1aabb46b73a05`  
		Last Modified: Thu, 16 Mar 2023 01:01:09 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6483e3e49a69d80955bd72f5c320b94da933ef7cd9241bcb768c474cbafd3e8f`  
		Last Modified: Thu, 16 Mar 2023 01:01:10 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:2.4`

```console
$ docker pull influxdb@sha256:67a8e5a038a287e8788d94f4ba46405505311ccf0bd4fb25f008236fa532bd40
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:2.4` - linux; amd64

```console
$ docker pull influxdb@sha256:3ecf42afa2a58a69033df0d52b8c59ec99469f606a2366f4ab5348d5ed84ab4e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **144.8 MB (144754565 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c458df6c89099c26dd2e8a0e12a3df22e03e03d75741e0b81722aa0c49c00ec`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 01 Mar 2023 04:09:58 GMT
ADD file:493a5b0c8d2d63a1343258b3f9aa5fcd59a93f44fe26ad9e56b094c3a08fd3be in / 
# Wed, 01 Mar 2023 04:09:59 GMT
CMD ["bash"]
# Thu, 16 Mar 2023 00:56:52 GMT
RUN export DEBIAN_FRONTEND=noninteractive &&     apt-get update -y &&     apt-get install -y --no-install-recommends       ca-certificates       curl       gnupg &&     apt-get clean &&     rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 00:56:53 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     curl -fLo /usr/local/bin/yq "https://github.com/mikefarah/yq/releases/download/v4.30.8/yq_linux_${arch}" &&     case ${arch} in       amd64) echo '6c911103e0dcc54e2ba07e767d2d62bcfc77452b39ebaee45b1c46f062f4fd26 /usr/local/bin/yq' ;;       arm64) echo '95092e8b5332890c46689679b5e4360d96873c025ad8bafd961688f28ea434c7 /usr/local/bin/yq' ;;     esac | sha256sum -c - &&     chmod +x /usr/local/bin/yq &&     yq --version
# Thu, 16 Mar 2023 00:56:53 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --create-home --home-dir=/home/influxdb --shell=/bin/bash influxdb
# Thu, 16 Mar 2023 00:56:53 GMT
ENV GOSU_VER=1.12
# Thu, 16 Mar 2023 00:56:56 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       B42F6819007F00F88E364FD4036A9C25BF357DD4 &&     curl -fLo /usr/local/bin/gosu     "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-${arch}"          -fLo /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-${arch}.asc" &&     gpg --batch --verify /usr/local/bin/gosu.asc                          /usr/local/bin/gosu &&     rm -rf /usr/local/bin/gosu.asc &&     chmod +x /usr/local/bin/gosu &&     gosu --version &&     gosu nobody true
# Thu, 16 Mar 2023 00:56:56 GMT
ENV INFLUXDB_VERSION=2.4.0
# Thu, 16 Mar 2023 00:57:03 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     cp "influxdb2_linux_${arch}/influxd" /usr/local/bin/influxd &&     rm -rf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"            "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"            "influxdb2_linux_${arch}" &&     influxd version
# Thu, 16 Mar 2023 00:57:03 GMT
ENV INFLUX_CLI_VERSION=2.4.0
# Thu, 16 Mar 2023 00:57:06 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     cp "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}/influx" /usr/local/bin/influx &&     rm -rf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     influx version
# Thu, 16 Mar 2023 00:57:07 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Thu, 16 Mar 2023 00:57:07 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Thu, 16 Mar 2023 00:57:07 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Thu, 16 Mar 2023 00:57:07 GMT
COPY file:595a669a2c2c2f47df93700fcd3e412750aae40abb979bb4af48a89af97a8b72 in /entrypoint.sh 
# Thu, 16 Mar 2023 00:57:07 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 16 Mar 2023 00:57:07 GMT
CMD ["influxd"]
# Thu, 16 Mar 2023 00:57:07 GMT
EXPOSE 8086
# Thu, 16 Mar 2023 00:57:07 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Thu, 16 Mar 2023 00:57:07 GMT
ENV INFLUXD_INIT_PORT=9999
# Thu, 16 Mar 2023 00:57:07 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Thu, 16 Mar 2023 00:57:08 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:3f9582a2cbe7197f39185419c0ced2c986389f8fc6aa805e1f5c090eea6511e0`  
		Last Modified: Wed, 01 Mar 2023 04:14:23 GMT  
		Size: 31.4 MB (31411403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08a794c78d7ad502e285244fde2dd7768065af2038670e7f34208e22d1c857e2`  
		Last Modified: Thu, 16 Mar 2023 01:02:10 GMT  
		Size: 6.3 MB (6327743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acd90bd5b5e60e8373c43b82a755b742e62d469c7df42aef9ab6ad0ac943ef6b`  
		Last Modified: Thu, 16 Mar 2023 01:02:09 GMT  
		Size: 7.0 MB (7049181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a549c3bac6c035d00d970ff0a7c39398de5b5355e5264970174a609dfcb350c1`  
		Last Modified: Thu, 16 Mar 2023 01:02:08 GMT  
		Size: 4.1 KB (4117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d52f68e8e59a067e13373eed04aa01fa28f3e99320d3ccfb46232c85efe7432`  
		Last Modified: Thu, 16 Mar 2023 01:02:08 GMT  
		Size: 982.0 KB (982043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74bb7c04a956102e66f3cb994dc541b7cfa7c7dd7defdbbd043e9d998742f986`  
		Last Modified: Thu, 16 Mar 2023 01:02:13 GMT  
		Size: 92.9 MB (92899954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7ec98191584bb01e8d834ce27daff8379346e940c3bad50d29c41fe0ee826d8`  
		Last Modified: Thu, 16 Mar 2023 01:02:07 GMT  
		Size: 6.1 MB (6073125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70117d878e5ca6eb7043edc28da77e1283c3ea6c7ddcd4733ee091ae6cd9f2ea`  
		Last Modified: Thu, 16 Mar 2023 01:02:06 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:116bdcfe937000da7482135e940b4ff6f650468f06aae81e9362ebed3a52f897`  
		Last Modified: Thu, 16 Mar 2023 01:02:06 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbfeb8db7f405e32dfb913d7518ce7bc26dc4839fabcfa410a619d5343e2a118`  
		Last Modified: Thu, 16 Mar 2023 01:02:06 GMT  
		Size: 6.5 KB (6463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:2.4` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:9bd9efbcee8ed3b0504ebbd48a0e6ebe644411658074d3f08590796944f257dc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **140.8 MB (140770736 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d50b8c791f8296777f3586d747423699b5ebff3d0c515a52500f4c257ae7a5d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 01 Mar 2023 02:20:39 GMT
ADD file:9dc5c6fb6431df80107eddb76fb18256d6f4a06b4b22f9a7c4bcd58476068186 in / 
# Wed, 01 Mar 2023 02:20:39 GMT
CMD ["bash"]
# Wed, 15 Mar 2023 23:41:07 GMT
RUN export DEBIAN_FRONTEND=noninteractive &&     apt-get update -y &&     apt-get install -y --no-install-recommends       ca-certificates       curl       gnupg &&     apt-get clean &&     rm -rf /var/lib/apt/lists/*
# Wed, 15 Mar 2023 23:41:08 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     curl -fLo /usr/local/bin/yq "https://github.com/mikefarah/yq/releases/download/v4.30.8/yq_linux_${arch}" &&     case ${arch} in       amd64) echo '6c911103e0dcc54e2ba07e767d2d62bcfc77452b39ebaee45b1c46f062f4fd26 /usr/local/bin/yq' ;;       arm64) echo '95092e8b5332890c46689679b5e4360d96873c025ad8bafd961688f28ea434c7 /usr/local/bin/yq' ;;     esac | sha256sum -c - &&     chmod +x /usr/local/bin/yq &&     yq --version
# Wed, 15 Mar 2023 23:41:09 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --create-home --home-dir=/home/influxdb --shell=/bin/bash influxdb
# Wed, 15 Mar 2023 23:41:09 GMT
ENV GOSU_VER=1.12
# Wed, 15 Mar 2023 23:41:11 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       B42F6819007F00F88E364FD4036A9C25BF357DD4 &&     curl -fLo /usr/local/bin/gosu     "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-${arch}"          -fLo /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-${arch}.asc" &&     gpg --batch --verify /usr/local/bin/gosu.asc                          /usr/local/bin/gosu &&     rm -rf /usr/local/bin/gosu.asc &&     chmod +x /usr/local/bin/gosu &&     gosu --version &&     gosu nobody true
# Wed, 15 Mar 2023 23:41:11 GMT
ENV INFLUXDB_VERSION=2.4.0
# Wed, 15 Mar 2023 23:41:18 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     cp "influxdb2_linux_${arch}/influxd" /usr/local/bin/influxd &&     rm -rf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"            "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"            "influxdb2_linux_${arch}" &&     influxd version
# Wed, 15 Mar 2023 23:41:18 GMT
ENV INFLUX_CLI_VERSION=2.4.0
# Wed, 15 Mar 2023 23:41:20 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     cp "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}/influx" /usr/local/bin/influx &&     rm -rf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     influx version
# Wed, 15 Mar 2023 23:41:21 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Wed, 15 Mar 2023 23:41:21 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Wed, 15 Mar 2023 23:41:21 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Wed, 15 Mar 2023 23:41:21 GMT
COPY file:595a669a2c2c2f47df93700fcd3e412750aae40abb979bb4af48a89af97a8b72 in /entrypoint.sh 
# Wed, 15 Mar 2023 23:41:21 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 15 Mar 2023 23:41:21 GMT
CMD ["influxd"]
# Wed, 15 Mar 2023 23:41:21 GMT
EXPOSE 8086
# Wed, 15 Mar 2023 23:41:21 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Wed, 15 Mar 2023 23:41:21 GMT
ENV INFLUXD_INIT_PORT=9999
# Wed, 15 Mar 2023 23:41:22 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Wed, 15 Mar 2023 23:41:22 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:66dbba0fb1b568cc3ffd53409ba2f9f82995ab7f80e379338f3f36e4dcd223be`  
		Last Modified: Wed, 01 Mar 2023 02:24:17 GMT  
		Size: 30.1 MB (30062814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65fd6db03d5e7efd9c898c05fa431254e6753c9d39caf9a942d187e791ef698e`  
		Last Modified: Wed, 15 Mar 2023 23:42:58 GMT  
		Size: 6.3 MB (6308600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:623e77e647b06d59d840fce37c059b20aa366a51af80637fd63e1e5512a9e5e6`  
		Last Modified: Wed, 15 Mar 2023 23:42:57 GMT  
		Size: 6.6 MB (6643045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4316c8eeb27a0e8e1b5c0adabd0c1c7a915c9dfda919151dea2c1f0fbd9b5b8d`  
		Last Modified: Wed, 15 Mar 2023 23:42:57 GMT  
		Size: 4.1 KB (4124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ed509fbb0848d068923c7c2fb0326172783db14b7e706111aa8d36fef0724e1`  
		Last Modified: Wed, 15 Mar 2023 23:42:57 GMT  
		Size: 916.9 KB (916930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f524bde5de6be14d80266fa77c0f0b2e9b6715972a2366269e64ed8a5ec02f3f`  
		Last Modified: Wed, 15 Mar 2023 23:43:00 GMT  
		Size: 91.2 MB (91223715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a8371e14baf0dafcf58e34ac749e80281e50e01ea5507b0373a9b568b494f27`  
		Last Modified: Wed, 15 Mar 2023 23:42:55 GMT  
		Size: 5.6 MB (5604509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b41d5a99b1ac7a6fa810be4beaa511d6acba053dcb4f52a72faf153a95b4e52`  
		Last Modified: Wed, 15 Mar 2023 23:42:55 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dcdd865d8c48c8cb065683f1755dc579621a7e2dcc0033a0bf3c0f1930754b2`  
		Last Modified: Wed, 15 Mar 2023 23:42:54 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92d4fc2ba8efe9e0204b53cfe7a86244804c3a04f17be0f3c3ee8128a1a55fb8`  
		Last Modified: Wed, 15 Mar 2023 23:42:54 GMT  
		Size: 6.5 KB (6463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:2.4-alpine`

```console
$ docker pull influxdb@sha256:b294047dc44e6b9b7f8e152718a1bd2fb4707601782ff7a9d58e319eb2cc105e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:2.4-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:14dea367e153a8d4dd77231cfcf2c48399bb061139e7785c365d16fc62c7b8d2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.7 MB (114730997 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:04d8c9f3c8af55a8c01e61fb93e5af7332749e4a7b11dc7380fbc85389ef41da`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:42 GMT
ADD file:40887ab7c06977737e63c215c9bd297c0c74de8d12d16ebdf1c3d40ac392f62d in / 
# Sat, 11 Feb 2023 04:46:42 GMT
CMD ["/bin/sh"]
# Mon, 13 Mar 2023 23:20:24 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 16 Mar 2023 00:57:14 GMT
RUN apk add --no-cache       bash       ca-certificates       curl       gnupg       run-parts       su-exec       tzdata       yq &&     update-ca-certificates
# Thu, 16 Mar 2023 00:57:14 GMT
RUN addgroup -S -g 1000 influxdb &&     adduser -S -G influxdb -u 1000 -h /home/influxdb -s /bin/sh influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Thu, 16 Mar 2023 00:57:14 GMT
ENV INFLUXDB_VERSION=2.4.0
# Thu, 16 Mar 2023 00:57:19 GMT
RUN case "$(apk --print-arch)" in       x86_64)  arch=amd64 ;;       aarch64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&    curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     cp "influxdb2_linux_${arch}/influxd" /usr/local/bin/influxd &&     rm -rf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"            "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"            "influxdb2_linux_${arch}" &&     influxd version
# Thu, 16 Mar 2023 00:57:20 GMT
ENV INFLUX_CLI_VERSION=2.4.0
# Thu, 16 Mar 2023 00:57:21 GMT
RUN case "$(apk --print-arch)" in       x86_64)  arch=amd64 ;;       aarch64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     cp "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}/influx" /usr/local/bin/influx &&     rm -rf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     influx version
# Thu, 16 Mar 2023 00:57:22 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Thu, 16 Mar 2023 00:57:22 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Thu, 16 Mar 2023 00:57:22 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Thu, 16 Mar 2023 00:57:22 GMT
COPY file:708cccb15c29f10eb0c29e47f1c676d76b8ea9be434cce106ef95a7ba844bb2c in /entrypoint.sh 
# Thu, 16 Mar 2023 00:57:22 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 16 Mar 2023 00:57:22 GMT
CMD ["influxd"]
# Thu, 16 Mar 2023 00:57:22 GMT
EXPOSE 8086
# Thu, 16 Mar 2023 00:57:22 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Thu, 16 Mar 2023 00:57:23 GMT
ENV INFLUXD_INIT_PORT=9999
# Thu, 16 Mar 2023 00:57:23 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Thu, 16 Mar 2023 00:57:23 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:63b65145d645c1250c391b2d16ebe53b3747c295ca8ba2fcb6b0cf064a4dc21c`  
		Last Modified: Fri, 10 Feb 2023 22:41:31 GMT  
		Size: 3.4 MB (3374446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69b7a2cbfc2f3b3305293d689573f3c9651d6053e5f780a9ba42a4c836d8d6c9`  
		Last Modified: Mon, 13 Mar 2023 23:21:18 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9662dafd479312640e4852a3e8b4caa9c758e1d55e2177a988e8defb54fb3c4`  
		Last Modified: Thu, 16 Mar 2023 01:02:25 GMT  
		Size: 12.4 MB (12375014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cc9d593845c782b74273932afc2437f197ed7d05bc6d861ed3ac5f7d84da491`  
		Last Modified: Thu, 16 Mar 2023 01:02:24 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5752aeca8c552823e76ab58e99fd551721c4b38a0ac0871b7e5f1cf14a029b0`  
		Last Modified: Thu, 16 Mar 2023 01:02:29 GMT  
		Size: 92.9 MB (92899897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9ea5e8fc39fbbde89567d86def676e7c9f6e1a24bb83295bf60483ea1ced1ee`  
		Last Modified: Thu, 16 Mar 2023 01:02:23 GMT  
		Size: 6.1 MB (6073114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75c18bedddfdbccd0ecaf4b2477d2ff6a05025928771c575c05eeecc0e477388`  
		Last Modified: Thu, 16 Mar 2023 01:02:22 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21e813712bd5c3d8e52e6f4a1d0813dfecd1d6967baa8f6b2cc0793474c82fa3`  
		Last Modified: Thu, 16 Mar 2023 01:02:21 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9ff84c115204ae9cb222ecf853e6ad53697a26f6e1aabc6c391db9ebc88aa6e`  
		Last Modified: Thu, 16 Mar 2023 01:02:22 GMT  
		Size: 6.4 KB (6442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:2.4-alpine` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:9ec0c7a67d2c3f6e36325858423c6c01b9d4b1ba6560fc101487ed04ea2c50eb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **112.1 MB (112127015 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:47392e61808b63c1a3d5cbf76b5650719d35bbac9310de4fabe8c8cf140cd185`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:08 GMT
ADD file:9bd9ea42a9f3bdc769e80c6b8a4b117d65f73ae68e155a6172a1184e7ac8bcc1 in / 
# Fri, 10 Feb 2023 21:24:08 GMT
CMD ["/bin/sh"]
# Mon, 13 Mar 2023 23:47:18 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 15 Mar 2023 23:41:30 GMT
RUN apk add --no-cache       bash       ca-certificates       curl       gnupg       run-parts       su-exec       tzdata       yq &&     update-ca-certificates
# Wed, 15 Mar 2023 23:41:31 GMT
RUN addgroup -S -g 1000 influxdb &&     adduser -S -G influxdb -u 1000 -h /home/influxdb -s /bin/sh influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Wed, 15 Mar 2023 23:41:31 GMT
ENV INFLUXDB_VERSION=2.4.0
# Wed, 15 Mar 2023 23:41:35 GMT
RUN case "$(apk --print-arch)" in       x86_64)  arch=amd64 ;;       aarch64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&    curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     cp "influxdb2_linux_${arch}/influxd" /usr/local/bin/influxd &&     rm -rf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"            "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"            "influxdb2_linux_${arch}" &&     influxd version
# Wed, 15 Mar 2023 23:41:36 GMT
ENV INFLUX_CLI_VERSION=2.4.0
# Wed, 15 Mar 2023 23:41:38 GMT
RUN case "$(apk --print-arch)" in       x86_64)  arch=amd64 ;;       aarch64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     cp "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}/influx" /usr/local/bin/influx &&     rm -rf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     influx version
# Wed, 15 Mar 2023 23:41:38 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Wed, 15 Mar 2023 23:41:38 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Wed, 15 Mar 2023 23:41:39 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Wed, 15 Mar 2023 23:41:39 GMT
COPY file:708cccb15c29f10eb0c29e47f1c676d76b8ea9be434cce106ef95a7ba844bb2c in /entrypoint.sh 
# Wed, 15 Mar 2023 23:41:39 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 15 Mar 2023 23:41:39 GMT
CMD ["influxd"]
# Wed, 15 Mar 2023 23:41:39 GMT
EXPOSE 8086
# Wed, 15 Mar 2023 23:41:39 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Wed, 15 Mar 2023 23:41:39 GMT
ENV INFLUXD_INIT_PORT=9999
# Wed, 15 Mar 2023 23:41:39 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Wed, 15 Mar 2023 23:41:39 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:af6eaf76a39c2d3e7e0b8a0420486e3df33c4027d696c076a99a3d0ac09026af`  
		Last Modified: Fri, 10 Feb 2023 21:24:39 GMT  
		Size: 3.3 MB (3261959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dab1c38052d53938443512e37031810a03849aec98af5976a010b92ee4c13c1`  
		Last Modified: Mon, 13 Mar 2023 23:48:01 GMT  
		Size: 282.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd8e20b18f6688b37abc667eef7975eb77966987c3212d862a3b74b1e5a46151`  
		Last Modified: Wed, 15 Mar 2023 23:43:14 GMT  
		Size: 12.0 MB (12028387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:355a214bdc1929ff97f235f78bbe4313aa1f932134f19887c12d346d935da41e`  
		Last Modified: Wed, 15 Mar 2023 23:43:12 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2838674c2f9c183dc57cb7df56bdb750d889101e8dac0891cde3a2a4da77be0e`  
		Last Modified: Wed, 15 Mar 2023 23:43:16 GMT  
		Size: 91.2 MB (91223657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99c7fa0e61c0abdf5737711c7773876ff492bfcdb531a7bf8df3de30e1c6c491`  
		Last Modified: Wed, 15 Mar 2023 23:43:11 GMT  
		Size: 5.6 MB (5604482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:868fc0f0dc38e81c34af1ec71ff2071c9ec66ff81b6518bba94bb1c9e4b315bc`  
		Last Modified: Wed, 15 Mar 2023 23:43:10 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a99651d10b3c65f8e9e95531f448955b6abed3ddd329e22a4263c6404c51c401`  
		Last Modified: Wed, 15 Mar 2023 23:43:10 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a85002e06f2f9431c2f48da51407830849c5d6a67dceb068a4734ee31d39e849`  
		Last Modified: Wed, 15 Mar 2023 23:43:10 GMT  
		Size: 6.4 KB (6441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:2.4.0`

```console
$ docker pull influxdb@sha256:67a8e5a038a287e8788d94f4ba46405505311ccf0bd4fb25f008236fa532bd40
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:2.4.0` - linux; amd64

```console
$ docker pull influxdb@sha256:3ecf42afa2a58a69033df0d52b8c59ec99469f606a2366f4ab5348d5ed84ab4e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **144.8 MB (144754565 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c458df6c89099c26dd2e8a0e12a3df22e03e03d75741e0b81722aa0c49c00ec`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 01 Mar 2023 04:09:58 GMT
ADD file:493a5b0c8d2d63a1343258b3f9aa5fcd59a93f44fe26ad9e56b094c3a08fd3be in / 
# Wed, 01 Mar 2023 04:09:59 GMT
CMD ["bash"]
# Thu, 16 Mar 2023 00:56:52 GMT
RUN export DEBIAN_FRONTEND=noninteractive &&     apt-get update -y &&     apt-get install -y --no-install-recommends       ca-certificates       curl       gnupg &&     apt-get clean &&     rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 00:56:53 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     curl -fLo /usr/local/bin/yq "https://github.com/mikefarah/yq/releases/download/v4.30.8/yq_linux_${arch}" &&     case ${arch} in       amd64) echo '6c911103e0dcc54e2ba07e767d2d62bcfc77452b39ebaee45b1c46f062f4fd26 /usr/local/bin/yq' ;;       arm64) echo '95092e8b5332890c46689679b5e4360d96873c025ad8bafd961688f28ea434c7 /usr/local/bin/yq' ;;     esac | sha256sum -c - &&     chmod +x /usr/local/bin/yq &&     yq --version
# Thu, 16 Mar 2023 00:56:53 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --create-home --home-dir=/home/influxdb --shell=/bin/bash influxdb
# Thu, 16 Mar 2023 00:56:53 GMT
ENV GOSU_VER=1.12
# Thu, 16 Mar 2023 00:56:56 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       B42F6819007F00F88E364FD4036A9C25BF357DD4 &&     curl -fLo /usr/local/bin/gosu     "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-${arch}"          -fLo /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-${arch}.asc" &&     gpg --batch --verify /usr/local/bin/gosu.asc                          /usr/local/bin/gosu &&     rm -rf /usr/local/bin/gosu.asc &&     chmod +x /usr/local/bin/gosu &&     gosu --version &&     gosu nobody true
# Thu, 16 Mar 2023 00:56:56 GMT
ENV INFLUXDB_VERSION=2.4.0
# Thu, 16 Mar 2023 00:57:03 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     cp "influxdb2_linux_${arch}/influxd" /usr/local/bin/influxd &&     rm -rf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"            "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"            "influxdb2_linux_${arch}" &&     influxd version
# Thu, 16 Mar 2023 00:57:03 GMT
ENV INFLUX_CLI_VERSION=2.4.0
# Thu, 16 Mar 2023 00:57:06 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     cp "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}/influx" /usr/local/bin/influx &&     rm -rf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     influx version
# Thu, 16 Mar 2023 00:57:07 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Thu, 16 Mar 2023 00:57:07 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Thu, 16 Mar 2023 00:57:07 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Thu, 16 Mar 2023 00:57:07 GMT
COPY file:595a669a2c2c2f47df93700fcd3e412750aae40abb979bb4af48a89af97a8b72 in /entrypoint.sh 
# Thu, 16 Mar 2023 00:57:07 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 16 Mar 2023 00:57:07 GMT
CMD ["influxd"]
# Thu, 16 Mar 2023 00:57:07 GMT
EXPOSE 8086
# Thu, 16 Mar 2023 00:57:07 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Thu, 16 Mar 2023 00:57:07 GMT
ENV INFLUXD_INIT_PORT=9999
# Thu, 16 Mar 2023 00:57:07 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Thu, 16 Mar 2023 00:57:08 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:3f9582a2cbe7197f39185419c0ced2c986389f8fc6aa805e1f5c090eea6511e0`  
		Last Modified: Wed, 01 Mar 2023 04:14:23 GMT  
		Size: 31.4 MB (31411403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08a794c78d7ad502e285244fde2dd7768065af2038670e7f34208e22d1c857e2`  
		Last Modified: Thu, 16 Mar 2023 01:02:10 GMT  
		Size: 6.3 MB (6327743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acd90bd5b5e60e8373c43b82a755b742e62d469c7df42aef9ab6ad0ac943ef6b`  
		Last Modified: Thu, 16 Mar 2023 01:02:09 GMT  
		Size: 7.0 MB (7049181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a549c3bac6c035d00d970ff0a7c39398de5b5355e5264970174a609dfcb350c1`  
		Last Modified: Thu, 16 Mar 2023 01:02:08 GMT  
		Size: 4.1 KB (4117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d52f68e8e59a067e13373eed04aa01fa28f3e99320d3ccfb46232c85efe7432`  
		Last Modified: Thu, 16 Mar 2023 01:02:08 GMT  
		Size: 982.0 KB (982043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74bb7c04a956102e66f3cb994dc541b7cfa7c7dd7defdbbd043e9d998742f986`  
		Last Modified: Thu, 16 Mar 2023 01:02:13 GMT  
		Size: 92.9 MB (92899954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7ec98191584bb01e8d834ce27daff8379346e940c3bad50d29c41fe0ee826d8`  
		Last Modified: Thu, 16 Mar 2023 01:02:07 GMT  
		Size: 6.1 MB (6073125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70117d878e5ca6eb7043edc28da77e1283c3ea6c7ddcd4733ee091ae6cd9f2ea`  
		Last Modified: Thu, 16 Mar 2023 01:02:06 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:116bdcfe937000da7482135e940b4ff6f650468f06aae81e9362ebed3a52f897`  
		Last Modified: Thu, 16 Mar 2023 01:02:06 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbfeb8db7f405e32dfb913d7518ce7bc26dc4839fabcfa410a619d5343e2a118`  
		Last Modified: Thu, 16 Mar 2023 01:02:06 GMT  
		Size: 6.5 KB (6463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:2.4.0` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:9bd9efbcee8ed3b0504ebbd48a0e6ebe644411658074d3f08590796944f257dc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **140.8 MB (140770736 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d50b8c791f8296777f3586d747423699b5ebff3d0c515a52500f4c257ae7a5d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 01 Mar 2023 02:20:39 GMT
ADD file:9dc5c6fb6431df80107eddb76fb18256d6f4a06b4b22f9a7c4bcd58476068186 in / 
# Wed, 01 Mar 2023 02:20:39 GMT
CMD ["bash"]
# Wed, 15 Mar 2023 23:41:07 GMT
RUN export DEBIAN_FRONTEND=noninteractive &&     apt-get update -y &&     apt-get install -y --no-install-recommends       ca-certificates       curl       gnupg &&     apt-get clean &&     rm -rf /var/lib/apt/lists/*
# Wed, 15 Mar 2023 23:41:08 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     curl -fLo /usr/local/bin/yq "https://github.com/mikefarah/yq/releases/download/v4.30.8/yq_linux_${arch}" &&     case ${arch} in       amd64) echo '6c911103e0dcc54e2ba07e767d2d62bcfc77452b39ebaee45b1c46f062f4fd26 /usr/local/bin/yq' ;;       arm64) echo '95092e8b5332890c46689679b5e4360d96873c025ad8bafd961688f28ea434c7 /usr/local/bin/yq' ;;     esac | sha256sum -c - &&     chmod +x /usr/local/bin/yq &&     yq --version
# Wed, 15 Mar 2023 23:41:09 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --create-home --home-dir=/home/influxdb --shell=/bin/bash influxdb
# Wed, 15 Mar 2023 23:41:09 GMT
ENV GOSU_VER=1.12
# Wed, 15 Mar 2023 23:41:11 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       B42F6819007F00F88E364FD4036A9C25BF357DD4 &&     curl -fLo /usr/local/bin/gosu     "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-${arch}"          -fLo /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-${arch}.asc" &&     gpg --batch --verify /usr/local/bin/gosu.asc                          /usr/local/bin/gosu &&     rm -rf /usr/local/bin/gosu.asc &&     chmod +x /usr/local/bin/gosu &&     gosu --version &&     gosu nobody true
# Wed, 15 Mar 2023 23:41:11 GMT
ENV INFLUXDB_VERSION=2.4.0
# Wed, 15 Mar 2023 23:41:18 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     cp "influxdb2_linux_${arch}/influxd" /usr/local/bin/influxd &&     rm -rf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"            "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"            "influxdb2_linux_${arch}" &&     influxd version
# Wed, 15 Mar 2023 23:41:18 GMT
ENV INFLUX_CLI_VERSION=2.4.0
# Wed, 15 Mar 2023 23:41:20 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     cp "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}/influx" /usr/local/bin/influx &&     rm -rf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     influx version
# Wed, 15 Mar 2023 23:41:21 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Wed, 15 Mar 2023 23:41:21 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Wed, 15 Mar 2023 23:41:21 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Wed, 15 Mar 2023 23:41:21 GMT
COPY file:595a669a2c2c2f47df93700fcd3e412750aae40abb979bb4af48a89af97a8b72 in /entrypoint.sh 
# Wed, 15 Mar 2023 23:41:21 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 15 Mar 2023 23:41:21 GMT
CMD ["influxd"]
# Wed, 15 Mar 2023 23:41:21 GMT
EXPOSE 8086
# Wed, 15 Mar 2023 23:41:21 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Wed, 15 Mar 2023 23:41:21 GMT
ENV INFLUXD_INIT_PORT=9999
# Wed, 15 Mar 2023 23:41:22 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Wed, 15 Mar 2023 23:41:22 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:66dbba0fb1b568cc3ffd53409ba2f9f82995ab7f80e379338f3f36e4dcd223be`  
		Last Modified: Wed, 01 Mar 2023 02:24:17 GMT  
		Size: 30.1 MB (30062814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65fd6db03d5e7efd9c898c05fa431254e6753c9d39caf9a942d187e791ef698e`  
		Last Modified: Wed, 15 Mar 2023 23:42:58 GMT  
		Size: 6.3 MB (6308600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:623e77e647b06d59d840fce37c059b20aa366a51af80637fd63e1e5512a9e5e6`  
		Last Modified: Wed, 15 Mar 2023 23:42:57 GMT  
		Size: 6.6 MB (6643045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4316c8eeb27a0e8e1b5c0adabd0c1c7a915c9dfda919151dea2c1f0fbd9b5b8d`  
		Last Modified: Wed, 15 Mar 2023 23:42:57 GMT  
		Size: 4.1 KB (4124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ed509fbb0848d068923c7c2fb0326172783db14b7e706111aa8d36fef0724e1`  
		Last Modified: Wed, 15 Mar 2023 23:42:57 GMT  
		Size: 916.9 KB (916930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f524bde5de6be14d80266fa77c0f0b2e9b6715972a2366269e64ed8a5ec02f3f`  
		Last Modified: Wed, 15 Mar 2023 23:43:00 GMT  
		Size: 91.2 MB (91223715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a8371e14baf0dafcf58e34ac749e80281e50e01ea5507b0373a9b568b494f27`  
		Last Modified: Wed, 15 Mar 2023 23:42:55 GMT  
		Size: 5.6 MB (5604509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b41d5a99b1ac7a6fa810be4beaa511d6acba053dcb4f52a72faf153a95b4e52`  
		Last Modified: Wed, 15 Mar 2023 23:42:55 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dcdd865d8c48c8cb065683f1755dc579621a7e2dcc0033a0bf3c0f1930754b2`  
		Last Modified: Wed, 15 Mar 2023 23:42:54 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92d4fc2ba8efe9e0204b53cfe7a86244804c3a04f17be0f3c3ee8128a1a55fb8`  
		Last Modified: Wed, 15 Mar 2023 23:42:54 GMT  
		Size: 6.5 KB (6463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:2.4.0-alpine`

```console
$ docker pull influxdb@sha256:b294047dc44e6b9b7f8e152718a1bd2fb4707601782ff7a9d58e319eb2cc105e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:2.4.0-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:14dea367e153a8d4dd77231cfcf2c48399bb061139e7785c365d16fc62c7b8d2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.7 MB (114730997 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:04d8c9f3c8af55a8c01e61fb93e5af7332749e4a7b11dc7380fbc85389ef41da`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:42 GMT
ADD file:40887ab7c06977737e63c215c9bd297c0c74de8d12d16ebdf1c3d40ac392f62d in / 
# Sat, 11 Feb 2023 04:46:42 GMT
CMD ["/bin/sh"]
# Mon, 13 Mar 2023 23:20:24 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 16 Mar 2023 00:57:14 GMT
RUN apk add --no-cache       bash       ca-certificates       curl       gnupg       run-parts       su-exec       tzdata       yq &&     update-ca-certificates
# Thu, 16 Mar 2023 00:57:14 GMT
RUN addgroup -S -g 1000 influxdb &&     adduser -S -G influxdb -u 1000 -h /home/influxdb -s /bin/sh influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Thu, 16 Mar 2023 00:57:14 GMT
ENV INFLUXDB_VERSION=2.4.0
# Thu, 16 Mar 2023 00:57:19 GMT
RUN case "$(apk --print-arch)" in       x86_64)  arch=amd64 ;;       aarch64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&    curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     cp "influxdb2_linux_${arch}/influxd" /usr/local/bin/influxd &&     rm -rf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"            "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"            "influxdb2_linux_${arch}" &&     influxd version
# Thu, 16 Mar 2023 00:57:20 GMT
ENV INFLUX_CLI_VERSION=2.4.0
# Thu, 16 Mar 2023 00:57:21 GMT
RUN case "$(apk --print-arch)" in       x86_64)  arch=amd64 ;;       aarch64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     cp "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}/influx" /usr/local/bin/influx &&     rm -rf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     influx version
# Thu, 16 Mar 2023 00:57:22 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Thu, 16 Mar 2023 00:57:22 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Thu, 16 Mar 2023 00:57:22 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Thu, 16 Mar 2023 00:57:22 GMT
COPY file:708cccb15c29f10eb0c29e47f1c676d76b8ea9be434cce106ef95a7ba844bb2c in /entrypoint.sh 
# Thu, 16 Mar 2023 00:57:22 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 16 Mar 2023 00:57:22 GMT
CMD ["influxd"]
# Thu, 16 Mar 2023 00:57:22 GMT
EXPOSE 8086
# Thu, 16 Mar 2023 00:57:22 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Thu, 16 Mar 2023 00:57:23 GMT
ENV INFLUXD_INIT_PORT=9999
# Thu, 16 Mar 2023 00:57:23 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Thu, 16 Mar 2023 00:57:23 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:63b65145d645c1250c391b2d16ebe53b3747c295ca8ba2fcb6b0cf064a4dc21c`  
		Last Modified: Fri, 10 Feb 2023 22:41:31 GMT  
		Size: 3.4 MB (3374446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69b7a2cbfc2f3b3305293d689573f3c9651d6053e5f780a9ba42a4c836d8d6c9`  
		Last Modified: Mon, 13 Mar 2023 23:21:18 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9662dafd479312640e4852a3e8b4caa9c758e1d55e2177a988e8defb54fb3c4`  
		Last Modified: Thu, 16 Mar 2023 01:02:25 GMT  
		Size: 12.4 MB (12375014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cc9d593845c782b74273932afc2437f197ed7d05bc6d861ed3ac5f7d84da491`  
		Last Modified: Thu, 16 Mar 2023 01:02:24 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5752aeca8c552823e76ab58e99fd551721c4b38a0ac0871b7e5f1cf14a029b0`  
		Last Modified: Thu, 16 Mar 2023 01:02:29 GMT  
		Size: 92.9 MB (92899897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9ea5e8fc39fbbde89567d86def676e7c9f6e1a24bb83295bf60483ea1ced1ee`  
		Last Modified: Thu, 16 Mar 2023 01:02:23 GMT  
		Size: 6.1 MB (6073114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75c18bedddfdbccd0ecaf4b2477d2ff6a05025928771c575c05eeecc0e477388`  
		Last Modified: Thu, 16 Mar 2023 01:02:22 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21e813712bd5c3d8e52e6f4a1d0813dfecd1d6967baa8f6b2cc0793474c82fa3`  
		Last Modified: Thu, 16 Mar 2023 01:02:21 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9ff84c115204ae9cb222ecf853e6ad53697a26f6e1aabc6c391db9ebc88aa6e`  
		Last Modified: Thu, 16 Mar 2023 01:02:22 GMT  
		Size: 6.4 KB (6442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:2.4.0-alpine` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:9ec0c7a67d2c3f6e36325858423c6c01b9d4b1ba6560fc101487ed04ea2c50eb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **112.1 MB (112127015 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:47392e61808b63c1a3d5cbf76b5650719d35bbac9310de4fabe8c8cf140cd185`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:08 GMT
ADD file:9bd9ea42a9f3bdc769e80c6b8a4b117d65f73ae68e155a6172a1184e7ac8bcc1 in / 
# Fri, 10 Feb 2023 21:24:08 GMT
CMD ["/bin/sh"]
# Mon, 13 Mar 2023 23:47:18 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 15 Mar 2023 23:41:30 GMT
RUN apk add --no-cache       bash       ca-certificates       curl       gnupg       run-parts       su-exec       tzdata       yq &&     update-ca-certificates
# Wed, 15 Mar 2023 23:41:31 GMT
RUN addgroup -S -g 1000 influxdb &&     adduser -S -G influxdb -u 1000 -h /home/influxdb -s /bin/sh influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Wed, 15 Mar 2023 23:41:31 GMT
ENV INFLUXDB_VERSION=2.4.0
# Wed, 15 Mar 2023 23:41:35 GMT
RUN case "$(apk --print-arch)" in       x86_64)  arch=amd64 ;;       aarch64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&    curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     cp "influxdb2_linux_${arch}/influxd" /usr/local/bin/influxd &&     rm -rf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"            "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"            "influxdb2_linux_${arch}" &&     influxd version
# Wed, 15 Mar 2023 23:41:36 GMT
ENV INFLUX_CLI_VERSION=2.4.0
# Wed, 15 Mar 2023 23:41:38 GMT
RUN case "$(apk --print-arch)" in       x86_64)  arch=amd64 ;;       aarch64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     cp "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}/influx" /usr/local/bin/influx &&     rm -rf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     influx version
# Wed, 15 Mar 2023 23:41:38 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Wed, 15 Mar 2023 23:41:38 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Wed, 15 Mar 2023 23:41:39 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Wed, 15 Mar 2023 23:41:39 GMT
COPY file:708cccb15c29f10eb0c29e47f1c676d76b8ea9be434cce106ef95a7ba844bb2c in /entrypoint.sh 
# Wed, 15 Mar 2023 23:41:39 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 15 Mar 2023 23:41:39 GMT
CMD ["influxd"]
# Wed, 15 Mar 2023 23:41:39 GMT
EXPOSE 8086
# Wed, 15 Mar 2023 23:41:39 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Wed, 15 Mar 2023 23:41:39 GMT
ENV INFLUXD_INIT_PORT=9999
# Wed, 15 Mar 2023 23:41:39 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Wed, 15 Mar 2023 23:41:39 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:af6eaf76a39c2d3e7e0b8a0420486e3df33c4027d696c076a99a3d0ac09026af`  
		Last Modified: Fri, 10 Feb 2023 21:24:39 GMT  
		Size: 3.3 MB (3261959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dab1c38052d53938443512e37031810a03849aec98af5976a010b92ee4c13c1`  
		Last Modified: Mon, 13 Mar 2023 23:48:01 GMT  
		Size: 282.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd8e20b18f6688b37abc667eef7975eb77966987c3212d862a3b74b1e5a46151`  
		Last Modified: Wed, 15 Mar 2023 23:43:14 GMT  
		Size: 12.0 MB (12028387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:355a214bdc1929ff97f235f78bbe4313aa1f932134f19887c12d346d935da41e`  
		Last Modified: Wed, 15 Mar 2023 23:43:12 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2838674c2f9c183dc57cb7df56bdb750d889101e8dac0891cde3a2a4da77be0e`  
		Last Modified: Wed, 15 Mar 2023 23:43:16 GMT  
		Size: 91.2 MB (91223657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99c7fa0e61c0abdf5737711c7773876ff492bfcdb531a7bf8df3de30e1c6c491`  
		Last Modified: Wed, 15 Mar 2023 23:43:11 GMT  
		Size: 5.6 MB (5604482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:868fc0f0dc38e81c34af1ec71ff2071c9ec66ff81b6518bba94bb1c9e4b315bc`  
		Last Modified: Wed, 15 Mar 2023 23:43:10 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a99651d10b3c65f8e9e95531f448955b6abed3ddd329e22a4263c6404c51c401`  
		Last Modified: Wed, 15 Mar 2023 23:43:10 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a85002e06f2f9431c2f48da51407830849c5d6a67dceb068a4734ee31d39e849`  
		Last Modified: Wed, 15 Mar 2023 23:43:10 GMT  
		Size: 6.4 KB (6441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:2.5`

```console
$ docker pull influxdb@sha256:2afaacd5e947d1c44fc234740b17c9e39d7a82da692fbeaef3c9b0376748fbf3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:2.5` - linux; amd64

```console
$ docker pull influxdb@sha256:3d80813ce369e209785fcfa441aacbb31dabd21d3c91367ebf1eebcf8a6efc25
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.1 MB (99107385 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:305d84cc039e06d1f8379f18f1b4acc12b75a629e190373c2691b042f5fe6dd7`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 01 Mar 2023 04:09:58 GMT
ADD file:493a5b0c8d2d63a1343258b3f9aa5fcd59a93f44fe26ad9e56b094c3a08fd3be in / 
# Wed, 01 Mar 2023 04:09:59 GMT
CMD ["bash"]
# Thu, 16 Mar 2023 00:56:52 GMT
RUN export DEBIAN_FRONTEND=noninteractive &&     apt-get update -y &&     apt-get install -y --no-install-recommends       ca-certificates       curl       gnupg &&     apt-get clean &&     rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 00:56:53 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     curl -fLo /usr/local/bin/yq "https://github.com/mikefarah/yq/releases/download/v4.30.8/yq_linux_${arch}" &&     case ${arch} in       amd64) echo '6c911103e0dcc54e2ba07e767d2d62bcfc77452b39ebaee45b1c46f062f4fd26 /usr/local/bin/yq' ;;       arm64) echo '95092e8b5332890c46689679b5e4360d96873c025ad8bafd961688f28ea434c7 /usr/local/bin/yq' ;;     esac | sha256sum -c - &&     chmod +x /usr/local/bin/yq &&     yq --version
# Thu, 16 Mar 2023 00:56:53 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --create-home --home-dir=/home/influxdb --shell=/bin/bash influxdb
# Thu, 16 Mar 2023 00:56:53 GMT
ENV GOSU_VER=1.12
# Thu, 16 Mar 2023 00:56:56 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       B42F6819007F00F88E364FD4036A9C25BF357DD4 &&     curl -fLo /usr/local/bin/gosu     "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-${arch}"          -fLo /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-${arch}.asc" &&     gpg --batch --verify /usr/local/bin/gosu.asc                          /usr/local/bin/gosu &&     rm -rf /usr/local/bin/gosu.asc &&     chmod +x /usr/local/bin/gosu &&     gosu --version &&     gosu nobody true
# Thu, 16 Mar 2023 00:57:26 GMT
ENV INFLUXDB_VERSION=2.5.1
# Thu, 16 Mar 2023 00:57:29 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     cp "influxdb2_linux_${arch}/influxd" /usr/local/bin/influxd &&     rm -rf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"            "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"            "influxdb2_linux_${arch}" &&     influxd version
# Thu, 16 Mar 2023 00:57:29 GMT
ENV INFLUX_CLI_VERSION=2.5.0
# Thu, 16 Mar 2023 00:57:32 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     cp "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}/influx" /usr/local/bin/influx &&     rm -rf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     influx version
# Thu, 16 Mar 2023 00:57:32 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Thu, 16 Mar 2023 00:57:32 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Thu, 16 Mar 2023 00:57:33 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Thu, 16 Mar 2023 00:57:33 GMT
COPY file:595a669a2c2c2f47df93700fcd3e412750aae40abb979bb4af48a89af97a8b72 in /entrypoint.sh 
# Thu, 16 Mar 2023 00:57:33 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 16 Mar 2023 00:57:33 GMT
CMD ["influxd"]
# Thu, 16 Mar 2023 00:57:33 GMT
EXPOSE 8086
# Thu, 16 Mar 2023 00:57:33 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Thu, 16 Mar 2023 00:57:33 GMT
ENV INFLUXD_INIT_PORT=9999
# Thu, 16 Mar 2023 00:57:33 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Thu, 16 Mar 2023 00:57:33 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:3f9582a2cbe7197f39185419c0ced2c986389f8fc6aa805e1f5c090eea6511e0`  
		Last Modified: Wed, 01 Mar 2023 04:14:23 GMT  
		Size: 31.4 MB (31411403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08a794c78d7ad502e285244fde2dd7768065af2038670e7f34208e22d1c857e2`  
		Last Modified: Thu, 16 Mar 2023 01:02:10 GMT  
		Size: 6.3 MB (6327743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acd90bd5b5e60e8373c43b82a755b742e62d469c7df42aef9ab6ad0ac943ef6b`  
		Last Modified: Thu, 16 Mar 2023 01:02:09 GMT  
		Size: 7.0 MB (7049181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a549c3bac6c035d00d970ff0a7c39398de5b5355e5264970174a609dfcb350c1`  
		Last Modified: Thu, 16 Mar 2023 01:02:08 GMT  
		Size: 4.1 KB (4117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d52f68e8e59a067e13373eed04aa01fa28f3e99320d3ccfb46232c85efe7432`  
		Last Modified: Thu, 16 Mar 2023 01:02:08 GMT  
		Size: 982.0 KB (982043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2ea9d86f27540acd39611a86833c801157538b4f2c6cc79bfea236b46c16587`  
		Last Modified: Thu, 16 Mar 2023 01:02:43 GMT  
		Size: 47.2 MB (47217041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c33eec339657a27f65ed31b33b9b252509350beca52b3f0151ff6487b7a38b45`  
		Last Modified: Thu, 16 Mar 2023 01:02:39 GMT  
		Size: 6.1 MB (6108858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50e00287dd3920c7753b93797e35692443c37086701100f297e42f4269825c8d`  
		Last Modified: Thu, 16 Mar 2023 01:02:38 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cac3c34a4c3527bd81a7cda44f923bf75a6545c1802240348a8a56624a31fd1`  
		Last Modified: Thu, 16 Mar 2023 01:02:38 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:752ec4a7cc2c8a8d0219c80972d3d987315d4f2e9a1a7562d31880a5d143dd1a`  
		Last Modified: Thu, 16 Mar 2023 01:02:38 GMT  
		Size: 6.5 KB (6463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:2.5` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:1dc15c67c682303abba9e2e975d775c45f7acf8e8820bcc09599920a64c15ff1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.1 MB (95107563 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:11731aa5aa59ca69213f8b942b775d47fd8a3d1ec471dcc80e66f918aab5f82e`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 01 Mar 2023 02:20:39 GMT
ADD file:9dc5c6fb6431df80107eddb76fb18256d6f4a06b4b22f9a7c4bcd58476068186 in / 
# Wed, 01 Mar 2023 02:20:39 GMT
CMD ["bash"]
# Wed, 15 Mar 2023 23:41:07 GMT
RUN export DEBIAN_FRONTEND=noninteractive &&     apt-get update -y &&     apt-get install -y --no-install-recommends       ca-certificates       curl       gnupg &&     apt-get clean &&     rm -rf /var/lib/apt/lists/*
# Wed, 15 Mar 2023 23:41:08 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     curl -fLo /usr/local/bin/yq "https://github.com/mikefarah/yq/releases/download/v4.30.8/yq_linux_${arch}" &&     case ${arch} in       amd64) echo '6c911103e0dcc54e2ba07e767d2d62bcfc77452b39ebaee45b1c46f062f4fd26 /usr/local/bin/yq' ;;       arm64) echo '95092e8b5332890c46689679b5e4360d96873c025ad8bafd961688f28ea434c7 /usr/local/bin/yq' ;;     esac | sha256sum -c - &&     chmod +x /usr/local/bin/yq &&     yq --version
# Wed, 15 Mar 2023 23:41:09 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --create-home --home-dir=/home/influxdb --shell=/bin/bash influxdb
# Wed, 15 Mar 2023 23:41:09 GMT
ENV GOSU_VER=1.12
# Wed, 15 Mar 2023 23:41:11 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       B42F6819007F00F88E364FD4036A9C25BF357DD4 &&     curl -fLo /usr/local/bin/gosu     "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-${arch}"          -fLo /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-${arch}.asc" &&     gpg --batch --verify /usr/local/bin/gosu.asc                          /usr/local/bin/gosu &&     rm -rf /usr/local/bin/gosu.asc &&     chmod +x /usr/local/bin/gosu &&     gosu --version &&     gosu nobody true
# Wed, 15 Mar 2023 23:41:42 GMT
ENV INFLUXDB_VERSION=2.5.1
# Wed, 15 Mar 2023 23:41:47 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     cp "influxdb2_linux_${arch}/influxd" /usr/local/bin/influxd &&     rm -rf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"            "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"            "influxdb2_linux_${arch}" &&     influxd version
# Wed, 15 Mar 2023 23:41:47 GMT
ENV INFLUX_CLI_VERSION=2.5.0
# Wed, 15 Mar 2023 23:41:50 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     cp "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}/influx" /usr/local/bin/influx &&     rm -rf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     influx version
# Wed, 15 Mar 2023 23:41:50 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Wed, 15 Mar 2023 23:41:50 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Wed, 15 Mar 2023 23:41:50 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Wed, 15 Mar 2023 23:41:51 GMT
COPY file:595a669a2c2c2f47df93700fcd3e412750aae40abb979bb4af48a89af97a8b72 in /entrypoint.sh 
# Wed, 15 Mar 2023 23:41:51 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 15 Mar 2023 23:41:51 GMT
CMD ["influxd"]
# Wed, 15 Mar 2023 23:41:51 GMT
EXPOSE 8086
# Wed, 15 Mar 2023 23:41:51 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Wed, 15 Mar 2023 23:41:51 GMT
ENV INFLUXD_INIT_PORT=9999
# Wed, 15 Mar 2023 23:41:51 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Wed, 15 Mar 2023 23:41:51 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:66dbba0fb1b568cc3ffd53409ba2f9f82995ab7f80e379338f3f36e4dcd223be`  
		Last Modified: Wed, 01 Mar 2023 02:24:17 GMT  
		Size: 30.1 MB (30062814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65fd6db03d5e7efd9c898c05fa431254e6753c9d39caf9a942d187e791ef698e`  
		Last Modified: Wed, 15 Mar 2023 23:42:58 GMT  
		Size: 6.3 MB (6308600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:623e77e647b06d59d840fce37c059b20aa366a51af80637fd63e1e5512a9e5e6`  
		Last Modified: Wed, 15 Mar 2023 23:42:57 GMT  
		Size: 6.6 MB (6643045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4316c8eeb27a0e8e1b5c0adabd0c1c7a915c9dfda919151dea2c1f0fbd9b5b8d`  
		Last Modified: Wed, 15 Mar 2023 23:42:57 GMT  
		Size: 4.1 KB (4124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ed509fbb0848d068923c7c2fb0326172783db14b7e706111aa8d36fef0724e1`  
		Last Modified: Wed, 15 Mar 2023 23:42:57 GMT  
		Size: 916.9 KB (916930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a273690cf942de9b2fd921d5d105eb972972f327d5c78bf38cd0dddd9a19d14f`  
		Last Modified: Wed, 15 Mar 2023 23:43:28 GMT  
		Size: 45.5 MB (45530974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d70f8059ce319d4b529822be271486ffc3bd274d0fad0b25cfefdf7ef6027c23`  
		Last Modified: Wed, 15 Mar 2023 23:43:25 GMT  
		Size: 5.6 MB (5634078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d08e1dc9964922a5b45305b97cb04340a170431002aad3ae356a9b32954d1f3d`  
		Last Modified: Wed, 15 Mar 2023 23:43:24 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de4bc3ce6213b2c683379c83b6b77176fc51378e7f219f9f71d24d5afe43d2b7`  
		Last Modified: Wed, 15 Mar 2023 23:43:24 GMT  
		Size: 258.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc8218aafa4a06fa36348daa91e89e6ef2dbf50a3077d90587a16d18f6ff711e`  
		Last Modified: Wed, 15 Mar 2023 23:43:24 GMT  
		Size: 6.5 KB (6464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:2.5-alpine`

```console
$ docker pull influxdb@sha256:60dc79de01939092d62e1d17303b155fc679cdb5206c9373262bf80a1508fcfe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:2.5-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:d9f93c74fdbd36a7642473580465ce297efcc5acd054d203b2816cfc2f93c7b7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.1 MB (69083795 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:65e6a0f1814654bc9b5d73a7df985b67d2fc4fb235ee757386070442d4bb58b4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:42 GMT
ADD file:40887ab7c06977737e63c215c9bd297c0c74de8d12d16ebdf1c3d40ac392f62d in / 
# Sat, 11 Feb 2023 04:46:42 GMT
CMD ["/bin/sh"]
# Mon, 13 Mar 2023 23:20:24 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 16 Mar 2023 00:57:14 GMT
RUN apk add --no-cache       bash       ca-certificates       curl       gnupg       run-parts       su-exec       tzdata       yq &&     update-ca-certificates
# Thu, 16 Mar 2023 00:57:14 GMT
RUN addgroup -S -g 1000 influxdb &&     adduser -S -G influxdb -u 1000 -h /home/influxdb -s /bin/sh influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Thu, 16 Mar 2023 00:57:36 GMT
ENV INFLUXDB_VERSION=2.5.1
# Thu, 16 Mar 2023 00:57:40 GMT
RUN case "$(apk --print-arch)" in       x86_64)  arch=amd64 ;;       aarch64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&    curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     cp "influxdb2_linux_${arch}/influxd" /usr/local/bin/influxd &&     rm -rf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"            "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"            "influxdb2_linux_${arch}" &&     influxd version
# Thu, 16 Mar 2023 00:57:40 GMT
ENV INFLUX_CLI_VERSION=2.5.0
# Thu, 16 Mar 2023 00:57:42 GMT
RUN case "$(apk --print-arch)" in       x86_64)  arch=amd64 ;;       aarch64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     cp "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}/influx" /usr/local/bin/influx &&     rm -rf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     influx version
# Thu, 16 Mar 2023 00:57:42 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Thu, 16 Mar 2023 00:57:42 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Thu, 16 Mar 2023 00:57:42 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Thu, 16 Mar 2023 00:57:43 GMT
COPY file:708cccb15c29f10eb0c29e47f1c676d76b8ea9be434cce106ef95a7ba844bb2c in /entrypoint.sh 
# Thu, 16 Mar 2023 00:57:43 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 16 Mar 2023 00:57:43 GMT
CMD ["influxd"]
# Thu, 16 Mar 2023 00:57:43 GMT
EXPOSE 8086
# Thu, 16 Mar 2023 00:57:43 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Thu, 16 Mar 2023 00:57:43 GMT
ENV INFLUXD_INIT_PORT=9999
# Thu, 16 Mar 2023 00:57:43 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Thu, 16 Mar 2023 00:57:43 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:63b65145d645c1250c391b2d16ebe53b3747c295ca8ba2fcb6b0cf064a4dc21c`  
		Last Modified: Fri, 10 Feb 2023 22:41:31 GMT  
		Size: 3.4 MB (3374446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69b7a2cbfc2f3b3305293d689573f3c9651d6053e5f780a9ba42a4c836d8d6c9`  
		Last Modified: Mon, 13 Mar 2023 23:21:18 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9662dafd479312640e4852a3e8b4caa9c758e1d55e2177a988e8defb54fb3c4`  
		Last Modified: Thu, 16 Mar 2023 01:02:25 GMT  
		Size: 12.4 MB (12375014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cc9d593845c782b74273932afc2437f197ed7d05bc6d861ed3ac5f7d84da491`  
		Last Modified: Thu, 16 Mar 2023 01:02:24 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7426b3d232a8b299b181b69254630c25706a939c566007178c9a7196d8352b43`  
		Last Modified: Thu, 16 Mar 2023 01:02:58 GMT  
		Size: 47.2 MB (47216952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80deb5d640c36028b08da60cbc64f026b262bcd21097e641059282fb0afb058f`  
		Last Modified: Thu, 16 Mar 2023 01:02:53 GMT  
		Size: 6.1 MB (6108860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:928955f1a94ad77e83e667606bab8a42782e906e72f5322f43b361996918e5ae`  
		Last Modified: Thu, 16 Mar 2023 01:02:52 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c16992ae71ae2b04ed638e4aebf50cf2edc9fe1d9f42feebb0525c23b7b6ae8`  
		Last Modified: Thu, 16 Mar 2023 01:02:52 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b946cb2dd953f317125aef6d8dc99b9ecf114c1256e909b573b3500d20228d2e`  
		Last Modified: Thu, 16 Mar 2023 01:02:53 GMT  
		Size: 6.4 KB (6439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:2.5-alpine` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:3eea8ef5c0811479126fec2ff6c2b2056b4df063555b5d289355a85ed9e1c7a4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.5 MB (66463992 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8d458d6d18b35b35af68a227d2bd7a5cdafcf6923ca333c076f635a6adeb738b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:08 GMT
ADD file:9bd9ea42a9f3bdc769e80c6b8a4b117d65f73ae68e155a6172a1184e7ac8bcc1 in / 
# Fri, 10 Feb 2023 21:24:08 GMT
CMD ["/bin/sh"]
# Mon, 13 Mar 2023 23:47:18 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 15 Mar 2023 23:41:30 GMT
RUN apk add --no-cache       bash       ca-certificates       curl       gnupg       run-parts       su-exec       tzdata       yq &&     update-ca-certificates
# Wed, 15 Mar 2023 23:41:31 GMT
RUN addgroup -S -g 1000 influxdb &&     adduser -S -G influxdb -u 1000 -h /home/influxdb -s /bin/sh influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Wed, 15 Mar 2023 23:41:53 GMT
ENV INFLUXDB_VERSION=2.5.1
# Wed, 15 Mar 2023 23:41:56 GMT
RUN case "$(apk --print-arch)" in       x86_64)  arch=amd64 ;;       aarch64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&    curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     cp "influxdb2_linux_${arch}/influxd" /usr/local/bin/influxd &&     rm -rf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"            "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"            "influxdb2_linux_${arch}" &&     influxd version
# Wed, 15 Mar 2023 23:41:57 GMT
ENV INFLUX_CLI_VERSION=2.5.0
# Wed, 15 Mar 2023 23:41:58 GMT
RUN case "$(apk --print-arch)" in       x86_64)  arch=amd64 ;;       aarch64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     cp "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}/influx" /usr/local/bin/influx &&     rm -rf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     influx version
# Wed, 15 Mar 2023 23:41:59 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Wed, 15 Mar 2023 23:41:59 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Wed, 15 Mar 2023 23:41:59 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Wed, 15 Mar 2023 23:41:59 GMT
COPY file:708cccb15c29f10eb0c29e47f1c676d76b8ea9be434cce106ef95a7ba844bb2c in /entrypoint.sh 
# Wed, 15 Mar 2023 23:41:59 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 15 Mar 2023 23:41:59 GMT
CMD ["influxd"]
# Wed, 15 Mar 2023 23:41:59 GMT
EXPOSE 8086
# Wed, 15 Mar 2023 23:41:59 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Wed, 15 Mar 2023 23:41:59 GMT
ENV INFLUXD_INIT_PORT=9999
# Wed, 15 Mar 2023 23:42:00 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Wed, 15 Mar 2023 23:42:00 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:af6eaf76a39c2d3e7e0b8a0420486e3df33c4027d696c076a99a3d0ac09026af`  
		Last Modified: Fri, 10 Feb 2023 21:24:39 GMT  
		Size: 3.3 MB (3261959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dab1c38052d53938443512e37031810a03849aec98af5976a010b92ee4c13c1`  
		Last Modified: Mon, 13 Mar 2023 23:48:01 GMT  
		Size: 282.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd8e20b18f6688b37abc667eef7975eb77966987c3212d862a3b74b1e5a46151`  
		Last Modified: Wed, 15 Mar 2023 23:43:14 GMT  
		Size: 12.0 MB (12028387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:355a214bdc1929ff97f235f78bbe4313aa1f932134f19887c12d346d935da41e`  
		Last Modified: Wed, 15 Mar 2023 23:43:12 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2777196a705a2a282c40f8bc0817e7cb766798e4d4e0773d30e5b694682a8b86`  
		Last Modified: Wed, 15 Mar 2023 23:43:40 GMT  
		Size: 45.5 MB (45531047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa7debdcd18a4d1c16394c9c83956143acbb937a20ab72a99e5810a4fff9109c`  
		Last Modified: Wed, 15 Mar 2023 23:43:37 GMT  
		Size: 5.6 MB (5634069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6200d4bd08422da34a5e2256a45186b2e4c602656daed6c854baef545826ed4`  
		Last Modified: Wed, 15 Mar 2023 23:43:37 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:216535258a8063414110bcf3bb6fb5e969449290000892a4fb5c0750a7bf09e9`  
		Last Modified: Wed, 15 Mar 2023 23:43:37 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17d22f961f3e0d89443aae80f3f28d99e0e39036cbc74187aed87c2213231e46`  
		Last Modified: Wed, 15 Mar 2023 23:43:37 GMT  
		Size: 6.4 KB (6442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:2.5.1`

```console
$ docker pull influxdb@sha256:2afaacd5e947d1c44fc234740b17c9e39d7a82da692fbeaef3c9b0376748fbf3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:2.5.1` - linux; amd64

```console
$ docker pull influxdb@sha256:3d80813ce369e209785fcfa441aacbb31dabd21d3c91367ebf1eebcf8a6efc25
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.1 MB (99107385 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:305d84cc039e06d1f8379f18f1b4acc12b75a629e190373c2691b042f5fe6dd7`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 01 Mar 2023 04:09:58 GMT
ADD file:493a5b0c8d2d63a1343258b3f9aa5fcd59a93f44fe26ad9e56b094c3a08fd3be in / 
# Wed, 01 Mar 2023 04:09:59 GMT
CMD ["bash"]
# Thu, 16 Mar 2023 00:56:52 GMT
RUN export DEBIAN_FRONTEND=noninteractive &&     apt-get update -y &&     apt-get install -y --no-install-recommends       ca-certificates       curl       gnupg &&     apt-get clean &&     rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 00:56:53 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     curl -fLo /usr/local/bin/yq "https://github.com/mikefarah/yq/releases/download/v4.30.8/yq_linux_${arch}" &&     case ${arch} in       amd64) echo '6c911103e0dcc54e2ba07e767d2d62bcfc77452b39ebaee45b1c46f062f4fd26 /usr/local/bin/yq' ;;       arm64) echo '95092e8b5332890c46689679b5e4360d96873c025ad8bafd961688f28ea434c7 /usr/local/bin/yq' ;;     esac | sha256sum -c - &&     chmod +x /usr/local/bin/yq &&     yq --version
# Thu, 16 Mar 2023 00:56:53 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --create-home --home-dir=/home/influxdb --shell=/bin/bash influxdb
# Thu, 16 Mar 2023 00:56:53 GMT
ENV GOSU_VER=1.12
# Thu, 16 Mar 2023 00:56:56 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       B42F6819007F00F88E364FD4036A9C25BF357DD4 &&     curl -fLo /usr/local/bin/gosu     "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-${arch}"          -fLo /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-${arch}.asc" &&     gpg --batch --verify /usr/local/bin/gosu.asc                          /usr/local/bin/gosu &&     rm -rf /usr/local/bin/gosu.asc &&     chmod +x /usr/local/bin/gosu &&     gosu --version &&     gosu nobody true
# Thu, 16 Mar 2023 00:57:26 GMT
ENV INFLUXDB_VERSION=2.5.1
# Thu, 16 Mar 2023 00:57:29 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     cp "influxdb2_linux_${arch}/influxd" /usr/local/bin/influxd &&     rm -rf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"            "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"            "influxdb2_linux_${arch}" &&     influxd version
# Thu, 16 Mar 2023 00:57:29 GMT
ENV INFLUX_CLI_VERSION=2.5.0
# Thu, 16 Mar 2023 00:57:32 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     cp "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}/influx" /usr/local/bin/influx &&     rm -rf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     influx version
# Thu, 16 Mar 2023 00:57:32 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Thu, 16 Mar 2023 00:57:32 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Thu, 16 Mar 2023 00:57:33 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Thu, 16 Mar 2023 00:57:33 GMT
COPY file:595a669a2c2c2f47df93700fcd3e412750aae40abb979bb4af48a89af97a8b72 in /entrypoint.sh 
# Thu, 16 Mar 2023 00:57:33 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 16 Mar 2023 00:57:33 GMT
CMD ["influxd"]
# Thu, 16 Mar 2023 00:57:33 GMT
EXPOSE 8086
# Thu, 16 Mar 2023 00:57:33 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Thu, 16 Mar 2023 00:57:33 GMT
ENV INFLUXD_INIT_PORT=9999
# Thu, 16 Mar 2023 00:57:33 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Thu, 16 Mar 2023 00:57:33 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:3f9582a2cbe7197f39185419c0ced2c986389f8fc6aa805e1f5c090eea6511e0`  
		Last Modified: Wed, 01 Mar 2023 04:14:23 GMT  
		Size: 31.4 MB (31411403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08a794c78d7ad502e285244fde2dd7768065af2038670e7f34208e22d1c857e2`  
		Last Modified: Thu, 16 Mar 2023 01:02:10 GMT  
		Size: 6.3 MB (6327743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acd90bd5b5e60e8373c43b82a755b742e62d469c7df42aef9ab6ad0ac943ef6b`  
		Last Modified: Thu, 16 Mar 2023 01:02:09 GMT  
		Size: 7.0 MB (7049181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a549c3bac6c035d00d970ff0a7c39398de5b5355e5264970174a609dfcb350c1`  
		Last Modified: Thu, 16 Mar 2023 01:02:08 GMT  
		Size: 4.1 KB (4117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d52f68e8e59a067e13373eed04aa01fa28f3e99320d3ccfb46232c85efe7432`  
		Last Modified: Thu, 16 Mar 2023 01:02:08 GMT  
		Size: 982.0 KB (982043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2ea9d86f27540acd39611a86833c801157538b4f2c6cc79bfea236b46c16587`  
		Last Modified: Thu, 16 Mar 2023 01:02:43 GMT  
		Size: 47.2 MB (47217041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c33eec339657a27f65ed31b33b9b252509350beca52b3f0151ff6487b7a38b45`  
		Last Modified: Thu, 16 Mar 2023 01:02:39 GMT  
		Size: 6.1 MB (6108858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50e00287dd3920c7753b93797e35692443c37086701100f297e42f4269825c8d`  
		Last Modified: Thu, 16 Mar 2023 01:02:38 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cac3c34a4c3527bd81a7cda44f923bf75a6545c1802240348a8a56624a31fd1`  
		Last Modified: Thu, 16 Mar 2023 01:02:38 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:752ec4a7cc2c8a8d0219c80972d3d987315d4f2e9a1a7562d31880a5d143dd1a`  
		Last Modified: Thu, 16 Mar 2023 01:02:38 GMT  
		Size: 6.5 KB (6463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:2.5.1` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:1dc15c67c682303abba9e2e975d775c45f7acf8e8820bcc09599920a64c15ff1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.1 MB (95107563 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:11731aa5aa59ca69213f8b942b775d47fd8a3d1ec471dcc80e66f918aab5f82e`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 01 Mar 2023 02:20:39 GMT
ADD file:9dc5c6fb6431df80107eddb76fb18256d6f4a06b4b22f9a7c4bcd58476068186 in / 
# Wed, 01 Mar 2023 02:20:39 GMT
CMD ["bash"]
# Wed, 15 Mar 2023 23:41:07 GMT
RUN export DEBIAN_FRONTEND=noninteractive &&     apt-get update -y &&     apt-get install -y --no-install-recommends       ca-certificates       curl       gnupg &&     apt-get clean &&     rm -rf /var/lib/apt/lists/*
# Wed, 15 Mar 2023 23:41:08 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     curl -fLo /usr/local/bin/yq "https://github.com/mikefarah/yq/releases/download/v4.30.8/yq_linux_${arch}" &&     case ${arch} in       amd64) echo '6c911103e0dcc54e2ba07e767d2d62bcfc77452b39ebaee45b1c46f062f4fd26 /usr/local/bin/yq' ;;       arm64) echo '95092e8b5332890c46689679b5e4360d96873c025ad8bafd961688f28ea434c7 /usr/local/bin/yq' ;;     esac | sha256sum -c - &&     chmod +x /usr/local/bin/yq &&     yq --version
# Wed, 15 Mar 2023 23:41:09 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --create-home --home-dir=/home/influxdb --shell=/bin/bash influxdb
# Wed, 15 Mar 2023 23:41:09 GMT
ENV GOSU_VER=1.12
# Wed, 15 Mar 2023 23:41:11 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       B42F6819007F00F88E364FD4036A9C25BF357DD4 &&     curl -fLo /usr/local/bin/gosu     "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-${arch}"          -fLo /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-${arch}.asc" &&     gpg --batch --verify /usr/local/bin/gosu.asc                          /usr/local/bin/gosu &&     rm -rf /usr/local/bin/gosu.asc &&     chmod +x /usr/local/bin/gosu &&     gosu --version &&     gosu nobody true
# Wed, 15 Mar 2023 23:41:42 GMT
ENV INFLUXDB_VERSION=2.5.1
# Wed, 15 Mar 2023 23:41:47 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     cp "influxdb2_linux_${arch}/influxd" /usr/local/bin/influxd &&     rm -rf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"            "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"            "influxdb2_linux_${arch}" &&     influxd version
# Wed, 15 Mar 2023 23:41:47 GMT
ENV INFLUX_CLI_VERSION=2.5.0
# Wed, 15 Mar 2023 23:41:50 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     cp "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}/influx" /usr/local/bin/influx &&     rm -rf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     influx version
# Wed, 15 Mar 2023 23:41:50 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Wed, 15 Mar 2023 23:41:50 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Wed, 15 Mar 2023 23:41:50 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Wed, 15 Mar 2023 23:41:51 GMT
COPY file:595a669a2c2c2f47df93700fcd3e412750aae40abb979bb4af48a89af97a8b72 in /entrypoint.sh 
# Wed, 15 Mar 2023 23:41:51 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 15 Mar 2023 23:41:51 GMT
CMD ["influxd"]
# Wed, 15 Mar 2023 23:41:51 GMT
EXPOSE 8086
# Wed, 15 Mar 2023 23:41:51 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Wed, 15 Mar 2023 23:41:51 GMT
ENV INFLUXD_INIT_PORT=9999
# Wed, 15 Mar 2023 23:41:51 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Wed, 15 Mar 2023 23:41:51 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:66dbba0fb1b568cc3ffd53409ba2f9f82995ab7f80e379338f3f36e4dcd223be`  
		Last Modified: Wed, 01 Mar 2023 02:24:17 GMT  
		Size: 30.1 MB (30062814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65fd6db03d5e7efd9c898c05fa431254e6753c9d39caf9a942d187e791ef698e`  
		Last Modified: Wed, 15 Mar 2023 23:42:58 GMT  
		Size: 6.3 MB (6308600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:623e77e647b06d59d840fce37c059b20aa366a51af80637fd63e1e5512a9e5e6`  
		Last Modified: Wed, 15 Mar 2023 23:42:57 GMT  
		Size: 6.6 MB (6643045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4316c8eeb27a0e8e1b5c0adabd0c1c7a915c9dfda919151dea2c1f0fbd9b5b8d`  
		Last Modified: Wed, 15 Mar 2023 23:42:57 GMT  
		Size: 4.1 KB (4124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ed509fbb0848d068923c7c2fb0326172783db14b7e706111aa8d36fef0724e1`  
		Last Modified: Wed, 15 Mar 2023 23:42:57 GMT  
		Size: 916.9 KB (916930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a273690cf942de9b2fd921d5d105eb972972f327d5c78bf38cd0dddd9a19d14f`  
		Last Modified: Wed, 15 Mar 2023 23:43:28 GMT  
		Size: 45.5 MB (45530974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d70f8059ce319d4b529822be271486ffc3bd274d0fad0b25cfefdf7ef6027c23`  
		Last Modified: Wed, 15 Mar 2023 23:43:25 GMT  
		Size: 5.6 MB (5634078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d08e1dc9964922a5b45305b97cb04340a170431002aad3ae356a9b32954d1f3d`  
		Last Modified: Wed, 15 Mar 2023 23:43:24 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de4bc3ce6213b2c683379c83b6b77176fc51378e7f219f9f71d24d5afe43d2b7`  
		Last Modified: Wed, 15 Mar 2023 23:43:24 GMT  
		Size: 258.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc8218aafa4a06fa36348daa91e89e6ef2dbf50a3077d90587a16d18f6ff711e`  
		Last Modified: Wed, 15 Mar 2023 23:43:24 GMT  
		Size: 6.5 KB (6464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:2.5.1-alpine`

```console
$ docker pull influxdb@sha256:60dc79de01939092d62e1d17303b155fc679cdb5206c9373262bf80a1508fcfe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:2.5.1-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:d9f93c74fdbd36a7642473580465ce297efcc5acd054d203b2816cfc2f93c7b7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.1 MB (69083795 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:65e6a0f1814654bc9b5d73a7df985b67d2fc4fb235ee757386070442d4bb58b4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:42 GMT
ADD file:40887ab7c06977737e63c215c9bd297c0c74de8d12d16ebdf1c3d40ac392f62d in / 
# Sat, 11 Feb 2023 04:46:42 GMT
CMD ["/bin/sh"]
# Mon, 13 Mar 2023 23:20:24 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 16 Mar 2023 00:57:14 GMT
RUN apk add --no-cache       bash       ca-certificates       curl       gnupg       run-parts       su-exec       tzdata       yq &&     update-ca-certificates
# Thu, 16 Mar 2023 00:57:14 GMT
RUN addgroup -S -g 1000 influxdb &&     adduser -S -G influxdb -u 1000 -h /home/influxdb -s /bin/sh influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Thu, 16 Mar 2023 00:57:36 GMT
ENV INFLUXDB_VERSION=2.5.1
# Thu, 16 Mar 2023 00:57:40 GMT
RUN case "$(apk --print-arch)" in       x86_64)  arch=amd64 ;;       aarch64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&    curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     cp "influxdb2_linux_${arch}/influxd" /usr/local/bin/influxd &&     rm -rf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"            "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"            "influxdb2_linux_${arch}" &&     influxd version
# Thu, 16 Mar 2023 00:57:40 GMT
ENV INFLUX_CLI_VERSION=2.5.0
# Thu, 16 Mar 2023 00:57:42 GMT
RUN case "$(apk --print-arch)" in       x86_64)  arch=amd64 ;;       aarch64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     cp "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}/influx" /usr/local/bin/influx &&     rm -rf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     influx version
# Thu, 16 Mar 2023 00:57:42 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Thu, 16 Mar 2023 00:57:42 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Thu, 16 Mar 2023 00:57:42 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Thu, 16 Mar 2023 00:57:43 GMT
COPY file:708cccb15c29f10eb0c29e47f1c676d76b8ea9be434cce106ef95a7ba844bb2c in /entrypoint.sh 
# Thu, 16 Mar 2023 00:57:43 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 16 Mar 2023 00:57:43 GMT
CMD ["influxd"]
# Thu, 16 Mar 2023 00:57:43 GMT
EXPOSE 8086
# Thu, 16 Mar 2023 00:57:43 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Thu, 16 Mar 2023 00:57:43 GMT
ENV INFLUXD_INIT_PORT=9999
# Thu, 16 Mar 2023 00:57:43 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Thu, 16 Mar 2023 00:57:43 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:63b65145d645c1250c391b2d16ebe53b3747c295ca8ba2fcb6b0cf064a4dc21c`  
		Last Modified: Fri, 10 Feb 2023 22:41:31 GMT  
		Size: 3.4 MB (3374446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69b7a2cbfc2f3b3305293d689573f3c9651d6053e5f780a9ba42a4c836d8d6c9`  
		Last Modified: Mon, 13 Mar 2023 23:21:18 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9662dafd479312640e4852a3e8b4caa9c758e1d55e2177a988e8defb54fb3c4`  
		Last Modified: Thu, 16 Mar 2023 01:02:25 GMT  
		Size: 12.4 MB (12375014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cc9d593845c782b74273932afc2437f197ed7d05bc6d861ed3ac5f7d84da491`  
		Last Modified: Thu, 16 Mar 2023 01:02:24 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7426b3d232a8b299b181b69254630c25706a939c566007178c9a7196d8352b43`  
		Last Modified: Thu, 16 Mar 2023 01:02:58 GMT  
		Size: 47.2 MB (47216952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80deb5d640c36028b08da60cbc64f026b262bcd21097e641059282fb0afb058f`  
		Last Modified: Thu, 16 Mar 2023 01:02:53 GMT  
		Size: 6.1 MB (6108860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:928955f1a94ad77e83e667606bab8a42782e906e72f5322f43b361996918e5ae`  
		Last Modified: Thu, 16 Mar 2023 01:02:52 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c16992ae71ae2b04ed638e4aebf50cf2edc9fe1d9f42feebb0525c23b7b6ae8`  
		Last Modified: Thu, 16 Mar 2023 01:02:52 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b946cb2dd953f317125aef6d8dc99b9ecf114c1256e909b573b3500d20228d2e`  
		Last Modified: Thu, 16 Mar 2023 01:02:53 GMT  
		Size: 6.4 KB (6439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:2.5.1-alpine` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:3eea8ef5c0811479126fec2ff6c2b2056b4df063555b5d289355a85ed9e1c7a4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.5 MB (66463992 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8d458d6d18b35b35af68a227d2bd7a5cdafcf6923ca333c076f635a6adeb738b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:08 GMT
ADD file:9bd9ea42a9f3bdc769e80c6b8a4b117d65f73ae68e155a6172a1184e7ac8bcc1 in / 
# Fri, 10 Feb 2023 21:24:08 GMT
CMD ["/bin/sh"]
# Mon, 13 Mar 2023 23:47:18 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 15 Mar 2023 23:41:30 GMT
RUN apk add --no-cache       bash       ca-certificates       curl       gnupg       run-parts       su-exec       tzdata       yq &&     update-ca-certificates
# Wed, 15 Mar 2023 23:41:31 GMT
RUN addgroup -S -g 1000 influxdb &&     adduser -S -G influxdb -u 1000 -h /home/influxdb -s /bin/sh influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Wed, 15 Mar 2023 23:41:53 GMT
ENV INFLUXDB_VERSION=2.5.1
# Wed, 15 Mar 2023 23:41:56 GMT
RUN case "$(apk --print-arch)" in       x86_64)  arch=amd64 ;;       aarch64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&    curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     cp "influxdb2_linux_${arch}/influxd" /usr/local/bin/influxd &&     rm -rf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"            "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"            "influxdb2_linux_${arch}" &&     influxd version
# Wed, 15 Mar 2023 23:41:57 GMT
ENV INFLUX_CLI_VERSION=2.5.0
# Wed, 15 Mar 2023 23:41:58 GMT
RUN case "$(apk --print-arch)" in       x86_64)  arch=amd64 ;;       aarch64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     cp "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}/influx" /usr/local/bin/influx &&     rm -rf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     influx version
# Wed, 15 Mar 2023 23:41:59 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Wed, 15 Mar 2023 23:41:59 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Wed, 15 Mar 2023 23:41:59 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Wed, 15 Mar 2023 23:41:59 GMT
COPY file:708cccb15c29f10eb0c29e47f1c676d76b8ea9be434cce106ef95a7ba844bb2c in /entrypoint.sh 
# Wed, 15 Mar 2023 23:41:59 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 15 Mar 2023 23:41:59 GMT
CMD ["influxd"]
# Wed, 15 Mar 2023 23:41:59 GMT
EXPOSE 8086
# Wed, 15 Mar 2023 23:41:59 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Wed, 15 Mar 2023 23:41:59 GMT
ENV INFLUXD_INIT_PORT=9999
# Wed, 15 Mar 2023 23:42:00 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Wed, 15 Mar 2023 23:42:00 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:af6eaf76a39c2d3e7e0b8a0420486e3df33c4027d696c076a99a3d0ac09026af`  
		Last Modified: Fri, 10 Feb 2023 21:24:39 GMT  
		Size: 3.3 MB (3261959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dab1c38052d53938443512e37031810a03849aec98af5976a010b92ee4c13c1`  
		Last Modified: Mon, 13 Mar 2023 23:48:01 GMT  
		Size: 282.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd8e20b18f6688b37abc667eef7975eb77966987c3212d862a3b74b1e5a46151`  
		Last Modified: Wed, 15 Mar 2023 23:43:14 GMT  
		Size: 12.0 MB (12028387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:355a214bdc1929ff97f235f78bbe4313aa1f932134f19887c12d346d935da41e`  
		Last Modified: Wed, 15 Mar 2023 23:43:12 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2777196a705a2a282c40f8bc0817e7cb766798e4d4e0773d30e5b694682a8b86`  
		Last Modified: Wed, 15 Mar 2023 23:43:40 GMT  
		Size: 45.5 MB (45531047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa7debdcd18a4d1c16394c9c83956143acbb937a20ab72a99e5810a4fff9109c`  
		Last Modified: Wed, 15 Mar 2023 23:43:37 GMT  
		Size: 5.6 MB (5634069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6200d4bd08422da34a5e2256a45186b2e4c602656daed6c854baef545826ed4`  
		Last Modified: Wed, 15 Mar 2023 23:43:37 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:216535258a8063414110bcf3bb6fb5e969449290000892a4fb5c0750a7bf09e9`  
		Last Modified: Wed, 15 Mar 2023 23:43:37 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17d22f961f3e0d89443aae80f3f28d99e0e39036cbc74187aed87c2213231e46`  
		Last Modified: Wed, 15 Mar 2023 23:43:37 GMT  
		Size: 6.4 KB (6442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:2.6`

```console
$ docker pull influxdb@sha256:dfa86201228943d0ac8c3e675fc8e85843a872a9edeedb0b3fddf52e64414188
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:2.6` - linux; amd64

```console
$ docker pull influxdb@sha256:d9ea508f639968720934cc9dd727e83cd5515f87c7a35fec044728a455a9578b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **98.8 MB (98837218 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a023b77ee0d8d5dbfca34a91f77e165247c3017017b782924ce74aa7dcfde836`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 01 Mar 2023 04:09:58 GMT
ADD file:493a5b0c8d2d63a1343258b3f9aa5fcd59a93f44fe26ad9e56b094c3a08fd3be in / 
# Wed, 01 Mar 2023 04:09:59 GMT
CMD ["bash"]
# Thu, 16 Mar 2023 00:56:52 GMT
RUN export DEBIAN_FRONTEND=noninteractive &&     apt-get update -y &&     apt-get install -y --no-install-recommends       ca-certificates       curl       gnupg &&     apt-get clean &&     rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 00:56:53 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     curl -fLo /usr/local/bin/yq "https://github.com/mikefarah/yq/releases/download/v4.30.8/yq_linux_${arch}" &&     case ${arch} in       amd64) echo '6c911103e0dcc54e2ba07e767d2d62bcfc77452b39ebaee45b1c46f062f4fd26 /usr/local/bin/yq' ;;       arm64) echo '95092e8b5332890c46689679b5e4360d96873c025ad8bafd961688f28ea434c7 /usr/local/bin/yq' ;;     esac | sha256sum -c - &&     chmod +x /usr/local/bin/yq &&     yq --version
# Thu, 16 Mar 2023 00:56:53 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --create-home --home-dir=/home/influxdb --shell=/bin/bash influxdb
# Thu, 16 Mar 2023 00:56:53 GMT
ENV GOSU_VER=1.12
# Thu, 16 Mar 2023 00:56:56 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       B42F6819007F00F88E364FD4036A9C25BF357DD4 &&     curl -fLo /usr/local/bin/gosu     "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-${arch}"          -fLo /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-${arch}.asc" &&     gpg --batch --verify /usr/local/bin/gosu.asc                          /usr/local/bin/gosu &&     rm -rf /usr/local/bin/gosu.asc &&     chmod +x /usr/local/bin/gosu &&     gosu --version &&     gosu nobody true
# Thu, 16 Mar 2023 00:57:46 GMT
ENV INFLUXDB_VERSION=2.6.1
# Thu, 16 Mar 2023 00:57:50 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     cp "influxdb2_linux_${arch}/influxd" /usr/local/bin/influxd &&     rm -rf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"            "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"            "influxdb2_linux_${arch}" &&     influxd version
# Thu, 16 Mar 2023 00:57:50 GMT
ENV INFLUX_CLI_VERSION=2.6.1
# Thu, 16 Mar 2023 00:57:52 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     cp "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}/influx" /usr/local/bin/influx &&     rm -rf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     influx version
# Thu, 16 Mar 2023 00:57:53 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Thu, 16 Mar 2023 00:57:53 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Thu, 16 Mar 2023 00:57:53 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Thu, 16 Mar 2023 00:57:53 GMT
COPY file:595a669a2c2c2f47df93700fcd3e412750aae40abb979bb4af48a89af97a8b72 in /entrypoint.sh 
# Thu, 16 Mar 2023 00:57:53 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 16 Mar 2023 00:57:53 GMT
CMD ["influxd"]
# Thu, 16 Mar 2023 00:57:53 GMT
EXPOSE 8086
# Thu, 16 Mar 2023 00:57:53 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Thu, 16 Mar 2023 00:57:53 GMT
ENV INFLUXD_INIT_PORT=9999
# Thu, 16 Mar 2023 00:57:53 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Thu, 16 Mar 2023 00:57:53 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:3f9582a2cbe7197f39185419c0ced2c986389f8fc6aa805e1f5c090eea6511e0`  
		Last Modified: Wed, 01 Mar 2023 04:14:23 GMT  
		Size: 31.4 MB (31411403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08a794c78d7ad502e285244fde2dd7768065af2038670e7f34208e22d1c857e2`  
		Last Modified: Thu, 16 Mar 2023 01:02:10 GMT  
		Size: 6.3 MB (6327743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acd90bd5b5e60e8373c43b82a755b742e62d469c7df42aef9ab6ad0ac943ef6b`  
		Last Modified: Thu, 16 Mar 2023 01:02:09 GMT  
		Size: 7.0 MB (7049181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a549c3bac6c035d00d970ff0a7c39398de5b5355e5264970174a609dfcb350c1`  
		Last Modified: Thu, 16 Mar 2023 01:02:08 GMT  
		Size: 4.1 KB (4117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d52f68e8e59a067e13373eed04aa01fa28f3e99320d3ccfb46232c85efe7432`  
		Last Modified: Thu, 16 Mar 2023 01:02:08 GMT  
		Size: 982.0 KB (982043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48976d943c24ad838f918383f3fa1d1cbb1b40eb19d039b778c23ea46752a865`  
		Last Modified: Thu, 16 Mar 2023 01:03:12 GMT  
		Size: 46.8 MB (46844106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3539972aef6eac29878ccd083697a376eb1aec8d5e229b5c8a6dcab6036edea`  
		Last Modified: Thu, 16 Mar 2023 01:03:07 GMT  
		Size: 6.2 MB (6211626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bb00e5e812eae43c162c6884051314289a906fcf9e53e5c6e8578ad0f5c1c00`  
		Last Modified: Thu, 16 Mar 2023 01:03:06 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec172591e2a97b25dd5c54f835a03191efb469ea9b38708ac8c0d7c7dc16f764`  
		Last Modified: Thu, 16 Mar 2023 01:03:06 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca79f302ed0dd277dff382083d00f0d5d62349e4defa511a5a54753e2358b2f5`  
		Last Modified: Thu, 16 Mar 2023 01:03:06 GMT  
		Size: 6.5 KB (6462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:2.6` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:750f7ade153ce2c99e6a718d63a82e6ef50c9b80edf08de87406a128725d0ef0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.8 MB (94794365 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d965327ac4600487dce1bd0b2306373fc5b4ec9127b5274a7a4ca06c614dc065`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 01 Mar 2023 02:20:39 GMT
ADD file:9dc5c6fb6431df80107eddb76fb18256d6f4a06b4b22f9a7c4bcd58476068186 in / 
# Wed, 01 Mar 2023 02:20:39 GMT
CMD ["bash"]
# Wed, 15 Mar 2023 23:41:07 GMT
RUN export DEBIAN_FRONTEND=noninteractive &&     apt-get update -y &&     apt-get install -y --no-install-recommends       ca-certificates       curl       gnupg &&     apt-get clean &&     rm -rf /var/lib/apt/lists/*
# Wed, 15 Mar 2023 23:41:08 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     curl -fLo /usr/local/bin/yq "https://github.com/mikefarah/yq/releases/download/v4.30.8/yq_linux_${arch}" &&     case ${arch} in       amd64) echo '6c911103e0dcc54e2ba07e767d2d62bcfc77452b39ebaee45b1c46f062f4fd26 /usr/local/bin/yq' ;;       arm64) echo '95092e8b5332890c46689679b5e4360d96873c025ad8bafd961688f28ea434c7 /usr/local/bin/yq' ;;     esac | sha256sum -c - &&     chmod +x /usr/local/bin/yq &&     yq --version
# Wed, 15 Mar 2023 23:41:09 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --create-home --home-dir=/home/influxdb --shell=/bin/bash influxdb
# Wed, 15 Mar 2023 23:41:09 GMT
ENV GOSU_VER=1.12
# Wed, 15 Mar 2023 23:41:11 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       B42F6819007F00F88E364FD4036A9C25BF357DD4 &&     curl -fLo /usr/local/bin/gosu     "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-${arch}"          -fLo /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-${arch}.asc" &&     gpg --batch --verify /usr/local/bin/gosu.asc                          /usr/local/bin/gosu &&     rm -rf /usr/local/bin/gosu.asc &&     chmod +x /usr/local/bin/gosu &&     gosu --version &&     gosu nobody true
# Wed, 15 Mar 2023 23:42:03 GMT
ENV INFLUXDB_VERSION=2.6.1
# Wed, 15 Mar 2023 23:42:06 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     cp "influxdb2_linux_${arch}/influxd" /usr/local/bin/influxd &&     rm -rf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"            "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"            "influxdb2_linux_${arch}" &&     influxd version
# Wed, 15 Mar 2023 23:42:07 GMT
ENV INFLUX_CLI_VERSION=2.6.1
# Wed, 15 Mar 2023 23:42:09 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     cp "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}/influx" /usr/local/bin/influx &&     rm -rf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     influx version
# Wed, 15 Mar 2023 23:42:09 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Wed, 15 Mar 2023 23:42:10 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Wed, 15 Mar 2023 23:42:10 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Wed, 15 Mar 2023 23:42:10 GMT
COPY file:595a669a2c2c2f47df93700fcd3e412750aae40abb979bb4af48a89af97a8b72 in /entrypoint.sh 
# Wed, 15 Mar 2023 23:42:10 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 15 Mar 2023 23:42:10 GMT
CMD ["influxd"]
# Wed, 15 Mar 2023 23:42:10 GMT
EXPOSE 8086
# Wed, 15 Mar 2023 23:42:10 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Wed, 15 Mar 2023 23:42:10 GMT
ENV INFLUXD_INIT_PORT=9999
# Wed, 15 Mar 2023 23:42:10 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Wed, 15 Mar 2023 23:42:10 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:66dbba0fb1b568cc3ffd53409ba2f9f82995ab7f80e379338f3f36e4dcd223be`  
		Last Modified: Wed, 01 Mar 2023 02:24:17 GMT  
		Size: 30.1 MB (30062814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65fd6db03d5e7efd9c898c05fa431254e6753c9d39caf9a942d187e791ef698e`  
		Last Modified: Wed, 15 Mar 2023 23:42:58 GMT  
		Size: 6.3 MB (6308600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:623e77e647b06d59d840fce37c059b20aa366a51af80637fd63e1e5512a9e5e6`  
		Last Modified: Wed, 15 Mar 2023 23:42:57 GMT  
		Size: 6.6 MB (6643045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4316c8eeb27a0e8e1b5c0adabd0c1c7a915c9dfda919151dea2c1f0fbd9b5b8d`  
		Last Modified: Wed, 15 Mar 2023 23:42:57 GMT  
		Size: 4.1 KB (4124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ed509fbb0848d068923c7c2fb0326172783db14b7e706111aa8d36fef0724e1`  
		Last Modified: Wed, 15 Mar 2023 23:42:57 GMT  
		Size: 916.9 KB (916930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcd9f815af9fa7713836edcaf8c0edfede3b00c2f262af85dee43e3bf5706a89`  
		Last Modified: Wed, 15 Mar 2023 23:43:53 GMT  
		Size: 45.1 MB (45145851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15e98fd076597f7d2ddfa0871be33a56e936d19752c20858efc5f76b0fe57e03`  
		Last Modified: Wed, 15 Mar 2023 23:43:50 GMT  
		Size: 5.7 MB (5706001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4e1b9223729f0d3aebccfacb5a0b15c96af102a78398ac8b0df5cfa5329e7ed`  
		Last Modified: Wed, 15 Mar 2023 23:43:49 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc31e1ada9713c6aa0ae771c2ff4a99aeaa09bcd46114941d005d37a165d5c8d`  
		Last Modified: Wed, 15 Mar 2023 23:43:49 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74f654e5c408f27396570fc3ebb1bfee8bd77d4e2f82a808aa4ce8cd861ff0af`  
		Last Modified: Wed, 15 Mar 2023 23:43:49 GMT  
		Size: 6.5 KB (6463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:2.6-alpine`

```console
$ docker pull influxdb@sha256:0db3d6571a3b139112c8b414a87d78993dd4915180020363da791fedc392b849
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:2.6-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:8bd70537963442987876957f5cc9428d3eed5213a8c043745dc638960d64d21c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.8 MB (68813716 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:304c50024095f76a248b28dfde97abb90eb69dada8f80a11c5d463be8e61ef69`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:42 GMT
ADD file:40887ab7c06977737e63c215c9bd297c0c74de8d12d16ebdf1c3d40ac392f62d in / 
# Sat, 11 Feb 2023 04:46:42 GMT
CMD ["/bin/sh"]
# Mon, 13 Mar 2023 23:20:24 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 16 Mar 2023 00:57:14 GMT
RUN apk add --no-cache       bash       ca-certificates       curl       gnupg       run-parts       su-exec       tzdata       yq &&     update-ca-certificates
# Thu, 16 Mar 2023 00:57:14 GMT
RUN addgroup -S -g 1000 influxdb &&     adduser -S -G influxdb -u 1000 -h /home/influxdb -s /bin/sh influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Thu, 16 Mar 2023 00:57:57 GMT
ENV INFLUXDB_VERSION=2.6.1
# Thu, 16 Mar 2023 00:58:00 GMT
RUN case "$(apk --print-arch)" in       x86_64)  arch=amd64 ;;       aarch64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&    curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     cp "influxdb2_linux_${arch}/influxd" /usr/local/bin/influxd &&     rm -rf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"            "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"            "influxdb2_linux_${arch}" &&     influxd version
# Thu, 16 Mar 2023 00:58:01 GMT
ENV INFLUX_CLI_VERSION=2.6.1
# Thu, 16 Mar 2023 00:58:02 GMT
RUN case "$(apk --print-arch)" in       x86_64)  arch=amd64 ;;       aarch64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     cp "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}/influx" /usr/local/bin/influx &&     rm -rf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     influx version
# Thu, 16 Mar 2023 00:58:03 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Thu, 16 Mar 2023 00:58:03 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Thu, 16 Mar 2023 00:58:03 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Thu, 16 Mar 2023 00:58:03 GMT
COPY file:708cccb15c29f10eb0c29e47f1c676d76b8ea9be434cce106ef95a7ba844bb2c in /entrypoint.sh 
# Thu, 16 Mar 2023 00:58:03 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 16 Mar 2023 00:58:03 GMT
CMD ["influxd"]
# Thu, 16 Mar 2023 00:58:03 GMT
EXPOSE 8086
# Thu, 16 Mar 2023 00:58:03 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Thu, 16 Mar 2023 00:58:03 GMT
ENV INFLUXD_INIT_PORT=9999
# Thu, 16 Mar 2023 00:58:04 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Thu, 16 Mar 2023 00:58:04 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:63b65145d645c1250c391b2d16ebe53b3747c295ca8ba2fcb6b0cf064a4dc21c`  
		Last Modified: Fri, 10 Feb 2023 22:41:31 GMT  
		Size: 3.4 MB (3374446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69b7a2cbfc2f3b3305293d689573f3c9651d6053e5f780a9ba42a4c836d8d6c9`  
		Last Modified: Mon, 13 Mar 2023 23:21:18 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9662dafd479312640e4852a3e8b4caa9c758e1d55e2177a988e8defb54fb3c4`  
		Last Modified: Thu, 16 Mar 2023 01:02:25 GMT  
		Size: 12.4 MB (12375014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cc9d593845c782b74273932afc2437f197ed7d05bc6d861ed3ac5f7d84da491`  
		Last Modified: Thu, 16 Mar 2023 01:02:24 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bd6a5613be96b84704c17fa831782b1243af2c2ebfa7963d0a193bd667faa4f`  
		Last Modified: Thu, 16 Mar 2023 01:03:28 GMT  
		Size: 46.8 MB (46844100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93c00aabe78e65e78ce67a651eb145760972b04e87d27131da57cd1835d64ff7`  
		Last Modified: Thu, 16 Mar 2023 01:03:24 GMT  
		Size: 6.2 MB (6211627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ad0c19283e8c9459b02ef61e5312d9bc478f9a7e329d2b9f702a9024059cd43`  
		Last Modified: Thu, 16 Mar 2023 01:03:22 GMT  
		Size: 280.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6aed13e88a5723653f63f22eabf55e9a131e1d79b45dd8e9fc919999f2907190`  
		Last Modified: Thu, 16 Mar 2023 01:03:22 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0703611b1c12d2d8de8a553e1a1ad45e0113537d4c258e39be31a7cfb5e1a655`  
		Last Modified: Thu, 16 Mar 2023 01:03:22 GMT  
		Size: 6.4 KB (6441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:2.6-alpine` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:be8083f8011125627bddf8127a1afd1271c0e325d077390ed370c928fb38dc64
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.2 MB (66150734 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d53a04a41de54103270b266678b74a01a811e78295275a00e78daa48b5da5e4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:08 GMT
ADD file:9bd9ea42a9f3bdc769e80c6b8a4b117d65f73ae68e155a6172a1184e7ac8bcc1 in / 
# Fri, 10 Feb 2023 21:24:08 GMT
CMD ["/bin/sh"]
# Mon, 13 Mar 2023 23:47:18 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 15 Mar 2023 23:41:30 GMT
RUN apk add --no-cache       bash       ca-certificates       curl       gnupg       run-parts       su-exec       tzdata       yq &&     update-ca-certificates
# Wed, 15 Mar 2023 23:41:31 GMT
RUN addgroup -S -g 1000 influxdb &&     adduser -S -G influxdb -u 1000 -h /home/influxdb -s /bin/sh influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Wed, 15 Mar 2023 23:42:12 GMT
ENV INFLUXDB_VERSION=2.6.1
# Wed, 15 Mar 2023 23:42:15 GMT
RUN case "$(apk --print-arch)" in       x86_64)  arch=amd64 ;;       aarch64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&    curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     cp "influxdb2_linux_${arch}/influxd" /usr/local/bin/influxd &&     rm -rf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"            "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"            "influxdb2_linux_${arch}" &&     influxd version
# Wed, 15 Mar 2023 23:42:16 GMT
ENV INFLUX_CLI_VERSION=2.6.1
# Wed, 15 Mar 2023 23:42:18 GMT
RUN case "$(apk --print-arch)" in       x86_64)  arch=amd64 ;;       aarch64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     cp "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}/influx" /usr/local/bin/influx &&     rm -rf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     influx version
# Wed, 15 Mar 2023 23:42:18 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Wed, 15 Mar 2023 23:42:18 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Wed, 15 Mar 2023 23:42:18 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Wed, 15 Mar 2023 23:42:18 GMT
COPY file:708cccb15c29f10eb0c29e47f1c676d76b8ea9be434cce106ef95a7ba844bb2c in /entrypoint.sh 
# Wed, 15 Mar 2023 23:42:18 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 15 Mar 2023 23:42:19 GMT
CMD ["influxd"]
# Wed, 15 Mar 2023 23:42:19 GMT
EXPOSE 8086
# Wed, 15 Mar 2023 23:42:19 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Wed, 15 Mar 2023 23:42:19 GMT
ENV INFLUXD_INIT_PORT=9999
# Wed, 15 Mar 2023 23:42:19 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Wed, 15 Mar 2023 23:42:19 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:af6eaf76a39c2d3e7e0b8a0420486e3df33c4027d696c076a99a3d0ac09026af`  
		Last Modified: Fri, 10 Feb 2023 21:24:39 GMT  
		Size: 3.3 MB (3261959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dab1c38052d53938443512e37031810a03849aec98af5976a010b92ee4c13c1`  
		Last Modified: Mon, 13 Mar 2023 23:48:01 GMT  
		Size: 282.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd8e20b18f6688b37abc667eef7975eb77966987c3212d862a3b74b1e5a46151`  
		Last Modified: Wed, 15 Mar 2023 23:43:14 GMT  
		Size: 12.0 MB (12028387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:355a214bdc1929ff97f235f78bbe4313aa1f932134f19887c12d346d935da41e`  
		Last Modified: Wed, 15 Mar 2023 23:43:12 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31e07cdd4df7ad6d279c2b0ad02b70e9f235d81a8faa491877aa8341de8e586a`  
		Last Modified: Wed, 15 Mar 2023 23:44:08 GMT  
		Size: 45.1 MB (45145868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce244d050d45643e86cca057b3df2b013760003acb0209e1f4b6e4760a579fb1`  
		Last Modified: Wed, 15 Mar 2023 23:44:05 GMT  
		Size: 5.7 MB (5705990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10d50124879a181daaef286a413248c3ee6ffbb09f088509892c5e6072c04145`  
		Last Modified: Wed, 15 Mar 2023 23:44:04 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4634f3eddfa8d87f297a0680e8d814f4aaf0e938a34f4d1d3a96b0a8892a7b17`  
		Last Modified: Wed, 15 Mar 2023 23:44:04 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:533388fbfa94c36396e618ac9b82f1599926fa25005e1f18241603e60fb04056`  
		Last Modified: Wed, 15 Mar 2023 23:44:05 GMT  
		Size: 6.4 KB (6442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:2.6.1`

```console
$ docker pull influxdb@sha256:dfa86201228943d0ac8c3e675fc8e85843a872a9edeedb0b3fddf52e64414188
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:2.6.1` - linux; amd64

```console
$ docker pull influxdb@sha256:d9ea508f639968720934cc9dd727e83cd5515f87c7a35fec044728a455a9578b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **98.8 MB (98837218 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a023b77ee0d8d5dbfca34a91f77e165247c3017017b782924ce74aa7dcfde836`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 01 Mar 2023 04:09:58 GMT
ADD file:493a5b0c8d2d63a1343258b3f9aa5fcd59a93f44fe26ad9e56b094c3a08fd3be in / 
# Wed, 01 Mar 2023 04:09:59 GMT
CMD ["bash"]
# Thu, 16 Mar 2023 00:56:52 GMT
RUN export DEBIAN_FRONTEND=noninteractive &&     apt-get update -y &&     apt-get install -y --no-install-recommends       ca-certificates       curl       gnupg &&     apt-get clean &&     rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 00:56:53 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     curl -fLo /usr/local/bin/yq "https://github.com/mikefarah/yq/releases/download/v4.30.8/yq_linux_${arch}" &&     case ${arch} in       amd64) echo '6c911103e0dcc54e2ba07e767d2d62bcfc77452b39ebaee45b1c46f062f4fd26 /usr/local/bin/yq' ;;       arm64) echo '95092e8b5332890c46689679b5e4360d96873c025ad8bafd961688f28ea434c7 /usr/local/bin/yq' ;;     esac | sha256sum -c - &&     chmod +x /usr/local/bin/yq &&     yq --version
# Thu, 16 Mar 2023 00:56:53 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --create-home --home-dir=/home/influxdb --shell=/bin/bash influxdb
# Thu, 16 Mar 2023 00:56:53 GMT
ENV GOSU_VER=1.12
# Thu, 16 Mar 2023 00:56:56 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       B42F6819007F00F88E364FD4036A9C25BF357DD4 &&     curl -fLo /usr/local/bin/gosu     "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-${arch}"          -fLo /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-${arch}.asc" &&     gpg --batch --verify /usr/local/bin/gosu.asc                          /usr/local/bin/gosu &&     rm -rf /usr/local/bin/gosu.asc &&     chmod +x /usr/local/bin/gosu &&     gosu --version &&     gosu nobody true
# Thu, 16 Mar 2023 00:57:46 GMT
ENV INFLUXDB_VERSION=2.6.1
# Thu, 16 Mar 2023 00:57:50 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     cp "influxdb2_linux_${arch}/influxd" /usr/local/bin/influxd &&     rm -rf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"            "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"            "influxdb2_linux_${arch}" &&     influxd version
# Thu, 16 Mar 2023 00:57:50 GMT
ENV INFLUX_CLI_VERSION=2.6.1
# Thu, 16 Mar 2023 00:57:52 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     cp "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}/influx" /usr/local/bin/influx &&     rm -rf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     influx version
# Thu, 16 Mar 2023 00:57:53 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Thu, 16 Mar 2023 00:57:53 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Thu, 16 Mar 2023 00:57:53 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Thu, 16 Mar 2023 00:57:53 GMT
COPY file:595a669a2c2c2f47df93700fcd3e412750aae40abb979bb4af48a89af97a8b72 in /entrypoint.sh 
# Thu, 16 Mar 2023 00:57:53 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 16 Mar 2023 00:57:53 GMT
CMD ["influxd"]
# Thu, 16 Mar 2023 00:57:53 GMT
EXPOSE 8086
# Thu, 16 Mar 2023 00:57:53 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Thu, 16 Mar 2023 00:57:53 GMT
ENV INFLUXD_INIT_PORT=9999
# Thu, 16 Mar 2023 00:57:53 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Thu, 16 Mar 2023 00:57:53 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:3f9582a2cbe7197f39185419c0ced2c986389f8fc6aa805e1f5c090eea6511e0`  
		Last Modified: Wed, 01 Mar 2023 04:14:23 GMT  
		Size: 31.4 MB (31411403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08a794c78d7ad502e285244fde2dd7768065af2038670e7f34208e22d1c857e2`  
		Last Modified: Thu, 16 Mar 2023 01:02:10 GMT  
		Size: 6.3 MB (6327743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acd90bd5b5e60e8373c43b82a755b742e62d469c7df42aef9ab6ad0ac943ef6b`  
		Last Modified: Thu, 16 Mar 2023 01:02:09 GMT  
		Size: 7.0 MB (7049181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a549c3bac6c035d00d970ff0a7c39398de5b5355e5264970174a609dfcb350c1`  
		Last Modified: Thu, 16 Mar 2023 01:02:08 GMT  
		Size: 4.1 KB (4117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d52f68e8e59a067e13373eed04aa01fa28f3e99320d3ccfb46232c85efe7432`  
		Last Modified: Thu, 16 Mar 2023 01:02:08 GMT  
		Size: 982.0 KB (982043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48976d943c24ad838f918383f3fa1d1cbb1b40eb19d039b778c23ea46752a865`  
		Last Modified: Thu, 16 Mar 2023 01:03:12 GMT  
		Size: 46.8 MB (46844106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3539972aef6eac29878ccd083697a376eb1aec8d5e229b5c8a6dcab6036edea`  
		Last Modified: Thu, 16 Mar 2023 01:03:07 GMT  
		Size: 6.2 MB (6211626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bb00e5e812eae43c162c6884051314289a906fcf9e53e5c6e8578ad0f5c1c00`  
		Last Modified: Thu, 16 Mar 2023 01:03:06 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec172591e2a97b25dd5c54f835a03191efb469ea9b38708ac8c0d7c7dc16f764`  
		Last Modified: Thu, 16 Mar 2023 01:03:06 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca79f302ed0dd277dff382083d00f0d5d62349e4defa511a5a54753e2358b2f5`  
		Last Modified: Thu, 16 Mar 2023 01:03:06 GMT  
		Size: 6.5 KB (6462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:2.6.1` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:750f7ade153ce2c99e6a718d63a82e6ef50c9b80edf08de87406a128725d0ef0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.8 MB (94794365 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d965327ac4600487dce1bd0b2306373fc5b4ec9127b5274a7a4ca06c614dc065`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 01 Mar 2023 02:20:39 GMT
ADD file:9dc5c6fb6431df80107eddb76fb18256d6f4a06b4b22f9a7c4bcd58476068186 in / 
# Wed, 01 Mar 2023 02:20:39 GMT
CMD ["bash"]
# Wed, 15 Mar 2023 23:41:07 GMT
RUN export DEBIAN_FRONTEND=noninteractive &&     apt-get update -y &&     apt-get install -y --no-install-recommends       ca-certificates       curl       gnupg &&     apt-get clean &&     rm -rf /var/lib/apt/lists/*
# Wed, 15 Mar 2023 23:41:08 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     curl -fLo /usr/local/bin/yq "https://github.com/mikefarah/yq/releases/download/v4.30.8/yq_linux_${arch}" &&     case ${arch} in       amd64) echo '6c911103e0dcc54e2ba07e767d2d62bcfc77452b39ebaee45b1c46f062f4fd26 /usr/local/bin/yq' ;;       arm64) echo '95092e8b5332890c46689679b5e4360d96873c025ad8bafd961688f28ea434c7 /usr/local/bin/yq' ;;     esac | sha256sum -c - &&     chmod +x /usr/local/bin/yq &&     yq --version
# Wed, 15 Mar 2023 23:41:09 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --create-home --home-dir=/home/influxdb --shell=/bin/bash influxdb
# Wed, 15 Mar 2023 23:41:09 GMT
ENV GOSU_VER=1.12
# Wed, 15 Mar 2023 23:41:11 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       B42F6819007F00F88E364FD4036A9C25BF357DD4 &&     curl -fLo /usr/local/bin/gosu     "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-${arch}"          -fLo /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-${arch}.asc" &&     gpg --batch --verify /usr/local/bin/gosu.asc                          /usr/local/bin/gosu &&     rm -rf /usr/local/bin/gosu.asc &&     chmod +x /usr/local/bin/gosu &&     gosu --version &&     gosu nobody true
# Wed, 15 Mar 2023 23:42:03 GMT
ENV INFLUXDB_VERSION=2.6.1
# Wed, 15 Mar 2023 23:42:06 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     cp "influxdb2_linux_${arch}/influxd" /usr/local/bin/influxd &&     rm -rf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"            "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"            "influxdb2_linux_${arch}" &&     influxd version
# Wed, 15 Mar 2023 23:42:07 GMT
ENV INFLUX_CLI_VERSION=2.6.1
# Wed, 15 Mar 2023 23:42:09 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     cp "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}/influx" /usr/local/bin/influx &&     rm -rf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     influx version
# Wed, 15 Mar 2023 23:42:09 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Wed, 15 Mar 2023 23:42:10 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Wed, 15 Mar 2023 23:42:10 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Wed, 15 Mar 2023 23:42:10 GMT
COPY file:595a669a2c2c2f47df93700fcd3e412750aae40abb979bb4af48a89af97a8b72 in /entrypoint.sh 
# Wed, 15 Mar 2023 23:42:10 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 15 Mar 2023 23:42:10 GMT
CMD ["influxd"]
# Wed, 15 Mar 2023 23:42:10 GMT
EXPOSE 8086
# Wed, 15 Mar 2023 23:42:10 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Wed, 15 Mar 2023 23:42:10 GMT
ENV INFLUXD_INIT_PORT=9999
# Wed, 15 Mar 2023 23:42:10 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Wed, 15 Mar 2023 23:42:10 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:66dbba0fb1b568cc3ffd53409ba2f9f82995ab7f80e379338f3f36e4dcd223be`  
		Last Modified: Wed, 01 Mar 2023 02:24:17 GMT  
		Size: 30.1 MB (30062814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65fd6db03d5e7efd9c898c05fa431254e6753c9d39caf9a942d187e791ef698e`  
		Last Modified: Wed, 15 Mar 2023 23:42:58 GMT  
		Size: 6.3 MB (6308600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:623e77e647b06d59d840fce37c059b20aa366a51af80637fd63e1e5512a9e5e6`  
		Last Modified: Wed, 15 Mar 2023 23:42:57 GMT  
		Size: 6.6 MB (6643045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4316c8eeb27a0e8e1b5c0adabd0c1c7a915c9dfda919151dea2c1f0fbd9b5b8d`  
		Last Modified: Wed, 15 Mar 2023 23:42:57 GMT  
		Size: 4.1 KB (4124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ed509fbb0848d068923c7c2fb0326172783db14b7e706111aa8d36fef0724e1`  
		Last Modified: Wed, 15 Mar 2023 23:42:57 GMT  
		Size: 916.9 KB (916930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcd9f815af9fa7713836edcaf8c0edfede3b00c2f262af85dee43e3bf5706a89`  
		Last Modified: Wed, 15 Mar 2023 23:43:53 GMT  
		Size: 45.1 MB (45145851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15e98fd076597f7d2ddfa0871be33a56e936d19752c20858efc5f76b0fe57e03`  
		Last Modified: Wed, 15 Mar 2023 23:43:50 GMT  
		Size: 5.7 MB (5706001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4e1b9223729f0d3aebccfacb5a0b15c96af102a78398ac8b0df5cfa5329e7ed`  
		Last Modified: Wed, 15 Mar 2023 23:43:49 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc31e1ada9713c6aa0ae771c2ff4a99aeaa09bcd46114941d005d37a165d5c8d`  
		Last Modified: Wed, 15 Mar 2023 23:43:49 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74f654e5c408f27396570fc3ebb1bfee8bd77d4e2f82a808aa4ce8cd861ff0af`  
		Last Modified: Wed, 15 Mar 2023 23:43:49 GMT  
		Size: 6.5 KB (6463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:2.6.1-alpine`

```console
$ docker pull influxdb@sha256:0db3d6571a3b139112c8b414a87d78993dd4915180020363da791fedc392b849
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:2.6.1-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:8bd70537963442987876957f5cc9428d3eed5213a8c043745dc638960d64d21c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.8 MB (68813716 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:304c50024095f76a248b28dfde97abb90eb69dada8f80a11c5d463be8e61ef69`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:42 GMT
ADD file:40887ab7c06977737e63c215c9bd297c0c74de8d12d16ebdf1c3d40ac392f62d in / 
# Sat, 11 Feb 2023 04:46:42 GMT
CMD ["/bin/sh"]
# Mon, 13 Mar 2023 23:20:24 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 16 Mar 2023 00:57:14 GMT
RUN apk add --no-cache       bash       ca-certificates       curl       gnupg       run-parts       su-exec       tzdata       yq &&     update-ca-certificates
# Thu, 16 Mar 2023 00:57:14 GMT
RUN addgroup -S -g 1000 influxdb &&     adduser -S -G influxdb -u 1000 -h /home/influxdb -s /bin/sh influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Thu, 16 Mar 2023 00:57:57 GMT
ENV INFLUXDB_VERSION=2.6.1
# Thu, 16 Mar 2023 00:58:00 GMT
RUN case "$(apk --print-arch)" in       x86_64)  arch=amd64 ;;       aarch64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&    curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     cp "influxdb2_linux_${arch}/influxd" /usr/local/bin/influxd &&     rm -rf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"            "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"            "influxdb2_linux_${arch}" &&     influxd version
# Thu, 16 Mar 2023 00:58:01 GMT
ENV INFLUX_CLI_VERSION=2.6.1
# Thu, 16 Mar 2023 00:58:02 GMT
RUN case "$(apk --print-arch)" in       x86_64)  arch=amd64 ;;       aarch64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     cp "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}/influx" /usr/local/bin/influx &&     rm -rf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     influx version
# Thu, 16 Mar 2023 00:58:03 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Thu, 16 Mar 2023 00:58:03 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Thu, 16 Mar 2023 00:58:03 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Thu, 16 Mar 2023 00:58:03 GMT
COPY file:708cccb15c29f10eb0c29e47f1c676d76b8ea9be434cce106ef95a7ba844bb2c in /entrypoint.sh 
# Thu, 16 Mar 2023 00:58:03 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 16 Mar 2023 00:58:03 GMT
CMD ["influxd"]
# Thu, 16 Mar 2023 00:58:03 GMT
EXPOSE 8086
# Thu, 16 Mar 2023 00:58:03 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Thu, 16 Mar 2023 00:58:03 GMT
ENV INFLUXD_INIT_PORT=9999
# Thu, 16 Mar 2023 00:58:04 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Thu, 16 Mar 2023 00:58:04 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:63b65145d645c1250c391b2d16ebe53b3747c295ca8ba2fcb6b0cf064a4dc21c`  
		Last Modified: Fri, 10 Feb 2023 22:41:31 GMT  
		Size: 3.4 MB (3374446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69b7a2cbfc2f3b3305293d689573f3c9651d6053e5f780a9ba42a4c836d8d6c9`  
		Last Modified: Mon, 13 Mar 2023 23:21:18 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9662dafd479312640e4852a3e8b4caa9c758e1d55e2177a988e8defb54fb3c4`  
		Last Modified: Thu, 16 Mar 2023 01:02:25 GMT  
		Size: 12.4 MB (12375014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cc9d593845c782b74273932afc2437f197ed7d05bc6d861ed3ac5f7d84da491`  
		Last Modified: Thu, 16 Mar 2023 01:02:24 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bd6a5613be96b84704c17fa831782b1243af2c2ebfa7963d0a193bd667faa4f`  
		Last Modified: Thu, 16 Mar 2023 01:03:28 GMT  
		Size: 46.8 MB (46844100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93c00aabe78e65e78ce67a651eb145760972b04e87d27131da57cd1835d64ff7`  
		Last Modified: Thu, 16 Mar 2023 01:03:24 GMT  
		Size: 6.2 MB (6211627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ad0c19283e8c9459b02ef61e5312d9bc478f9a7e329d2b9f702a9024059cd43`  
		Last Modified: Thu, 16 Mar 2023 01:03:22 GMT  
		Size: 280.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6aed13e88a5723653f63f22eabf55e9a131e1d79b45dd8e9fc919999f2907190`  
		Last Modified: Thu, 16 Mar 2023 01:03:22 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0703611b1c12d2d8de8a553e1a1ad45e0113537d4c258e39be31a7cfb5e1a655`  
		Last Modified: Thu, 16 Mar 2023 01:03:22 GMT  
		Size: 6.4 KB (6441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:2.6.1-alpine` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:be8083f8011125627bddf8127a1afd1271c0e325d077390ed370c928fb38dc64
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.2 MB (66150734 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d53a04a41de54103270b266678b74a01a811e78295275a00e78daa48b5da5e4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:08 GMT
ADD file:9bd9ea42a9f3bdc769e80c6b8a4b117d65f73ae68e155a6172a1184e7ac8bcc1 in / 
# Fri, 10 Feb 2023 21:24:08 GMT
CMD ["/bin/sh"]
# Mon, 13 Mar 2023 23:47:18 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 15 Mar 2023 23:41:30 GMT
RUN apk add --no-cache       bash       ca-certificates       curl       gnupg       run-parts       su-exec       tzdata       yq &&     update-ca-certificates
# Wed, 15 Mar 2023 23:41:31 GMT
RUN addgroup -S -g 1000 influxdb &&     adduser -S -G influxdb -u 1000 -h /home/influxdb -s /bin/sh influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Wed, 15 Mar 2023 23:42:12 GMT
ENV INFLUXDB_VERSION=2.6.1
# Wed, 15 Mar 2023 23:42:15 GMT
RUN case "$(apk --print-arch)" in       x86_64)  arch=amd64 ;;       aarch64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&    curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     cp "influxdb2_linux_${arch}/influxd" /usr/local/bin/influxd &&     rm -rf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"            "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"            "influxdb2_linux_${arch}" &&     influxd version
# Wed, 15 Mar 2023 23:42:16 GMT
ENV INFLUX_CLI_VERSION=2.6.1
# Wed, 15 Mar 2023 23:42:18 GMT
RUN case "$(apk --print-arch)" in       x86_64)  arch=amd64 ;;       aarch64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     cp "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}/influx" /usr/local/bin/influx &&     rm -rf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     influx version
# Wed, 15 Mar 2023 23:42:18 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Wed, 15 Mar 2023 23:42:18 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Wed, 15 Mar 2023 23:42:18 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Wed, 15 Mar 2023 23:42:18 GMT
COPY file:708cccb15c29f10eb0c29e47f1c676d76b8ea9be434cce106ef95a7ba844bb2c in /entrypoint.sh 
# Wed, 15 Mar 2023 23:42:18 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 15 Mar 2023 23:42:19 GMT
CMD ["influxd"]
# Wed, 15 Mar 2023 23:42:19 GMT
EXPOSE 8086
# Wed, 15 Mar 2023 23:42:19 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Wed, 15 Mar 2023 23:42:19 GMT
ENV INFLUXD_INIT_PORT=9999
# Wed, 15 Mar 2023 23:42:19 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Wed, 15 Mar 2023 23:42:19 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:af6eaf76a39c2d3e7e0b8a0420486e3df33c4027d696c076a99a3d0ac09026af`  
		Last Modified: Fri, 10 Feb 2023 21:24:39 GMT  
		Size: 3.3 MB (3261959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dab1c38052d53938443512e37031810a03849aec98af5976a010b92ee4c13c1`  
		Last Modified: Mon, 13 Mar 2023 23:48:01 GMT  
		Size: 282.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd8e20b18f6688b37abc667eef7975eb77966987c3212d862a3b74b1e5a46151`  
		Last Modified: Wed, 15 Mar 2023 23:43:14 GMT  
		Size: 12.0 MB (12028387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:355a214bdc1929ff97f235f78bbe4313aa1f932134f19887c12d346d935da41e`  
		Last Modified: Wed, 15 Mar 2023 23:43:12 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31e07cdd4df7ad6d279c2b0ad02b70e9f235d81a8faa491877aa8341de8e586a`  
		Last Modified: Wed, 15 Mar 2023 23:44:08 GMT  
		Size: 45.1 MB (45145868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce244d050d45643e86cca057b3df2b013760003acb0209e1f4b6e4760a579fb1`  
		Last Modified: Wed, 15 Mar 2023 23:44:05 GMT  
		Size: 5.7 MB (5705990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10d50124879a181daaef286a413248c3ee6ffbb09f088509892c5e6072c04145`  
		Last Modified: Wed, 15 Mar 2023 23:44:04 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4634f3eddfa8d87f297a0680e8d814f4aaf0e938a34f4d1d3a96b0a8892a7b17`  
		Last Modified: Wed, 15 Mar 2023 23:44:04 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:533388fbfa94c36396e618ac9b82f1599926fa25005e1f18241603e60fb04056`  
		Last Modified: Wed, 15 Mar 2023 23:44:05 GMT  
		Size: 6.4 KB (6442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:alpine`

```console
$ docker pull influxdb@sha256:0db3d6571a3b139112c8b414a87d78993dd4915180020363da791fedc392b849
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:8bd70537963442987876957f5cc9428d3eed5213a8c043745dc638960d64d21c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.8 MB (68813716 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:304c50024095f76a248b28dfde97abb90eb69dada8f80a11c5d463be8e61ef69`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:42 GMT
ADD file:40887ab7c06977737e63c215c9bd297c0c74de8d12d16ebdf1c3d40ac392f62d in / 
# Sat, 11 Feb 2023 04:46:42 GMT
CMD ["/bin/sh"]
# Mon, 13 Mar 2023 23:20:24 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 16 Mar 2023 00:57:14 GMT
RUN apk add --no-cache       bash       ca-certificates       curl       gnupg       run-parts       su-exec       tzdata       yq &&     update-ca-certificates
# Thu, 16 Mar 2023 00:57:14 GMT
RUN addgroup -S -g 1000 influxdb &&     adduser -S -G influxdb -u 1000 -h /home/influxdb -s /bin/sh influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Thu, 16 Mar 2023 00:57:57 GMT
ENV INFLUXDB_VERSION=2.6.1
# Thu, 16 Mar 2023 00:58:00 GMT
RUN case "$(apk --print-arch)" in       x86_64)  arch=amd64 ;;       aarch64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&    curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     cp "influxdb2_linux_${arch}/influxd" /usr/local/bin/influxd &&     rm -rf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"            "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"            "influxdb2_linux_${arch}" &&     influxd version
# Thu, 16 Mar 2023 00:58:01 GMT
ENV INFLUX_CLI_VERSION=2.6.1
# Thu, 16 Mar 2023 00:58:02 GMT
RUN case "$(apk --print-arch)" in       x86_64)  arch=amd64 ;;       aarch64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     cp "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}/influx" /usr/local/bin/influx &&     rm -rf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     influx version
# Thu, 16 Mar 2023 00:58:03 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Thu, 16 Mar 2023 00:58:03 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Thu, 16 Mar 2023 00:58:03 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Thu, 16 Mar 2023 00:58:03 GMT
COPY file:708cccb15c29f10eb0c29e47f1c676d76b8ea9be434cce106ef95a7ba844bb2c in /entrypoint.sh 
# Thu, 16 Mar 2023 00:58:03 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 16 Mar 2023 00:58:03 GMT
CMD ["influxd"]
# Thu, 16 Mar 2023 00:58:03 GMT
EXPOSE 8086
# Thu, 16 Mar 2023 00:58:03 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Thu, 16 Mar 2023 00:58:03 GMT
ENV INFLUXD_INIT_PORT=9999
# Thu, 16 Mar 2023 00:58:04 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Thu, 16 Mar 2023 00:58:04 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:63b65145d645c1250c391b2d16ebe53b3747c295ca8ba2fcb6b0cf064a4dc21c`  
		Last Modified: Fri, 10 Feb 2023 22:41:31 GMT  
		Size: 3.4 MB (3374446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69b7a2cbfc2f3b3305293d689573f3c9651d6053e5f780a9ba42a4c836d8d6c9`  
		Last Modified: Mon, 13 Mar 2023 23:21:18 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9662dafd479312640e4852a3e8b4caa9c758e1d55e2177a988e8defb54fb3c4`  
		Last Modified: Thu, 16 Mar 2023 01:02:25 GMT  
		Size: 12.4 MB (12375014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cc9d593845c782b74273932afc2437f197ed7d05bc6d861ed3ac5f7d84da491`  
		Last Modified: Thu, 16 Mar 2023 01:02:24 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bd6a5613be96b84704c17fa831782b1243af2c2ebfa7963d0a193bd667faa4f`  
		Last Modified: Thu, 16 Mar 2023 01:03:28 GMT  
		Size: 46.8 MB (46844100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93c00aabe78e65e78ce67a651eb145760972b04e87d27131da57cd1835d64ff7`  
		Last Modified: Thu, 16 Mar 2023 01:03:24 GMT  
		Size: 6.2 MB (6211627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ad0c19283e8c9459b02ef61e5312d9bc478f9a7e329d2b9f702a9024059cd43`  
		Last Modified: Thu, 16 Mar 2023 01:03:22 GMT  
		Size: 280.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6aed13e88a5723653f63f22eabf55e9a131e1d79b45dd8e9fc919999f2907190`  
		Last Modified: Thu, 16 Mar 2023 01:03:22 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0703611b1c12d2d8de8a553e1a1ad45e0113537d4c258e39be31a7cfb5e1a655`  
		Last Modified: Thu, 16 Mar 2023 01:03:22 GMT  
		Size: 6.4 KB (6441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:alpine` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:be8083f8011125627bddf8127a1afd1271c0e325d077390ed370c928fb38dc64
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.2 MB (66150734 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d53a04a41de54103270b266678b74a01a811e78295275a00e78daa48b5da5e4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:08 GMT
ADD file:9bd9ea42a9f3bdc769e80c6b8a4b117d65f73ae68e155a6172a1184e7ac8bcc1 in / 
# Fri, 10 Feb 2023 21:24:08 GMT
CMD ["/bin/sh"]
# Mon, 13 Mar 2023 23:47:18 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 15 Mar 2023 23:41:30 GMT
RUN apk add --no-cache       bash       ca-certificates       curl       gnupg       run-parts       su-exec       tzdata       yq &&     update-ca-certificates
# Wed, 15 Mar 2023 23:41:31 GMT
RUN addgroup -S -g 1000 influxdb &&     adduser -S -G influxdb -u 1000 -h /home/influxdb -s /bin/sh influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Wed, 15 Mar 2023 23:42:12 GMT
ENV INFLUXDB_VERSION=2.6.1
# Wed, 15 Mar 2023 23:42:15 GMT
RUN case "$(apk --print-arch)" in       x86_64)  arch=amd64 ;;       aarch64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&    curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     cp "influxdb2_linux_${arch}/influxd" /usr/local/bin/influxd &&     rm -rf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"            "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"            "influxdb2_linux_${arch}" &&     influxd version
# Wed, 15 Mar 2023 23:42:16 GMT
ENV INFLUX_CLI_VERSION=2.6.1
# Wed, 15 Mar 2023 23:42:18 GMT
RUN case "$(apk --print-arch)" in       x86_64)  arch=amd64 ;;       aarch64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     cp "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}/influx" /usr/local/bin/influx &&     rm -rf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     influx version
# Wed, 15 Mar 2023 23:42:18 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Wed, 15 Mar 2023 23:42:18 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Wed, 15 Mar 2023 23:42:18 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Wed, 15 Mar 2023 23:42:18 GMT
COPY file:708cccb15c29f10eb0c29e47f1c676d76b8ea9be434cce106ef95a7ba844bb2c in /entrypoint.sh 
# Wed, 15 Mar 2023 23:42:18 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 15 Mar 2023 23:42:19 GMT
CMD ["influxd"]
# Wed, 15 Mar 2023 23:42:19 GMT
EXPOSE 8086
# Wed, 15 Mar 2023 23:42:19 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Wed, 15 Mar 2023 23:42:19 GMT
ENV INFLUXD_INIT_PORT=9999
# Wed, 15 Mar 2023 23:42:19 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Wed, 15 Mar 2023 23:42:19 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:af6eaf76a39c2d3e7e0b8a0420486e3df33c4027d696c076a99a3d0ac09026af`  
		Last Modified: Fri, 10 Feb 2023 21:24:39 GMT  
		Size: 3.3 MB (3261959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dab1c38052d53938443512e37031810a03849aec98af5976a010b92ee4c13c1`  
		Last Modified: Mon, 13 Mar 2023 23:48:01 GMT  
		Size: 282.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd8e20b18f6688b37abc667eef7975eb77966987c3212d862a3b74b1e5a46151`  
		Last Modified: Wed, 15 Mar 2023 23:43:14 GMT  
		Size: 12.0 MB (12028387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:355a214bdc1929ff97f235f78bbe4313aa1f932134f19887c12d346d935da41e`  
		Last Modified: Wed, 15 Mar 2023 23:43:12 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31e07cdd4df7ad6d279c2b0ad02b70e9f235d81a8faa491877aa8341de8e586a`  
		Last Modified: Wed, 15 Mar 2023 23:44:08 GMT  
		Size: 45.1 MB (45145868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce244d050d45643e86cca057b3df2b013760003acb0209e1f4b6e4760a579fb1`  
		Last Modified: Wed, 15 Mar 2023 23:44:05 GMT  
		Size: 5.7 MB (5705990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10d50124879a181daaef286a413248c3ee6ffbb09f088509892c5e6072c04145`  
		Last Modified: Wed, 15 Mar 2023 23:44:04 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4634f3eddfa8d87f297a0680e8d814f4aaf0e938a34f4d1d3a96b0a8892a7b17`  
		Last Modified: Wed, 15 Mar 2023 23:44:04 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:533388fbfa94c36396e618ac9b82f1599926fa25005e1f18241603e60fb04056`  
		Last Modified: Wed, 15 Mar 2023 23:44:05 GMT  
		Size: 6.4 KB (6442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:data`

```console
$ docker pull influxdb@sha256:d70a44306e5c0a3774d8cfa978fdb119a9864f1844e3e85d374b4c93584fed64
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:data` - linux; amd64

```console
$ docker pull influxdb@sha256:894aa6fecfd3f4a9f87f8d72086e1f8b409a85112afab30ca34b3952602080fb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.8 MB (127797922 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d8e09311c7aa581a42b2643e4b1bb5f9f80decf1c37482ee4e9e087fd9a10dd`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 01 Mar 2023 04:09:45 GMT
ADD file:513c5d5e501279c21a05c1d8b66e5f0b02ee4b27f0b928706d92fd9ce11c1be6 in / 
# Wed, 01 Mar 2023 04:09:46 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 04:42:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 04:42:43 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Mar 2023 00:54:43 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 16 Mar 2023 00:55:02 GMT
ENV INFLUXDB_VERSION=1.8.10-c1.8.10
# Thu, 16 Mar 2023 00:55:08 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-data_${INFLUXDB_VERSION}_amd64.deb*
# Thu, 16 Mar 2023 00:55:08 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Thu, 16 Mar 2023 00:55:08 GMT
EXPOSE 8086
# Thu, 16 Mar 2023 00:55:08 GMT
VOLUME [/var/lib/influxdb]
# Thu, 16 Mar 2023 00:55:09 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Thu, 16 Mar 2023 00:55:09 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Thu, 16 Mar 2023 00:55:09 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 16 Mar 2023 00:55:09 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:32fb02163b6bb519a30f909008e852354dae10bdfd6b34190dbdfe8f15403ea0`  
		Last Modified: Wed, 01 Mar 2023 04:13:58 GMT  
		Size: 55.0 MB (55045922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:167c7feebee855d117e192389484ea8367be1ba84e7ee35f4e5e5663195facbf`  
		Last Modified: Wed, 01 Mar 2023 04:50:15 GMT  
		Size: 5.2 MB (5166586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6dfff1f6f3ddd2194ea0775f199572e8b2d75c38713eef0444d6b1fd0ac7604`  
		Last Modified: Wed, 01 Mar 2023 04:50:15 GMT  
		Size: 10.9 MB (10876729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a90f0187c37c44f2ad04f9d930d40ee0b886fc8d783b914b10a620683739873`  
		Last Modified: Thu, 16 Mar 2023 00:58:47 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4924ec9dc809c1730e7c63922a8e5165926ba2c739cef19170759a0d114745cc`  
		Last Modified: Thu, 16 Mar 2023 00:59:25 GMT  
		Size: 56.7 MB (56705114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8db089179f3c59891770a09bb5a9039cdedf7ffa9452abb94320eca049ff512`  
		Last Modified: Thu, 16 Mar 2023 00:59:18 GMT  
		Size: 242.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1dc009f87cbeaf772c33446fed5360fc8f2edc94895aa45fb77b68751462fd1`  
		Last Modified: Thu, 16 Mar 2023 00:59:18 GMT  
		Size: 252.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8e9a069b786cd091e09d7a579e3d9a77cccb94fa2c895d3724ec882a2c209ef`  
		Last Modified: Thu, 16 Mar 2023 00:59:18 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:data-alpine`

```console
$ docker pull influxdb@sha256:261d1655b8cc2dc5404af459329701d0b8245717caadd711036a2e2a36888e36
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:data-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:4062b21acf2700f04d0da13c37ecf473b0a75ac6de7b03c3f7fd4c3df2ce7524
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.4 MB (61352861 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f18f1dce311ade7a5bc787e5cc41b48cb635fb2e249b34189c63fbc882712b7`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:42 GMT
ADD file:40887ab7c06977737e63c215c9bd297c0c74de8d12d16ebdf1c3d40ac392f62d in / 
# Sat, 11 Feb 2023 04:46:42 GMT
CMD ["/bin/sh"]
# Mon, 13 Mar 2023 23:20:24 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 16 Mar 2023 00:54:52 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Thu, 16 Mar 2023 00:55:13 GMT
ENV INFLUXDB_VERSION=1.8.10-c1.8.10
# Thu, 16 Mar 2023 00:55:21 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Thu, 16 Mar 2023 00:55:21 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Thu, 16 Mar 2023 00:55:21 GMT
EXPOSE 8086
# Thu, 16 Mar 2023 00:55:22 GMT
VOLUME [/var/lib/influxdb]
# Thu, 16 Mar 2023 00:55:22 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Thu, 16 Mar 2023 00:55:22 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Thu, 16 Mar 2023 00:55:22 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 16 Mar 2023 00:55:22 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:63b65145d645c1250c391b2d16ebe53b3747c295ca8ba2fcb6b0cf064a4dc21c`  
		Last Modified: Fri, 10 Feb 2023 22:41:31 GMT  
		Size: 3.4 MB (3374446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69b7a2cbfc2f3b3305293d689573f3c9651d6053e5f780a9ba42a4c836d8d6c9`  
		Last Modified: Mon, 13 Mar 2023 23:21:18 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5b0a9605b8bc1c4f3b877c51f73e8d0cc4b02403f8f9d18c276f012b604c038`  
		Last Modified: Thu, 16 Mar 2023 00:59:03 GMT  
		Size: 1.5 MB (1472712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61bad459754475dfd8621019d72d1bd32ca2b9be86fb936ab64308888ee0073a`  
		Last Modified: Thu, 16 Mar 2023 00:59:43 GMT  
		Size: 56.5 MB (56503629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0fdd4464dd3872545334e618c0323eef93811cc622aa2409dc50a984d042034`  
		Last Modified: Thu, 16 Mar 2023 00:59:36 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aeb71d6736a13e612d2dc8a667133647ee9099895936ffa258569114cc772086`  
		Last Modified: Thu, 16 Mar 2023 00:59:36 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a34548e01d2f855e58fb7674a9102ca3878dda447d78e6060033d7827d27589f`  
		Last Modified: Thu, 16 Mar 2023 00:59:36 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:latest`

```console
$ docker pull influxdb@sha256:dfa86201228943d0ac8c3e675fc8e85843a872a9edeedb0b3fddf52e64414188
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:latest` - linux; amd64

```console
$ docker pull influxdb@sha256:d9ea508f639968720934cc9dd727e83cd5515f87c7a35fec044728a455a9578b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **98.8 MB (98837218 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a023b77ee0d8d5dbfca34a91f77e165247c3017017b782924ce74aa7dcfde836`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 01 Mar 2023 04:09:58 GMT
ADD file:493a5b0c8d2d63a1343258b3f9aa5fcd59a93f44fe26ad9e56b094c3a08fd3be in / 
# Wed, 01 Mar 2023 04:09:59 GMT
CMD ["bash"]
# Thu, 16 Mar 2023 00:56:52 GMT
RUN export DEBIAN_FRONTEND=noninteractive &&     apt-get update -y &&     apt-get install -y --no-install-recommends       ca-certificates       curl       gnupg &&     apt-get clean &&     rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 00:56:53 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     curl -fLo /usr/local/bin/yq "https://github.com/mikefarah/yq/releases/download/v4.30.8/yq_linux_${arch}" &&     case ${arch} in       amd64) echo '6c911103e0dcc54e2ba07e767d2d62bcfc77452b39ebaee45b1c46f062f4fd26 /usr/local/bin/yq' ;;       arm64) echo '95092e8b5332890c46689679b5e4360d96873c025ad8bafd961688f28ea434c7 /usr/local/bin/yq' ;;     esac | sha256sum -c - &&     chmod +x /usr/local/bin/yq &&     yq --version
# Thu, 16 Mar 2023 00:56:53 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --create-home --home-dir=/home/influxdb --shell=/bin/bash influxdb
# Thu, 16 Mar 2023 00:56:53 GMT
ENV GOSU_VER=1.12
# Thu, 16 Mar 2023 00:56:56 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       B42F6819007F00F88E364FD4036A9C25BF357DD4 &&     curl -fLo /usr/local/bin/gosu     "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-${arch}"          -fLo /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-${arch}.asc" &&     gpg --batch --verify /usr/local/bin/gosu.asc                          /usr/local/bin/gosu &&     rm -rf /usr/local/bin/gosu.asc &&     chmod +x /usr/local/bin/gosu &&     gosu --version &&     gosu nobody true
# Thu, 16 Mar 2023 00:57:46 GMT
ENV INFLUXDB_VERSION=2.6.1
# Thu, 16 Mar 2023 00:57:50 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     cp "influxdb2_linux_${arch}/influxd" /usr/local/bin/influxd &&     rm -rf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"            "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"            "influxdb2_linux_${arch}" &&     influxd version
# Thu, 16 Mar 2023 00:57:50 GMT
ENV INFLUX_CLI_VERSION=2.6.1
# Thu, 16 Mar 2023 00:57:52 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     cp "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}/influx" /usr/local/bin/influx &&     rm -rf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     influx version
# Thu, 16 Mar 2023 00:57:53 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Thu, 16 Mar 2023 00:57:53 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Thu, 16 Mar 2023 00:57:53 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Thu, 16 Mar 2023 00:57:53 GMT
COPY file:595a669a2c2c2f47df93700fcd3e412750aae40abb979bb4af48a89af97a8b72 in /entrypoint.sh 
# Thu, 16 Mar 2023 00:57:53 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 16 Mar 2023 00:57:53 GMT
CMD ["influxd"]
# Thu, 16 Mar 2023 00:57:53 GMT
EXPOSE 8086
# Thu, 16 Mar 2023 00:57:53 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Thu, 16 Mar 2023 00:57:53 GMT
ENV INFLUXD_INIT_PORT=9999
# Thu, 16 Mar 2023 00:57:53 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Thu, 16 Mar 2023 00:57:53 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:3f9582a2cbe7197f39185419c0ced2c986389f8fc6aa805e1f5c090eea6511e0`  
		Last Modified: Wed, 01 Mar 2023 04:14:23 GMT  
		Size: 31.4 MB (31411403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08a794c78d7ad502e285244fde2dd7768065af2038670e7f34208e22d1c857e2`  
		Last Modified: Thu, 16 Mar 2023 01:02:10 GMT  
		Size: 6.3 MB (6327743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acd90bd5b5e60e8373c43b82a755b742e62d469c7df42aef9ab6ad0ac943ef6b`  
		Last Modified: Thu, 16 Mar 2023 01:02:09 GMT  
		Size: 7.0 MB (7049181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a549c3bac6c035d00d970ff0a7c39398de5b5355e5264970174a609dfcb350c1`  
		Last Modified: Thu, 16 Mar 2023 01:02:08 GMT  
		Size: 4.1 KB (4117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d52f68e8e59a067e13373eed04aa01fa28f3e99320d3ccfb46232c85efe7432`  
		Last Modified: Thu, 16 Mar 2023 01:02:08 GMT  
		Size: 982.0 KB (982043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48976d943c24ad838f918383f3fa1d1cbb1b40eb19d039b778c23ea46752a865`  
		Last Modified: Thu, 16 Mar 2023 01:03:12 GMT  
		Size: 46.8 MB (46844106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3539972aef6eac29878ccd083697a376eb1aec8d5e229b5c8a6dcab6036edea`  
		Last Modified: Thu, 16 Mar 2023 01:03:07 GMT  
		Size: 6.2 MB (6211626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bb00e5e812eae43c162c6884051314289a906fcf9e53e5c6e8578ad0f5c1c00`  
		Last Modified: Thu, 16 Mar 2023 01:03:06 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec172591e2a97b25dd5c54f835a03191efb469ea9b38708ac8c0d7c7dc16f764`  
		Last Modified: Thu, 16 Mar 2023 01:03:06 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca79f302ed0dd277dff382083d00f0d5d62349e4defa511a5a54753e2358b2f5`  
		Last Modified: Thu, 16 Mar 2023 01:03:06 GMT  
		Size: 6.5 KB (6462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:latest` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:750f7ade153ce2c99e6a718d63a82e6ef50c9b80edf08de87406a128725d0ef0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.8 MB (94794365 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d965327ac4600487dce1bd0b2306373fc5b4ec9127b5274a7a4ca06c614dc065`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 01 Mar 2023 02:20:39 GMT
ADD file:9dc5c6fb6431df80107eddb76fb18256d6f4a06b4b22f9a7c4bcd58476068186 in / 
# Wed, 01 Mar 2023 02:20:39 GMT
CMD ["bash"]
# Wed, 15 Mar 2023 23:41:07 GMT
RUN export DEBIAN_FRONTEND=noninteractive &&     apt-get update -y &&     apt-get install -y --no-install-recommends       ca-certificates       curl       gnupg &&     apt-get clean &&     rm -rf /var/lib/apt/lists/*
# Wed, 15 Mar 2023 23:41:08 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     curl -fLo /usr/local/bin/yq "https://github.com/mikefarah/yq/releases/download/v4.30.8/yq_linux_${arch}" &&     case ${arch} in       amd64) echo '6c911103e0dcc54e2ba07e767d2d62bcfc77452b39ebaee45b1c46f062f4fd26 /usr/local/bin/yq' ;;       arm64) echo '95092e8b5332890c46689679b5e4360d96873c025ad8bafd961688f28ea434c7 /usr/local/bin/yq' ;;     esac | sha256sum -c - &&     chmod +x /usr/local/bin/yq &&     yq --version
# Wed, 15 Mar 2023 23:41:09 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --create-home --home-dir=/home/influxdb --shell=/bin/bash influxdb
# Wed, 15 Mar 2023 23:41:09 GMT
ENV GOSU_VER=1.12
# Wed, 15 Mar 2023 23:41:11 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       B42F6819007F00F88E364FD4036A9C25BF357DD4 &&     curl -fLo /usr/local/bin/gosu     "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-${arch}"          -fLo /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-${arch}.asc" &&     gpg --batch --verify /usr/local/bin/gosu.asc                          /usr/local/bin/gosu &&     rm -rf /usr/local/bin/gosu.asc &&     chmod +x /usr/local/bin/gosu &&     gosu --version &&     gosu nobody true
# Wed, 15 Mar 2023 23:42:03 GMT
ENV INFLUXDB_VERSION=2.6.1
# Wed, 15 Mar 2023 23:42:06 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     cp "influxdb2_linux_${arch}/influxd" /usr/local/bin/influxd &&     rm -rf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"            "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"            "influxdb2_linux_${arch}" &&     influxd version
# Wed, 15 Mar 2023 23:42:07 GMT
ENV INFLUX_CLI_VERSION=2.6.1
# Wed, 15 Mar 2023 23:42:09 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     cp "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}/influx" /usr/local/bin/influx &&     rm -rf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     influx version
# Wed, 15 Mar 2023 23:42:09 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Wed, 15 Mar 2023 23:42:10 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Wed, 15 Mar 2023 23:42:10 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Wed, 15 Mar 2023 23:42:10 GMT
COPY file:595a669a2c2c2f47df93700fcd3e412750aae40abb979bb4af48a89af97a8b72 in /entrypoint.sh 
# Wed, 15 Mar 2023 23:42:10 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 15 Mar 2023 23:42:10 GMT
CMD ["influxd"]
# Wed, 15 Mar 2023 23:42:10 GMT
EXPOSE 8086
# Wed, 15 Mar 2023 23:42:10 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Wed, 15 Mar 2023 23:42:10 GMT
ENV INFLUXD_INIT_PORT=9999
# Wed, 15 Mar 2023 23:42:10 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Wed, 15 Mar 2023 23:42:10 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:66dbba0fb1b568cc3ffd53409ba2f9f82995ab7f80e379338f3f36e4dcd223be`  
		Last Modified: Wed, 01 Mar 2023 02:24:17 GMT  
		Size: 30.1 MB (30062814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65fd6db03d5e7efd9c898c05fa431254e6753c9d39caf9a942d187e791ef698e`  
		Last Modified: Wed, 15 Mar 2023 23:42:58 GMT  
		Size: 6.3 MB (6308600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:623e77e647b06d59d840fce37c059b20aa366a51af80637fd63e1e5512a9e5e6`  
		Last Modified: Wed, 15 Mar 2023 23:42:57 GMT  
		Size: 6.6 MB (6643045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4316c8eeb27a0e8e1b5c0adabd0c1c7a915c9dfda919151dea2c1f0fbd9b5b8d`  
		Last Modified: Wed, 15 Mar 2023 23:42:57 GMT  
		Size: 4.1 KB (4124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ed509fbb0848d068923c7c2fb0326172783db14b7e706111aa8d36fef0724e1`  
		Last Modified: Wed, 15 Mar 2023 23:42:57 GMT  
		Size: 916.9 KB (916930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcd9f815af9fa7713836edcaf8c0edfede3b00c2f262af85dee43e3bf5706a89`  
		Last Modified: Wed, 15 Mar 2023 23:43:53 GMT  
		Size: 45.1 MB (45145851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15e98fd076597f7d2ddfa0871be33a56e936d19752c20858efc5f76b0fe57e03`  
		Last Modified: Wed, 15 Mar 2023 23:43:50 GMT  
		Size: 5.7 MB (5706001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4e1b9223729f0d3aebccfacb5a0b15c96af102a78398ac8b0df5cfa5329e7ed`  
		Last Modified: Wed, 15 Mar 2023 23:43:49 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc31e1ada9713c6aa0ae771c2ff4a99aeaa09bcd46114941d005d37a165d5c8d`  
		Last Modified: Wed, 15 Mar 2023 23:43:49 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74f654e5c408f27396570fc3ebb1bfee8bd77d4e2f82a808aa4ce8cd861ff0af`  
		Last Modified: Wed, 15 Mar 2023 23:43:49 GMT  
		Size: 6.5 KB (6463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:meta`

```console
$ docker pull influxdb@sha256:f2cc8820fb7d417f8284255f4edf73326e75b1b1f8b3f0db0a869f5fd93cb5a6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:meta` - linux; amd64

```console
$ docker pull influxdb@sha256:9949b62ba091bf1e0c6d555a0d62f9c0e3f111d34468c12790701841607c2054
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.5 MB (94504419 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c421d7d950d23de67391a03fa05758737a2990ed39e0371b765c58cfe8d49d27`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Wed, 01 Mar 2023 04:09:45 GMT
ADD file:513c5d5e501279c21a05c1d8b66e5f0b02ee4b27f0b928706d92fd9ce11c1be6 in / 
# Wed, 01 Mar 2023 04:09:46 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 04:42:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 04:42:43 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Mar 2023 00:54:43 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 16 Mar 2023 00:55:02 GMT
ENV INFLUXDB_VERSION=1.8.10-c1.8.10
# Thu, 16 Mar 2023 00:55:28 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-meta_${INFLUXDB_VERSION}_amd64.deb*
# Thu, 16 Mar 2023 00:55:28 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Thu, 16 Mar 2023 00:55:28 GMT
EXPOSE 8091
# Thu, 16 Mar 2023 00:55:28 GMT
VOLUME [/var/lib/influxdb]
# Thu, 16 Mar 2023 00:55:28 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Thu, 16 Mar 2023 00:55:28 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 16 Mar 2023 00:55:28 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:32fb02163b6bb519a30f909008e852354dae10bdfd6b34190dbdfe8f15403ea0`  
		Last Modified: Wed, 01 Mar 2023 04:13:58 GMT  
		Size: 55.0 MB (55045922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:167c7feebee855d117e192389484ea8367be1ba84e7ee35f4e5e5663195facbf`  
		Last Modified: Wed, 01 Mar 2023 04:50:15 GMT  
		Size: 5.2 MB (5166586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6dfff1f6f3ddd2194ea0775f199572e8b2d75c38713eef0444d6b1fd0ac7604`  
		Last Modified: Wed, 01 Mar 2023 04:50:15 GMT  
		Size: 10.9 MB (10876729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a90f0187c37c44f2ad04f9d930d40ee0b886fc8d783b914b10a620683739873`  
		Last Modified: Thu, 16 Mar 2023 00:58:47 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4da79a67cea3e0423fbd017b960736725ee1a9d645259e5e116f7b80f65e3ffb`  
		Last Modified: Thu, 16 Mar 2023 00:59:57 GMT  
		Size: 23.4 MB (23412815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:467317e0fc8b77b1ea7e470e0bb2acd70c9fbc0666761d3a46c639cf1a4bd57a`  
		Last Modified: Thu, 16 Mar 2023 00:59:54 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2476469e17a280c1a07bbbe66a0c405e79e95fe2a45baf4f259f8d0942389de`  
		Last Modified: Thu, 16 Mar 2023 00:59:54 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:meta-alpine`

```console
$ docker pull influxdb@sha256:b332bb7ba17ea35119db932b2f532aba89d7cf9008f3c53ca0cb572e1b465492
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:meta-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:d47c4b7d73fe4dab3506b30191fb878ff88e235e33a57ec221fc5243f1de5229
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.1 MB (28141489 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3401b5ccad79633922a0201457f58a455907b6280a3aa68c53a079dff96d0220`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:42 GMT
ADD file:40887ab7c06977737e63c215c9bd297c0c74de8d12d16ebdf1c3d40ac392f62d in / 
# Sat, 11 Feb 2023 04:46:42 GMT
CMD ["/bin/sh"]
# Mon, 13 Mar 2023 23:20:24 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 16 Mar 2023 00:54:52 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Thu, 16 Mar 2023 00:55:13 GMT
ENV INFLUXDB_VERSION=1.8.10-c1.8.10
# Thu, 16 Mar 2023 00:55:36 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb-meta.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Thu, 16 Mar 2023 00:55:37 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Thu, 16 Mar 2023 00:55:37 GMT
EXPOSE 8091
# Thu, 16 Mar 2023 00:55:37 GMT
VOLUME [/var/lib/influxdb]
# Thu, 16 Mar 2023 00:55:37 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Thu, 16 Mar 2023 00:55:37 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 16 Mar 2023 00:55:37 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:63b65145d645c1250c391b2d16ebe53b3747c295ca8ba2fcb6b0cf064a4dc21c`  
		Last Modified: Fri, 10 Feb 2023 22:41:31 GMT  
		Size: 3.4 MB (3374446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69b7a2cbfc2f3b3305293d689573f3c9651d6053e5f780a9ba42a4c836d8d6c9`  
		Last Modified: Mon, 13 Mar 2023 23:21:18 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5b0a9605b8bc1c4f3b877c51f73e8d0cc4b02403f8f9d18c276f012b604c038`  
		Last Modified: Thu, 16 Mar 2023 00:59:03 GMT  
		Size: 1.5 MB (1472712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9765a5f3bc0d01c3d573bd99fa2c9c6b278d99a9738cd4da9bf3dadb610b22ce`  
		Last Modified: Thu, 16 Mar 2023 01:00:19 GMT  
		Size: 23.3 MB (23293461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ca8edc79b71d358c7eeb599969087beb75b17b94b72e37e85056251578cf1ac`  
		Last Modified: Thu, 16 Mar 2023 01:00:16 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9ab6bb76bc121d5c9b2d774be4fcc78dd5b2b36148a3599db35a72a0861a51f`  
		Last Modified: Thu, 16 Mar 2023 01:00:16 GMT  
		Size: 373.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
