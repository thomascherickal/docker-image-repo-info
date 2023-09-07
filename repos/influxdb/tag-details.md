<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `influxdb`

-	[`influxdb:1.10-data`](#influxdb110-data)
-	[`influxdb:1.10-data-alpine`](#influxdb110-data-alpine)
-	[`influxdb:1.10-meta`](#influxdb110-meta)
-	[`influxdb:1.10-meta-alpine`](#influxdb110-meta-alpine)
-	[`influxdb:1.10.4-data`](#influxdb1104-data)
-	[`influxdb:1.10.4-data-alpine`](#influxdb1104-data-alpine)
-	[`influxdb:1.10.4-meta`](#influxdb1104-meta)
-	[`influxdb:1.10.4-meta-alpine`](#influxdb1104-meta-alpine)
-	[`influxdb:1.11-data`](#influxdb111-data)
-	[`influxdb:1.11-data-alpine`](#influxdb111-data-alpine)
-	[`influxdb:1.11-meta`](#influxdb111-meta)
-	[`influxdb:1.11-meta-alpine`](#influxdb111-meta-alpine)
-	[`influxdb:1.11.1-data`](#influxdb1111-data)
-	[`influxdb:1.11.1-data-alpine`](#influxdb1111-data-alpine)
-	[`influxdb:1.11.1-meta`](#influxdb1111-meta)
-	[`influxdb:1.11.1-meta-alpine`](#influxdb1111-meta-alpine)
-	[`influxdb:1.8`](#influxdb18)
-	[`influxdb:1.8-alpine`](#influxdb18-alpine)
-	[`influxdb:1.8.10`](#influxdb1810)
-	[`influxdb:1.8.10-alpine`](#influxdb1810-alpine)
-	[`influxdb:1.9-data`](#influxdb19-data)
-	[`influxdb:1.9-data-alpine`](#influxdb19-data-alpine)
-	[`influxdb:1.9-meta`](#influxdb19-meta)
-	[`influxdb:1.9-meta-alpine`](#influxdb19-meta-alpine)
-	[`influxdb:1.9.12-data`](#influxdb1912-data)
-	[`influxdb:1.9.12-data-alpine`](#influxdb1912-data-alpine)
-	[`influxdb:1.9.12-meta`](#influxdb1912-meta)
-	[`influxdb:1.9.12-meta-alpine`](#influxdb1912-meta-alpine)
-	[`influxdb:2.7`](#influxdb27)
-	[`influxdb:2.7-alpine`](#influxdb27-alpine)
-	[`influxdb:2.7.1`](#influxdb271)
-	[`influxdb:2.7.1-alpine`](#influxdb271-alpine)
-	[`influxdb:alpine`](#influxdbalpine)
-	[`influxdb:latest`](#influxdblatest)

## `influxdb:1.10-data`

```console
$ docker pull influxdb@sha256:0d9adec03446ecd502c15112bc725e77984baddd59996180dfaa1c1ac0306a22
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.10-data` - linux; amd64

```console
$ docker pull influxdb@sha256:5c4361b48dad5fb9d3a506c734df5f33a9a0ede7037c93975b44915a69c676ab
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.9 MB (110892856 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ef5eb133a93d999f96e526aee80668020f580df9ac5e751e2e3a3aebcb03fc7b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 16 Aug 2023 00:59:57 GMT
ADD file:20f89ff93bfbd6c9fb1a97058a1f3de4485a8974e8a83892072c511fbd2e4134 in / 
# Wed, 16 Aug 2023 00:59:58 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 06:59:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Aug 2023 01:50:12 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 17 Aug 2023 01:50:41 GMT
ENV INFLUXDB_VERSION=1.10.4-c1.10.4
# Thu, 17 Aug 2023 01:50:46 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-data_${INFLUXDB_VERSION}_amd64.deb*
# Thu, 17 Aug 2023 01:50:46 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Thu, 17 Aug 2023 01:50:46 GMT
EXPOSE 8086
# Thu, 17 Aug 2023 01:50:46 GMT
VOLUME [/var/lib/influxdb]
# Thu, 17 Aug 2023 01:50:47 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Thu, 17 Aug 2023 01:50:47 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Thu, 17 Aug 2023 01:50:47 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Aug 2023 01:50:47 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:6a70103cc499a199e10e379794c60aa524d9598587cc2bdfe2995642c2da8df7`  
		Last Modified: Wed, 16 Aug 2023 01:04:50 GMT  
		Size: 55.1 MB (55056621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccb4221e2c63c35bb16b63f6d24c104c7ea5d453997636c2244b66884f540537`  
		Last Modified: Wed, 16 Aug 2023 07:13:46 GMT  
		Size: 15.8 MB (15760534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89b46b2782c35ef5f65808b1b87f49bfe8827c8c03be281c098d7e2f832b617f`  
		Last Modified: Thu, 17 Aug 2023 01:51:49 GMT  
		Size: 1.8 KB (1806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:315bbdc029563a4c939d78f55cd7bd83bc43c7946d253a2c6789cf0878444f84`  
		Last Modified: Thu, 17 Aug 2023 01:52:36 GMT  
		Size: 40.1 MB (40072118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bddc5a42b2e4118551c0b6c0498f5577d79c307e204adf145cba9c9a65ea190`  
		Last Modified: Thu, 17 Aug 2023 01:52:30 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1acb880b09b7dc27705a5cd73d47c38f68f1620fd79fd9fd23357d3d0937369a`  
		Last Modified: Thu, 17 Aug 2023 01:52:30 GMT  
		Size: 252.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:436a7980327fad3887aefbe453a4914c6cda48525bb22033aa16fa6f86bf699b`  
		Last Modified: Thu, 17 Aug 2023 01:52:31 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.10-data-alpine`

```console
$ docker pull influxdb@sha256:30fd78b53b38603b803dee28115442e42fc74a72d6abf494de45ba1919333c46
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.10-data-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:00b07bb81d22caa994b5e3a4981f9675a9d775de134ee0fa582113f733c63133
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.9 MB (44884881 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:10059de6556cc0bec7fea3ac59f115490dc969cd4d5cc8ee50211fccf768de0d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:26 GMT
ADD file:6dd87346b8be240b21b4f4d9296253bf0d28b6579aa52d2118872e3936963b6b in / 
# Mon, 07 Aug 2023 19:20:26 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 20:30:41 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 09 Aug 2023 01:54:15 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Wed, 09 Aug 2023 01:54:54 GMT
ENV INFLUXDB_VERSION=1.10.4-c1.10.4
# Wed, 09 Aug 2023 01:55:02 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb.conf &&     chmod +x /usr/src/influxdb-*/fs/usr/bin/* &&     cp -a /usr/src/influxdb-*/fs/usr/bin/. /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Wed, 09 Aug 2023 01:55:02 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Wed, 09 Aug 2023 01:55:02 GMT
EXPOSE 8086
# Wed, 09 Aug 2023 01:55:02 GMT
VOLUME [/var/lib/influxdb]
# Wed, 09 Aug 2023 01:55:02 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Wed, 09 Aug 2023 01:55:02 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Wed, 09 Aug 2023 01:55:02 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 09 Aug 2023 01:55:02 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:9398808236ffac29e60c04ec906d8d409af7fa19dc57d8c65ad167e9c4967006`  
		Last Modified: Mon, 07 Aug 2023 19:21:08 GMT  
		Size: 3.4 MB (3378609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bdca2725167af68b5a2e88c072759b23a3bf0e32c8526c7e9b89f616db5a88d`  
		Last Modified: Mon, 07 Aug 2023 20:31:39 GMT  
		Size: 279.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90412949f8cfd74e35fbc8d623c490f3d19ec67abaac2447d3f55007f36a18a1`  
		Last Modified: Wed, 09 Aug 2023 01:56:21 GMT  
		Size: 1.5 MB (1472417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d99fa3e00b6a2e37099b0035955aae40e8d948ded7e4edf294034bcd91f5414e`  
		Last Modified: Wed, 09 Aug 2023 01:57:08 GMT  
		Size: 40.0 MB (40031778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1d3babb693246bc8e99099654f014f2ea53a5c18e681959daa902986d3864b8`  
		Last Modified: Wed, 09 Aug 2023 01:57:03 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fdaf741ffe4145e4313a0495b08cdd8639b285c9723590d7684926352bfc0ed`  
		Last Modified: Wed, 09 Aug 2023 01:57:02 GMT  
		Size: 252.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e017fc3ac2b1809daacbdfb0f249a2f6716d12e0d857cdbde9c0f3ae220c2848`  
		Last Modified: Wed, 09 Aug 2023 01:57:03 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.10-meta`

```console
$ docker pull influxdb@sha256:90ff46c435594efa1a308ac59c43d8b8eec1a7bfe2cd95f3ceb4ed2664e84f6a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.10-meta` - linux; amd64

```console
$ docker pull influxdb@sha256:757167b6e1f407f00bf9760470eb1817ea133425804160f15ff23d9e31c60673
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.1 MB (91057805 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ab2ed3a5017fa995426f9d4c3fcaf944aafa802968d33623653a86b3c85218b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Wed, 16 Aug 2023 00:59:57 GMT
ADD file:20f89ff93bfbd6c9fb1a97058a1f3de4485a8974e8a83892072c511fbd2e4134 in / 
# Wed, 16 Aug 2023 00:59:58 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 06:59:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Aug 2023 01:50:12 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 17 Aug 2023 01:50:41 GMT
ENV INFLUXDB_VERSION=1.10.4-c1.10.4
# Thu, 17 Aug 2023 01:50:56 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-meta_${INFLUXDB_VERSION}_amd64.deb*
# Thu, 17 Aug 2023 01:50:56 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Thu, 17 Aug 2023 01:50:56 GMT
EXPOSE 8091
# Thu, 17 Aug 2023 01:50:56 GMT
VOLUME [/var/lib/influxdb]
# Thu, 17 Aug 2023 01:50:56 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Thu, 17 Aug 2023 01:50:56 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Aug 2023 01:50:56 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:6a70103cc499a199e10e379794c60aa524d9598587cc2bdfe2995642c2da8df7`  
		Last Modified: Wed, 16 Aug 2023 01:04:50 GMT  
		Size: 55.1 MB (55056621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccb4221e2c63c35bb16b63f6d24c104c7ea5d453997636c2244b66884f540537`  
		Last Modified: Wed, 16 Aug 2023 07:13:46 GMT  
		Size: 15.8 MB (15760534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89b46b2782c35ef5f65808b1b87f49bfe8827c8c03be281c098d7e2f832b617f`  
		Last Modified: Thu, 17 Aug 2023 01:51:49 GMT  
		Size: 1.8 KB (1806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1fb1beee509820904b83d76b962dc0c358fe549122dbf001a587038321aa437`  
		Last Modified: Thu, 17 Aug 2023 01:52:49 GMT  
		Size: 20.2 MB (20238272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d28191b74b4e7287e3e6d87bd8b2567d6fa6aa01f8cd7274099069760866c3a1`  
		Last Modified: Thu, 17 Aug 2023 01:52:46 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c3d6fcc3d722d0e1af6309f73a10d28e9ef15de0459fa5051162eca0530c2f3`  
		Last Modified: Thu, 17 Aug 2023 01:52:46 GMT  
		Size: 375.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.10-meta-alpine`

```console
$ docker pull influxdb@sha256:582e81312d445b39425347274f81de9755e6958c82be1a296cd851ccf257fb69
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.10-meta-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:d358f770c09053edb026a169659cfce3319ff7d267657d6e4ea985d5d4f4ffa4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.1 MB (25058369 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a54933f3052bfc6032d85bf31500b778db7b09b9807bb46be6971b6424d1c98`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:26 GMT
ADD file:6dd87346b8be240b21b4f4d9296253bf0d28b6579aa52d2118872e3936963b6b in / 
# Mon, 07 Aug 2023 19:20:26 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 20:30:41 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 09 Aug 2023 01:54:15 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Wed, 09 Aug 2023 01:54:54 GMT
ENV INFLUXDB_VERSION=1.10.4-c1.10.4
# Wed, 09 Aug 2023 01:55:14 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb-meta.conf &&     chmod +x /usr/src/influxdb-*/fs/usr/bin/* &&     cp -a /usr/src/influxdb-*/fs/usr/bin/. /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Wed, 09 Aug 2023 01:55:14 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Wed, 09 Aug 2023 01:55:14 GMT
EXPOSE 8091
# Wed, 09 Aug 2023 01:55:14 GMT
VOLUME [/var/lib/influxdb]
# Wed, 09 Aug 2023 01:55:14 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Wed, 09 Aug 2023 01:55:14 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 09 Aug 2023 01:55:14 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:9398808236ffac29e60c04ec906d8d409af7fa19dc57d8c65ad167e9c4967006`  
		Last Modified: Mon, 07 Aug 2023 19:21:08 GMT  
		Size: 3.4 MB (3378609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bdca2725167af68b5a2e88c072759b23a3bf0e32c8526c7e9b89f616db5a88d`  
		Last Modified: Mon, 07 Aug 2023 20:31:39 GMT  
		Size: 279.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90412949f8cfd74e35fbc8d623c490f3d19ec67abaac2447d3f55007f36a18a1`  
		Last Modified: Wed, 09 Aug 2023 01:56:21 GMT  
		Size: 1.5 MB (1472417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f54371a5b804126a0f61c0f0baeff8c0ae2b12865d0721014d386249acff35d`  
		Last Modified: Wed, 09 Aug 2023 01:57:21 GMT  
		Size: 20.2 MB (20206475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f693434093bbd13721fd2ff8b8b70df510d23339ea7f0dfa831837b5870b3f9b`  
		Last Modified: Wed, 09 Aug 2023 01:57:18 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c582e4c03db9d56825708effb780fba49c61bdeb51b253226ce5b4c0145a736`  
		Last Modified: Wed, 09 Aug 2023 01:57:18 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.10.4-data`

```console
$ docker pull influxdb@sha256:0d9adec03446ecd502c15112bc725e77984baddd59996180dfaa1c1ac0306a22
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.10.4-data` - linux; amd64

```console
$ docker pull influxdb@sha256:5c4361b48dad5fb9d3a506c734df5f33a9a0ede7037c93975b44915a69c676ab
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.9 MB (110892856 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ef5eb133a93d999f96e526aee80668020f580df9ac5e751e2e3a3aebcb03fc7b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 16 Aug 2023 00:59:57 GMT
ADD file:20f89ff93bfbd6c9fb1a97058a1f3de4485a8974e8a83892072c511fbd2e4134 in / 
# Wed, 16 Aug 2023 00:59:58 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 06:59:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Aug 2023 01:50:12 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 17 Aug 2023 01:50:41 GMT
ENV INFLUXDB_VERSION=1.10.4-c1.10.4
# Thu, 17 Aug 2023 01:50:46 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-data_${INFLUXDB_VERSION}_amd64.deb*
# Thu, 17 Aug 2023 01:50:46 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Thu, 17 Aug 2023 01:50:46 GMT
EXPOSE 8086
# Thu, 17 Aug 2023 01:50:46 GMT
VOLUME [/var/lib/influxdb]
# Thu, 17 Aug 2023 01:50:47 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Thu, 17 Aug 2023 01:50:47 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Thu, 17 Aug 2023 01:50:47 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Aug 2023 01:50:47 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:6a70103cc499a199e10e379794c60aa524d9598587cc2bdfe2995642c2da8df7`  
		Last Modified: Wed, 16 Aug 2023 01:04:50 GMT  
		Size: 55.1 MB (55056621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccb4221e2c63c35bb16b63f6d24c104c7ea5d453997636c2244b66884f540537`  
		Last Modified: Wed, 16 Aug 2023 07:13:46 GMT  
		Size: 15.8 MB (15760534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89b46b2782c35ef5f65808b1b87f49bfe8827c8c03be281c098d7e2f832b617f`  
		Last Modified: Thu, 17 Aug 2023 01:51:49 GMT  
		Size: 1.8 KB (1806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:315bbdc029563a4c939d78f55cd7bd83bc43c7946d253a2c6789cf0878444f84`  
		Last Modified: Thu, 17 Aug 2023 01:52:36 GMT  
		Size: 40.1 MB (40072118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bddc5a42b2e4118551c0b6c0498f5577d79c307e204adf145cba9c9a65ea190`  
		Last Modified: Thu, 17 Aug 2023 01:52:30 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1acb880b09b7dc27705a5cd73d47c38f68f1620fd79fd9fd23357d3d0937369a`  
		Last Modified: Thu, 17 Aug 2023 01:52:30 GMT  
		Size: 252.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:436a7980327fad3887aefbe453a4914c6cda48525bb22033aa16fa6f86bf699b`  
		Last Modified: Thu, 17 Aug 2023 01:52:31 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.10.4-data-alpine`

```console
$ docker pull influxdb@sha256:30fd78b53b38603b803dee28115442e42fc74a72d6abf494de45ba1919333c46
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.10.4-data-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:00b07bb81d22caa994b5e3a4981f9675a9d775de134ee0fa582113f733c63133
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.9 MB (44884881 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:10059de6556cc0bec7fea3ac59f115490dc969cd4d5cc8ee50211fccf768de0d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:26 GMT
ADD file:6dd87346b8be240b21b4f4d9296253bf0d28b6579aa52d2118872e3936963b6b in / 
# Mon, 07 Aug 2023 19:20:26 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 20:30:41 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 09 Aug 2023 01:54:15 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Wed, 09 Aug 2023 01:54:54 GMT
ENV INFLUXDB_VERSION=1.10.4-c1.10.4
# Wed, 09 Aug 2023 01:55:02 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb.conf &&     chmod +x /usr/src/influxdb-*/fs/usr/bin/* &&     cp -a /usr/src/influxdb-*/fs/usr/bin/. /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Wed, 09 Aug 2023 01:55:02 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Wed, 09 Aug 2023 01:55:02 GMT
EXPOSE 8086
# Wed, 09 Aug 2023 01:55:02 GMT
VOLUME [/var/lib/influxdb]
# Wed, 09 Aug 2023 01:55:02 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Wed, 09 Aug 2023 01:55:02 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Wed, 09 Aug 2023 01:55:02 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 09 Aug 2023 01:55:02 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:9398808236ffac29e60c04ec906d8d409af7fa19dc57d8c65ad167e9c4967006`  
		Last Modified: Mon, 07 Aug 2023 19:21:08 GMT  
		Size: 3.4 MB (3378609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bdca2725167af68b5a2e88c072759b23a3bf0e32c8526c7e9b89f616db5a88d`  
		Last Modified: Mon, 07 Aug 2023 20:31:39 GMT  
		Size: 279.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90412949f8cfd74e35fbc8d623c490f3d19ec67abaac2447d3f55007f36a18a1`  
		Last Modified: Wed, 09 Aug 2023 01:56:21 GMT  
		Size: 1.5 MB (1472417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d99fa3e00b6a2e37099b0035955aae40e8d948ded7e4edf294034bcd91f5414e`  
		Last Modified: Wed, 09 Aug 2023 01:57:08 GMT  
		Size: 40.0 MB (40031778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1d3babb693246bc8e99099654f014f2ea53a5c18e681959daa902986d3864b8`  
		Last Modified: Wed, 09 Aug 2023 01:57:03 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fdaf741ffe4145e4313a0495b08cdd8639b285c9723590d7684926352bfc0ed`  
		Last Modified: Wed, 09 Aug 2023 01:57:02 GMT  
		Size: 252.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e017fc3ac2b1809daacbdfb0f249a2f6716d12e0d857cdbde9c0f3ae220c2848`  
		Last Modified: Wed, 09 Aug 2023 01:57:03 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.10.4-meta`

```console
$ docker pull influxdb@sha256:90ff46c435594efa1a308ac59c43d8b8eec1a7bfe2cd95f3ceb4ed2664e84f6a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.10.4-meta` - linux; amd64

```console
$ docker pull influxdb@sha256:757167b6e1f407f00bf9760470eb1817ea133425804160f15ff23d9e31c60673
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.1 MB (91057805 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ab2ed3a5017fa995426f9d4c3fcaf944aafa802968d33623653a86b3c85218b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Wed, 16 Aug 2023 00:59:57 GMT
ADD file:20f89ff93bfbd6c9fb1a97058a1f3de4485a8974e8a83892072c511fbd2e4134 in / 
# Wed, 16 Aug 2023 00:59:58 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 06:59:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Aug 2023 01:50:12 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 17 Aug 2023 01:50:41 GMT
ENV INFLUXDB_VERSION=1.10.4-c1.10.4
# Thu, 17 Aug 2023 01:50:56 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-meta_${INFLUXDB_VERSION}_amd64.deb*
# Thu, 17 Aug 2023 01:50:56 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Thu, 17 Aug 2023 01:50:56 GMT
EXPOSE 8091
# Thu, 17 Aug 2023 01:50:56 GMT
VOLUME [/var/lib/influxdb]
# Thu, 17 Aug 2023 01:50:56 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Thu, 17 Aug 2023 01:50:56 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Aug 2023 01:50:56 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:6a70103cc499a199e10e379794c60aa524d9598587cc2bdfe2995642c2da8df7`  
		Last Modified: Wed, 16 Aug 2023 01:04:50 GMT  
		Size: 55.1 MB (55056621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccb4221e2c63c35bb16b63f6d24c104c7ea5d453997636c2244b66884f540537`  
		Last Modified: Wed, 16 Aug 2023 07:13:46 GMT  
		Size: 15.8 MB (15760534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89b46b2782c35ef5f65808b1b87f49bfe8827c8c03be281c098d7e2f832b617f`  
		Last Modified: Thu, 17 Aug 2023 01:51:49 GMT  
		Size: 1.8 KB (1806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1fb1beee509820904b83d76b962dc0c358fe549122dbf001a587038321aa437`  
		Last Modified: Thu, 17 Aug 2023 01:52:49 GMT  
		Size: 20.2 MB (20238272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d28191b74b4e7287e3e6d87bd8b2567d6fa6aa01f8cd7274099069760866c3a1`  
		Last Modified: Thu, 17 Aug 2023 01:52:46 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c3d6fcc3d722d0e1af6309f73a10d28e9ef15de0459fa5051162eca0530c2f3`  
		Last Modified: Thu, 17 Aug 2023 01:52:46 GMT  
		Size: 375.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.10.4-meta-alpine`

```console
$ docker pull influxdb@sha256:582e81312d445b39425347274f81de9755e6958c82be1a296cd851ccf257fb69
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.10.4-meta-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:d358f770c09053edb026a169659cfce3319ff7d267657d6e4ea985d5d4f4ffa4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.1 MB (25058369 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a54933f3052bfc6032d85bf31500b778db7b09b9807bb46be6971b6424d1c98`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:26 GMT
ADD file:6dd87346b8be240b21b4f4d9296253bf0d28b6579aa52d2118872e3936963b6b in / 
# Mon, 07 Aug 2023 19:20:26 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 20:30:41 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 09 Aug 2023 01:54:15 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Wed, 09 Aug 2023 01:54:54 GMT
ENV INFLUXDB_VERSION=1.10.4-c1.10.4
# Wed, 09 Aug 2023 01:55:14 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb-meta.conf &&     chmod +x /usr/src/influxdb-*/fs/usr/bin/* &&     cp -a /usr/src/influxdb-*/fs/usr/bin/. /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Wed, 09 Aug 2023 01:55:14 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Wed, 09 Aug 2023 01:55:14 GMT
EXPOSE 8091
# Wed, 09 Aug 2023 01:55:14 GMT
VOLUME [/var/lib/influxdb]
# Wed, 09 Aug 2023 01:55:14 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Wed, 09 Aug 2023 01:55:14 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 09 Aug 2023 01:55:14 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:9398808236ffac29e60c04ec906d8d409af7fa19dc57d8c65ad167e9c4967006`  
		Last Modified: Mon, 07 Aug 2023 19:21:08 GMT  
		Size: 3.4 MB (3378609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bdca2725167af68b5a2e88c072759b23a3bf0e32c8526c7e9b89f616db5a88d`  
		Last Modified: Mon, 07 Aug 2023 20:31:39 GMT  
		Size: 279.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90412949f8cfd74e35fbc8d623c490f3d19ec67abaac2447d3f55007f36a18a1`  
		Last Modified: Wed, 09 Aug 2023 01:56:21 GMT  
		Size: 1.5 MB (1472417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f54371a5b804126a0f61c0f0baeff8c0ae2b12865d0721014d386249acff35d`  
		Last Modified: Wed, 09 Aug 2023 01:57:21 GMT  
		Size: 20.2 MB (20206475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f693434093bbd13721fd2ff8b8b70df510d23339ea7f0dfa831837b5870b3f9b`  
		Last Modified: Wed, 09 Aug 2023 01:57:18 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c582e4c03db9d56825708effb780fba49c61bdeb51b253226ce5b4c0145a736`  
		Last Modified: Wed, 09 Aug 2023 01:57:18 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.11-data`

```console
$ docker pull influxdb@sha256:e11a04e1795d9df227f4d64b223d094ea3d2eacc0db2850b884f2b29853e91fa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.11-data` - linux; amd64

```console
$ docker pull influxdb@sha256:4cba5ada6c0751b5206acb46a0d50f20db72e9d1ec229c3d9e129c9dfa399f62
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.0 MB (110978804 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:def5bbf8e862c05cf801b6acd2c2eb950e23c2dbcc6e9e1f85a13607173f0aa4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 16 Aug 2023 00:59:57 GMT
ADD file:20f89ff93bfbd6c9fb1a97058a1f3de4485a8974e8a83892072c511fbd2e4134 in / 
# Wed, 16 Aug 2023 00:59:58 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 06:59:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Aug 2023 01:50:12 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 17 Aug 2023 01:51:01 GMT
ENV INFLUXDB_VERSION=1.11.1-c1.11.1
# Thu, 17 Aug 2023 01:51:06 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-data_${INFLUXDB_VERSION}_amd64.deb*
# Thu, 17 Aug 2023 01:51:06 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Thu, 17 Aug 2023 01:51:06 GMT
EXPOSE 8086
# Thu, 17 Aug 2023 01:51:06 GMT
VOLUME [/var/lib/influxdb]
# Thu, 17 Aug 2023 01:51:07 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Thu, 17 Aug 2023 01:51:07 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Thu, 17 Aug 2023 01:51:07 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Aug 2023 01:51:07 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:6a70103cc499a199e10e379794c60aa524d9598587cc2bdfe2995642c2da8df7`  
		Last Modified: Wed, 16 Aug 2023 01:04:50 GMT  
		Size: 55.1 MB (55056621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccb4221e2c63c35bb16b63f6d24c104c7ea5d453997636c2244b66884f540537`  
		Last Modified: Wed, 16 Aug 2023 07:13:46 GMT  
		Size: 15.8 MB (15760534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89b46b2782c35ef5f65808b1b87f49bfe8827c8c03be281c098d7e2f832b617f`  
		Last Modified: Thu, 17 Aug 2023 01:51:49 GMT  
		Size: 1.8 KB (1806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21bff6c9fbdd6a2df029de26fae5723f88a7130c6044fc03cc4c3e0b7d176a65`  
		Last Modified: Thu, 17 Aug 2023 01:53:05 GMT  
		Size: 40.2 MB (40158064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b6739fea59e5b8a82f2d2fe8cf0c1146fc228704711b67790413ebcd7d04f9a`  
		Last Modified: Thu, 17 Aug 2023 01:52:59 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f1e9c3206a3e53b08fae7a5e328638c69f38961f96e291a98173ddfea903449`  
		Last Modified: Thu, 17 Aug 2023 01:52:59 GMT  
		Size: 252.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bff5f0fb771818ef68375e2658aa3abed006f00b462825b301e61c82c4533fb4`  
		Last Modified: Thu, 17 Aug 2023 01:52:59 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.11-data-alpine`

```console
$ docker pull influxdb@sha256:62684d55e7c7888069b9c4d17e3a416496a37f346df8ac5d888c71ce68deb7ee
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.11-data-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:8a8bd9bc75019bacd70da3bf5c39fff3b09e4c8af72983c7d5e4448946424f89
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.0 MB (44967875 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4997a8a94a1d6d440e27997698f97f5d7342dcb74768525efe222b42ef9fb923`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:26 GMT
ADD file:6dd87346b8be240b21b4f4d9296253bf0d28b6579aa52d2118872e3936963b6b in / 
# Mon, 07 Aug 2023 19:20:26 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 20:30:41 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 09 Aug 2023 01:54:15 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Wed, 09 Aug 2023 01:55:20 GMT
ENV INFLUXDB_VERSION=1.11.1-c1.11.1
# Wed, 09 Aug 2023 01:55:26 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb.conf &&     chmod +x /usr/src/influxdb-*/fs/usr/bin/* &&     cp -a /usr/src/influxdb-*/fs/usr/bin/. /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Wed, 09 Aug 2023 01:55:26 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Wed, 09 Aug 2023 01:55:26 GMT
EXPOSE 8086
# Wed, 09 Aug 2023 01:55:27 GMT
VOLUME [/var/lib/influxdb]
# Wed, 09 Aug 2023 01:55:27 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Wed, 09 Aug 2023 01:55:27 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Wed, 09 Aug 2023 01:55:27 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 09 Aug 2023 01:55:27 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:9398808236ffac29e60c04ec906d8d409af7fa19dc57d8c65ad167e9c4967006`  
		Last Modified: Mon, 07 Aug 2023 19:21:08 GMT  
		Size: 3.4 MB (3378609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bdca2725167af68b5a2e88c072759b23a3bf0e32c8526c7e9b89f616db5a88d`  
		Last Modified: Mon, 07 Aug 2023 20:31:39 GMT  
		Size: 279.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90412949f8cfd74e35fbc8d623c490f3d19ec67abaac2447d3f55007f36a18a1`  
		Last Modified: Wed, 09 Aug 2023 01:56:21 GMT  
		Size: 1.5 MB (1472417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4595e71ccc84641653b90d260127756204fdfea1a54f0a713ca71f01598a2b8`  
		Last Modified: Wed, 09 Aug 2023 01:57:37 GMT  
		Size: 40.1 MB (40114773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ead09dda79ec4a08283520fcbb457330f36bd8a1480baaf61be1e3d2aa6179fd`  
		Last Modified: Wed, 09 Aug 2023 01:57:30 GMT  
		Size: 264.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:849f4b1b089f63a045d817d11f2ca1c6657b523d35e229ad0e04365cd66338e3`  
		Last Modified: Wed, 09 Aug 2023 01:57:30 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab3c8f493dbc4fb1c0665f7b9adb9e83b07f09454da4372b53415cd4d32fec85`  
		Last Modified: Wed, 09 Aug 2023 01:57:30 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.11-meta`

```console
$ docker pull influxdb@sha256:12f9a7a51f2d54b959fca4b1266028b3f0a1cef55297d865305586f4da3031a4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.11-meta` - linux; amd64

```console
$ docker pull influxdb@sha256:797f251b9263b06a2a73feffc26855da192e0034f791bbe9ae83cfb6121de31b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.1 MB (91068557 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac15bdc40197c186642f8bd0d7f3f377f3a914891fad5cc3034d6644af5a8571`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Wed, 16 Aug 2023 00:59:57 GMT
ADD file:20f89ff93bfbd6c9fb1a97058a1f3de4485a8974e8a83892072c511fbd2e4134 in / 
# Wed, 16 Aug 2023 00:59:58 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 06:59:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Aug 2023 01:50:12 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 17 Aug 2023 01:51:01 GMT
ENV INFLUXDB_VERSION=1.11.1-c1.11.1
# Thu, 17 Aug 2023 01:51:15 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-meta_${INFLUXDB_VERSION}_amd64.deb*
# Thu, 17 Aug 2023 01:51:16 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Thu, 17 Aug 2023 01:51:16 GMT
EXPOSE 8091
# Thu, 17 Aug 2023 01:51:16 GMT
VOLUME [/var/lib/influxdb]
# Thu, 17 Aug 2023 01:51:16 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Thu, 17 Aug 2023 01:51:16 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Aug 2023 01:51:16 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:6a70103cc499a199e10e379794c60aa524d9598587cc2bdfe2995642c2da8df7`  
		Last Modified: Wed, 16 Aug 2023 01:04:50 GMT  
		Size: 55.1 MB (55056621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccb4221e2c63c35bb16b63f6d24c104c7ea5d453997636c2244b66884f540537`  
		Last Modified: Wed, 16 Aug 2023 07:13:46 GMT  
		Size: 15.8 MB (15760534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89b46b2782c35ef5f65808b1b87f49bfe8827c8c03be281c098d7e2f832b617f`  
		Last Modified: Thu, 17 Aug 2023 01:51:49 GMT  
		Size: 1.8 KB (1806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d861715c583388699cfe8fce7754fb95921e9bd9c8688c44463442fb5225ca4`  
		Last Modified: Thu, 17 Aug 2023 01:53:17 GMT  
		Size: 20.2 MB (20249023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0dbfe4340f563fbfe7a01ae6a6e2ea913660c1ad384c77ca3c2dec1ef52e11a`  
		Last Modified: Thu, 17 Aug 2023 01:53:14 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc1938c07a5ee85efffc4b7e71bfb39e945fe67772e69c403ab93c11a044dd12`  
		Last Modified: Thu, 17 Aug 2023 01:53:14 GMT  
		Size: 375.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.11-meta-alpine`

```console
$ docker pull influxdb@sha256:953d6274978df9a3280fa1aea7a0c4dae9ccc74b59e4388262c9bd025cafc6d1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.11-meta-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:fc5b9e422f6127a618a236c9b387a20651aa77fbb9162f3e8c99921f0e482ee3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.1 MB (25064242 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:74b55a257f61e31f28cac10586355617d61b72c6c79a4f00e813cfab059bca1b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:26 GMT
ADD file:6dd87346b8be240b21b4f4d9296253bf0d28b6579aa52d2118872e3936963b6b in / 
# Mon, 07 Aug 2023 19:20:26 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 20:30:41 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 09 Aug 2023 01:54:15 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Wed, 09 Aug 2023 01:55:20 GMT
ENV INFLUXDB_VERSION=1.11.1-c1.11.1
# Wed, 09 Aug 2023 01:55:37 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb-meta.conf &&     chmod +x /usr/src/influxdb-*/fs/usr/bin/* &&     cp -a /usr/src/influxdb-*/fs/usr/bin/. /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Wed, 09 Aug 2023 01:55:37 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Wed, 09 Aug 2023 01:55:37 GMT
EXPOSE 8091
# Wed, 09 Aug 2023 01:55:37 GMT
VOLUME [/var/lib/influxdb]
# Wed, 09 Aug 2023 01:55:37 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Wed, 09 Aug 2023 01:55:38 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 09 Aug 2023 01:55:38 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:9398808236ffac29e60c04ec906d8d409af7fa19dc57d8c65ad167e9c4967006`  
		Last Modified: Mon, 07 Aug 2023 19:21:08 GMT  
		Size: 3.4 MB (3378609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bdca2725167af68b5a2e88c072759b23a3bf0e32c8526c7e9b89f616db5a88d`  
		Last Modified: Mon, 07 Aug 2023 20:31:39 GMT  
		Size: 279.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90412949f8cfd74e35fbc8d623c490f3d19ec67abaac2447d3f55007f36a18a1`  
		Last Modified: Wed, 09 Aug 2023 01:56:21 GMT  
		Size: 1.5 MB (1472417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04b359de245bd88b2c968ebc3faaee5545903535961cc4174445077b828be50e`  
		Last Modified: Wed, 09 Aug 2023 01:57:49 GMT  
		Size: 20.2 MB (20212341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de0b08635ca3ea71c43f912a8a7fa599881ab95aeda951e261aaabd12c4dac64`  
		Last Modified: Wed, 09 Aug 2023 01:57:46 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0f7d3459e4b0362cd4c64b3b6750f2dbea18a04a270a1c71ed67da55c12c00f`  
		Last Modified: Wed, 09 Aug 2023 01:57:46 GMT  
		Size: 375.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.11.1-data`

```console
$ docker pull influxdb@sha256:e11a04e1795d9df227f4d64b223d094ea3d2eacc0db2850b884f2b29853e91fa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.11.1-data` - linux; amd64

```console
$ docker pull influxdb@sha256:4cba5ada6c0751b5206acb46a0d50f20db72e9d1ec229c3d9e129c9dfa399f62
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.0 MB (110978804 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:def5bbf8e862c05cf801b6acd2c2eb950e23c2dbcc6e9e1f85a13607173f0aa4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 16 Aug 2023 00:59:57 GMT
ADD file:20f89ff93bfbd6c9fb1a97058a1f3de4485a8974e8a83892072c511fbd2e4134 in / 
# Wed, 16 Aug 2023 00:59:58 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 06:59:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Aug 2023 01:50:12 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 17 Aug 2023 01:51:01 GMT
ENV INFLUXDB_VERSION=1.11.1-c1.11.1
# Thu, 17 Aug 2023 01:51:06 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-data_${INFLUXDB_VERSION}_amd64.deb*
# Thu, 17 Aug 2023 01:51:06 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Thu, 17 Aug 2023 01:51:06 GMT
EXPOSE 8086
# Thu, 17 Aug 2023 01:51:06 GMT
VOLUME [/var/lib/influxdb]
# Thu, 17 Aug 2023 01:51:07 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Thu, 17 Aug 2023 01:51:07 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Thu, 17 Aug 2023 01:51:07 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Aug 2023 01:51:07 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:6a70103cc499a199e10e379794c60aa524d9598587cc2bdfe2995642c2da8df7`  
		Last Modified: Wed, 16 Aug 2023 01:04:50 GMT  
		Size: 55.1 MB (55056621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccb4221e2c63c35bb16b63f6d24c104c7ea5d453997636c2244b66884f540537`  
		Last Modified: Wed, 16 Aug 2023 07:13:46 GMT  
		Size: 15.8 MB (15760534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89b46b2782c35ef5f65808b1b87f49bfe8827c8c03be281c098d7e2f832b617f`  
		Last Modified: Thu, 17 Aug 2023 01:51:49 GMT  
		Size: 1.8 KB (1806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21bff6c9fbdd6a2df029de26fae5723f88a7130c6044fc03cc4c3e0b7d176a65`  
		Last Modified: Thu, 17 Aug 2023 01:53:05 GMT  
		Size: 40.2 MB (40158064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b6739fea59e5b8a82f2d2fe8cf0c1146fc228704711b67790413ebcd7d04f9a`  
		Last Modified: Thu, 17 Aug 2023 01:52:59 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f1e9c3206a3e53b08fae7a5e328638c69f38961f96e291a98173ddfea903449`  
		Last Modified: Thu, 17 Aug 2023 01:52:59 GMT  
		Size: 252.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bff5f0fb771818ef68375e2658aa3abed006f00b462825b301e61c82c4533fb4`  
		Last Modified: Thu, 17 Aug 2023 01:52:59 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.11.1-data-alpine`

```console
$ docker pull influxdb@sha256:62684d55e7c7888069b9c4d17e3a416496a37f346df8ac5d888c71ce68deb7ee
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.11.1-data-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:8a8bd9bc75019bacd70da3bf5c39fff3b09e4c8af72983c7d5e4448946424f89
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.0 MB (44967875 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4997a8a94a1d6d440e27997698f97f5d7342dcb74768525efe222b42ef9fb923`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:26 GMT
ADD file:6dd87346b8be240b21b4f4d9296253bf0d28b6579aa52d2118872e3936963b6b in / 
# Mon, 07 Aug 2023 19:20:26 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 20:30:41 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 09 Aug 2023 01:54:15 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Wed, 09 Aug 2023 01:55:20 GMT
ENV INFLUXDB_VERSION=1.11.1-c1.11.1
# Wed, 09 Aug 2023 01:55:26 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb.conf &&     chmod +x /usr/src/influxdb-*/fs/usr/bin/* &&     cp -a /usr/src/influxdb-*/fs/usr/bin/. /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Wed, 09 Aug 2023 01:55:26 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Wed, 09 Aug 2023 01:55:26 GMT
EXPOSE 8086
# Wed, 09 Aug 2023 01:55:27 GMT
VOLUME [/var/lib/influxdb]
# Wed, 09 Aug 2023 01:55:27 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Wed, 09 Aug 2023 01:55:27 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Wed, 09 Aug 2023 01:55:27 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 09 Aug 2023 01:55:27 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:9398808236ffac29e60c04ec906d8d409af7fa19dc57d8c65ad167e9c4967006`  
		Last Modified: Mon, 07 Aug 2023 19:21:08 GMT  
		Size: 3.4 MB (3378609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bdca2725167af68b5a2e88c072759b23a3bf0e32c8526c7e9b89f616db5a88d`  
		Last Modified: Mon, 07 Aug 2023 20:31:39 GMT  
		Size: 279.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90412949f8cfd74e35fbc8d623c490f3d19ec67abaac2447d3f55007f36a18a1`  
		Last Modified: Wed, 09 Aug 2023 01:56:21 GMT  
		Size: 1.5 MB (1472417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4595e71ccc84641653b90d260127756204fdfea1a54f0a713ca71f01598a2b8`  
		Last Modified: Wed, 09 Aug 2023 01:57:37 GMT  
		Size: 40.1 MB (40114773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ead09dda79ec4a08283520fcbb457330f36bd8a1480baaf61be1e3d2aa6179fd`  
		Last Modified: Wed, 09 Aug 2023 01:57:30 GMT  
		Size: 264.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:849f4b1b089f63a045d817d11f2ca1c6657b523d35e229ad0e04365cd66338e3`  
		Last Modified: Wed, 09 Aug 2023 01:57:30 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab3c8f493dbc4fb1c0665f7b9adb9e83b07f09454da4372b53415cd4d32fec85`  
		Last Modified: Wed, 09 Aug 2023 01:57:30 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.11.1-meta`

```console
$ docker pull influxdb@sha256:12f9a7a51f2d54b959fca4b1266028b3f0a1cef55297d865305586f4da3031a4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.11.1-meta` - linux; amd64

```console
$ docker pull influxdb@sha256:797f251b9263b06a2a73feffc26855da192e0034f791bbe9ae83cfb6121de31b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.1 MB (91068557 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac15bdc40197c186642f8bd0d7f3f377f3a914891fad5cc3034d6644af5a8571`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Wed, 16 Aug 2023 00:59:57 GMT
ADD file:20f89ff93bfbd6c9fb1a97058a1f3de4485a8974e8a83892072c511fbd2e4134 in / 
# Wed, 16 Aug 2023 00:59:58 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 06:59:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Aug 2023 01:50:12 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 17 Aug 2023 01:51:01 GMT
ENV INFLUXDB_VERSION=1.11.1-c1.11.1
# Thu, 17 Aug 2023 01:51:15 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-meta_${INFLUXDB_VERSION}_amd64.deb*
# Thu, 17 Aug 2023 01:51:16 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Thu, 17 Aug 2023 01:51:16 GMT
EXPOSE 8091
# Thu, 17 Aug 2023 01:51:16 GMT
VOLUME [/var/lib/influxdb]
# Thu, 17 Aug 2023 01:51:16 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Thu, 17 Aug 2023 01:51:16 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Aug 2023 01:51:16 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:6a70103cc499a199e10e379794c60aa524d9598587cc2bdfe2995642c2da8df7`  
		Last Modified: Wed, 16 Aug 2023 01:04:50 GMT  
		Size: 55.1 MB (55056621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccb4221e2c63c35bb16b63f6d24c104c7ea5d453997636c2244b66884f540537`  
		Last Modified: Wed, 16 Aug 2023 07:13:46 GMT  
		Size: 15.8 MB (15760534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89b46b2782c35ef5f65808b1b87f49bfe8827c8c03be281c098d7e2f832b617f`  
		Last Modified: Thu, 17 Aug 2023 01:51:49 GMT  
		Size: 1.8 KB (1806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d861715c583388699cfe8fce7754fb95921e9bd9c8688c44463442fb5225ca4`  
		Last Modified: Thu, 17 Aug 2023 01:53:17 GMT  
		Size: 20.2 MB (20249023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0dbfe4340f563fbfe7a01ae6a6e2ea913660c1ad384c77ca3c2dec1ef52e11a`  
		Last Modified: Thu, 17 Aug 2023 01:53:14 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc1938c07a5ee85efffc4b7e71bfb39e945fe67772e69c403ab93c11a044dd12`  
		Last Modified: Thu, 17 Aug 2023 01:53:14 GMT  
		Size: 375.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.11.1-meta-alpine`

```console
$ docker pull influxdb@sha256:953d6274978df9a3280fa1aea7a0c4dae9ccc74b59e4388262c9bd025cafc6d1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.11.1-meta-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:fc5b9e422f6127a618a236c9b387a20651aa77fbb9162f3e8c99921f0e482ee3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.1 MB (25064242 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:74b55a257f61e31f28cac10586355617d61b72c6c79a4f00e813cfab059bca1b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:26 GMT
ADD file:6dd87346b8be240b21b4f4d9296253bf0d28b6579aa52d2118872e3936963b6b in / 
# Mon, 07 Aug 2023 19:20:26 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 20:30:41 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 09 Aug 2023 01:54:15 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Wed, 09 Aug 2023 01:55:20 GMT
ENV INFLUXDB_VERSION=1.11.1-c1.11.1
# Wed, 09 Aug 2023 01:55:37 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb-meta.conf &&     chmod +x /usr/src/influxdb-*/fs/usr/bin/* &&     cp -a /usr/src/influxdb-*/fs/usr/bin/. /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Wed, 09 Aug 2023 01:55:37 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Wed, 09 Aug 2023 01:55:37 GMT
EXPOSE 8091
# Wed, 09 Aug 2023 01:55:37 GMT
VOLUME [/var/lib/influxdb]
# Wed, 09 Aug 2023 01:55:37 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Wed, 09 Aug 2023 01:55:38 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 09 Aug 2023 01:55:38 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:9398808236ffac29e60c04ec906d8d409af7fa19dc57d8c65ad167e9c4967006`  
		Last Modified: Mon, 07 Aug 2023 19:21:08 GMT  
		Size: 3.4 MB (3378609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bdca2725167af68b5a2e88c072759b23a3bf0e32c8526c7e9b89f616db5a88d`  
		Last Modified: Mon, 07 Aug 2023 20:31:39 GMT  
		Size: 279.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90412949f8cfd74e35fbc8d623c490f3d19ec67abaac2447d3f55007f36a18a1`  
		Last Modified: Wed, 09 Aug 2023 01:56:21 GMT  
		Size: 1.5 MB (1472417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04b359de245bd88b2c968ebc3faaee5545903535961cc4174445077b828be50e`  
		Last Modified: Wed, 09 Aug 2023 01:57:49 GMT  
		Size: 20.2 MB (20212341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de0b08635ca3ea71c43f912a8a7fa599881ab95aeda951e261aaabd12c4dac64`  
		Last Modified: Wed, 09 Aug 2023 01:57:46 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0f7d3459e4b0362cd4c64b3b6750f2dbea18a04a270a1c71ed67da55c12c00f`  
		Last Modified: Wed, 09 Aug 2023 01:57:46 GMT  
		Size: 375.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.8`

```console
$ docker pull influxdb@sha256:95150dc455a3f794d8e4bdef4c4a7daf4fb216d1a7ddfe1cb670d91c49490079
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `influxdb:1.8` - linux; amd64

```console
$ docker pull influxdb@sha256:874febee948183f380fce4649a0dcb54110facdd8a363cadeac57a0daaa3c4b6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.7 MB (125706445 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:209f5640465fdf16c575f133385b655b794df99aa57448453b0a5fe8f58d2e83`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 16 Aug 2023 00:59:57 GMT
ADD file:20f89ff93bfbd6c9fb1a97058a1f3de4485a8974e8a83892072c511fbd2e4134 in / 
# Wed, 16 Aug 2023 00:59:58 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 06:59:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Aug 2023 01:50:12 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 17 Aug 2023 01:50:12 GMT
ENV INFLUXDB_VERSION=1.8.10
# Thu, 17 Aug 2023 01:50:16 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Thu, 17 Aug 2023 01:50:17 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Thu, 17 Aug 2023 01:50:17 GMT
EXPOSE 8086
# Thu, 17 Aug 2023 01:50:17 GMT
VOLUME [/var/lib/influxdb]
# Thu, 17 Aug 2023 01:50:17 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Thu, 17 Aug 2023 01:50:17 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Thu, 17 Aug 2023 01:50:17 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Aug 2023 01:50:17 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:6a70103cc499a199e10e379794c60aa524d9598587cc2bdfe2995642c2da8df7`  
		Last Modified: Wed, 16 Aug 2023 01:04:50 GMT  
		Size: 55.1 MB (55056621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccb4221e2c63c35bb16b63f6d24c104c7ea5d453997636c2244b66884f540537`  
		Last Modified: Wed, 16 Aug 2023 07:13:46 GMT  
		Size: 15.8 MB (15760534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89b46b2782c35ef5f65808b1b87f49bfe8827c8c03be281c098d7e2f832b617f`  
		Last Modified: Thu, 17 Aug 2023 01:51:49 GMT  
		Size: 1.8 KB (1806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b63814e3d9dc1231680c5cca700150d972aff2e9efc8e681443db15f3b919884`  
		Last Modified: Thu, 17 Aug 2023 01:51:55 GMT  
		Size: 54.9 MB (54885766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b3151302e3da96ab12cf72b60cdd45b9d02d685430f2f1f7805f28ad70d27ce`  
		Last Modified: Thu, 17 Aug 2023 01:51:49 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a6c60903d2958869e9f968f4cbc1acf4019d0f9e2ee855669a764da1158f667`  
		Last Modified: Thu, 17 Aug 2023 01:51:49 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daa8848b222d1c0c8968249cac91f368ffc54a8529e7f854eb65b8a8f1c9fa31`  
		Last Modified: Thu, 17 Aug 2023 01:51:49 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:1.8` - linux; arm variant v7

```console
$ docker pull influxdb@sha256:1305139001654769f0d108ca56b6364a9ff7ee150d1774284892b3bc8ac0a840
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.7 MB (116704997 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:01caa7cd0e04072cefeb0c96ed265ffe485192faff22d4bc3fe38c653e5adede`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 16 Aug 2023 00:17:21 GMT
ADD file:b529de8b48c1e507ad6f29320c3c5cd83d8d06fa66e8d89bb62faff62700e9f2 in / 
# Wed, 16 Aug 2023 00:17:22 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 05:30:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 23:53:30 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 16 Aug 2023 23:53:30 GMT
ENV INFLUXDB_VERSION=1.8.10
# Wed, 16 Aug 2023 23:53:36 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Wed, 16 Aug 2023 23:53:36 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Wed, 16 Aug 2023 23:53:36 GMT
EXPOSE 8086
# Wed, 16 Aug 2023 23:53:36 GMT
VOLUME [/var/lib/influxdb]
# Wed, 16 Aug 2023 23:53:36 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Wed, 16 Aug 2023 23:53:37 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Wed, 16 Aug 2023 23:53:37 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 16 Aug 2023 23:53:37 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:c53151c23650f086e15d3652b8a931fb4623765c0112e8adc74eb8853c8c9232`  
		Last Modified: Wed, 16 Aug 2023 00:21:46 GMT  
		Size: 50.2 MB (50219496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abbe9a81a850f9760477ffa3083b63d636090316a05f81146ffd62a60638926a`  
		Last Modified: Wed, 16 Aug 2023 05:48:44 GMT  
		Size: 14.9 MB (14868833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a699f70c555443c8ca27c61c24e69278bce270f3fff164e33952e5d0faed1f3`  
		Last Modified: Wed, 16 Aug 2023 23:53:44 GMT  
		Size: 1.8 KB (1815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a850778c634cdedccb69146597185f700edea36c766aa98e0a4ae964b313e9f4`  
		Last Modified: Wed, 16 Aug 2023 23:53:50 GMT  
		Size: 51.6 MB (51613138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b86e25f3dac10abb365d12a9f52ec872c2dd267c27973fe7ab17685ed09b444`  
		Last Modified: Wed, 16 Aug 2023 23:53:44 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74bb233eb2ab3ea0ad082ad01107880dfd8f026fc01b77430174c7595d133b68`  
		Last Modified: Wed, 16 Aug 2023 23:53:44 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35e3a83022048aefb8d842ae47c28ab8d27dcedf0bc63f7022e7a6301e422755`  
		Last Modified: Wed, 16 Aug 2023 23:53:44 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:1.8` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:584ab0b8a000f4373c15323c578ba3647054dbab5c0fd92927dc8a375695dace
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.7 MB (120684942 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48de5106000a72d512438fdf3a228295510ea1e7181b0c5c12104af1215f5ad8`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Thu, 07 Sep 2023 00:39:45 GMT
ADD file:6bc001e951ef1280f566a92e65fcff57aefb8a280aa3510b7cd4b4e0a54c5cff in / 
# Thu, 07 Sep 2023 00:39:46 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 06:52:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 11:19:10 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 07 Sep 2023 11:19:10 GMT
ENV INFLUXDB_VERSION=1.8.10
# Thu, 07 Sep 2023 11:19:14 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Thu, 07 Sep 2023 11:19:14 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Thu, 07 Sep 2023 11:19:14 GMT
EXPOSE 8086
# Thu, 07 Sep 2023 11:19:14 GMT
VOLUME [/var/lib/influxdb]
# Thu, 07 Sep 2023 11:19:14 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Thu, 07 Sep 2023 11:19:14 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Thu, 07 Sep 2023 11:19:15 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 07 Sep 2023 11:19:15 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:61c16b7975697b00760ff9536c09eed29b6a76923d4d98be38e9cdc749506417`  
		Last Modified: Thu, 07 Sep 2023 00:43:21 GMT  
		Size: 53.7 MB (53704716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07b3f92a99188e47f7b0b8d38aff11fd0ad90510e0d26506aec007d24fe539b6`  
		Last Modified: Thu, 07 Sep 2023 07:00:19 GMT  
		Size: 15.7 MB (15746623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86a1058b124bfc5691310ba8bebc4a6a722738cac7271a6842486950d9b9e1cd`  
		Last Modified: Thu, 07 Sep 2023 11:19:27 GMT  
		Size: 1.8 KB (1814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e4031ae85f5aab6853a837646384972525a3d4bf457d3849e5391d65ce46d9e`  
		Last Modified: Thu, 07 Sep 2023 11:19:32 GMT  
		Size: 51.2 MB (51230072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ca676fbddf21c566f3f17feac896781502a2311bc6dc91eb7639b5e5bb92871`  
		Last Modified: Thu, 07 Sep 2023 11:19:27 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:797d448641d313380afb1ac2d335cf338845a385f640d6f6a8f551e499b7c5cd`  
		Last Modified: Thu, 07 Sep 2023 11:19:27 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dff151cfd100174cee30417716601835d537b35b9535221c76df5c9bfdfe42c4`  
		Last Modified: Thu, 07 Sep 2023 11:19:27 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.8-alpine`

```console
$ docker pull influxdb@sha256:beb60ab73eb378f4ca4eed75c42d33c41ac5949a9c06855dd48cdbc3501aac00
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.8-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:42537eee368080ff9273aba4abcb7bfb860564a2331a06db260b1b65a1e9401a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.5 MB (59499656 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ab4fc5517d79ab1b762d452379d20003829754275f8108323d64245ecf27c54`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:26 GMT
ADD file:6dd87346b8be240b21b4f4d9296253bf0d28b6579aa52d2118872e3936963b6b in / 
# Mon, 07 Aug 2023 19:20:26 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 20:30:41 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 09 Aug 2023 01:54:15 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Wed, 09 Aug 2023 01:54:15 GMT
ENV INFLUXDB_VERSION=1.8.10
# Wed, 09 Aug 2023 01:54:23 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     chmod +x /usr/src/influxdb-*/influx              /usr/src/influxdb-*/influx_inspect              /usr/src/influxdb-*/influx_stress              /usr/src/influxdb-*/influxd &&    mv /usr/src/influxdb-*/influx        /usr/src/influxdb-*/influx_inspect        /usr/src/influxdb-*/influx_stress         /usr/src/influxdb-*/influxd        /usr/bin/ &&    gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Wed, 09 Aug 2023 01:54:24 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Wed, 09 Aug 2023 01:54:24 GMT
EXPOSE 8086
# Wed, 09 Aug 2023 01:54:24 GMT
VOLUME [/var/lib/influxdb]
# Wed, 09 Aug 2023 01:54:24 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Wed, 09 Aug 2023 01:54:24 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Wed, 09 Aug 2023 01:54:24 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 09 Aug 2023 01:54:24 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:9398808236ffac29e60c04ec906d8d409af7fa19dc57d8c65ad167e9c4967006`  
		Last Modified: Mon, 07 Aug 2023 19:21:08 GMT  
		Size: 3.4 MB (3378609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bdca2725167af68b5a2e88c072759b23a3bf0e32c8526c7e9b89f616db5a88d`  
		Last Modified: Mon, 07 Aug 2023 20:31:39 GMT  
		Size: 279.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90412949f8cfd74e35fbc8d623c490f3d19ec67abaac2447d3f55007f36a18a1`  
		Last Modified: Wed, 09 Aug 2023 01:56:21 GMT  
		Size: 1.5 MB (1472417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b3ee6940f19b79ffbb97495e04af9f011832edecf8aced034c48e6d77be2cbe`  
		Last Modified: Wed, 09 Aug 2023 01:56:28 GMT  
		Size: 54.6 MB (54646612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a6c289e9975009f2cedf31d0f41faa6e781935e01b092a27aed5840c47d916b`  
		Last Modified: Wed, 09 Aug 2023 01:56:21 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10e6ad59e302d04be331ef8a5fbf491f0f94666bc5de9f9630ecc8e363460d84`  
		Last Modified: Wed, 09 Aug 2023 01:56:21 GMT  
		Size: 208.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18948c75666c74a8a006542797764bbd66c686e06b5ef32a9a0fc091fe0e1ada`  
		Last Modified: Wed, 09 Aug 2023 01:56:21 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.8.10`

```console
$ docker pull influxdb@sha256:95150dc455a3f794d8e4bdef4c4a7daf4fb216d1a7ddfe1cb670d91c49490079
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `influxdb:1.8.10` - linux; amd64

```console
$ docker pull influxdb@sha256:874febee948183f380fce4649a0dcb54110facdd8a363cadeac57a0daaa3c4b6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.7 MB (125706445 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:209f5640465fdf16c575f133385b655b794df99aa57448453b0a5fe8f58d2e83`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 16 Aug 2023 00:59:57 GMT
ADD file:20f89ff93bfbd6c9fb1a97058a1f3de4485a8974e8a83892072c511fbd2e4134 in / 
# Wed, 16 Aug 2023 00:59:58 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 06:59:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Aug 2023 01:50:12 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 17 Aug 2023 01:50:12 GMT
ENV INFLUXDB_VERSION=1.8.10
# Thu, 17 Aug 2023 01:50:16 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Thu, 17 Aug 2023 01:50:17 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Thu, 17 Aug 2023 01:50:17 GMT
EXPOSE 8086
# Thu, 17 Aug 2023 01:50:17 GMT
VOLUME [/var/lib/influxdb]
# Thu, 17 Aug 2023 01:50:17 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Thu, 17 Aug 2023 01:50:17 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Thu, 17 Aug 2023 01:50:17 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Aug 2023 01:50:17 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:6a70103cc499a199e10e379794c60aa524d9598587cc2bdfe2995642c2da8df7`  
		Last Modified: Wed, 16 Aug 2023 01:04:50 GMT  
		Size: 55.1 MB (55056621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccb4221e2c63c35bb16b63f6d24c104c7ea5d453997636c2244b66884f540537`  
		Last Modified: Wed, 16 Aug 2023 07:13:46 GMT  
		Size: 15.8 MB (15760534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89b46b2782c35ef5f65808b1b87f49bfe8827c8c03be281c098d7e2f832b617f`  
		Last Modified: Thu, 17 Aug 2023 01:51:49 GMT  
		Size: 1.8 KB (1806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b63814e3d9dc1231680c5cca700150d972aff2e9efc8e681443db15f3b919884`  
		Last Modified: Thu, 17 Aug 2023 01:51:55 GMT  
		Size: 54.9 MB (54885766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b3151302e3da96ab12cf72b60cdd45b9d02d685430f2f1f7805f28ad70d27ce`  
		Last Modified: Thu, 17 Aug 2023 01:51:49 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a6c60903d2958869e9f968f4cbc1acf4019d0f9e2ee855669a764da1158f667`  
		Last Modified: Thu, 17 Aug 2023 01:51:49 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daa8848b222d1c0c8968249cac91f368ffc54a8529e7f854eb65b8a8f1c9fa31`  
		Last Modified: Thu, 17 Aug 2023 01:51:49 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:1.8.10` - linux; arm variant v7

```console
$ docker pull influxdb@sha256:1305139001654769f0d108ca56b6364a9ff7ee150d1774284892b3bc8ac0a840
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.7 MB (116704997 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:01caa7cd0e04072cefeb0c96ed265ffe485192faff22d4bc3fe38c653e5adede`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 16 Aug 2023 00:17:21 GMT
ADD file:b529de8b48c1e507ad6f29320c3c5cd83d8d06fa66e8d89bb62faff62700e9f2 in / 
# Wed, 16 Aug 2023 00:17:22 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 05:30:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 23:53:30 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 16 Aug 2023 23:53:30 GMT
ENV INFLUXDB_VERSION=1.8.10
# Wed, 16 Aug 2023 23:53:36 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Wed, 16 Aug 2023 23:53:36 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Wed, 16 Aug 2023 23:53:36 GMT
EXPOSE 8086
# Wed, 16 Aug 2023 23:53:36 GMT
VOLUME [/var/lib/influxdb]
# Wed, 16 Aug 2023 23:53:36 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Wed, 16 Aug 2023 23:53:37 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Wed, 16 Aug 2023 23:53:37 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 16 Aug 2023 23:53:37 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:c53151c23650f086e15d3652b8a931fb4623765c0112e8adc74eb8853c8c9232`  
		Last Modified: Wed, 16 Aug 2023 00:21:46 GMT  
		Size: 50.2 MB (50219496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abbe9a81a850f9760477ffa3083b63d636090316a05f81146ffd62a60638926a`  
		Last Modified: Wed, 16 Aug 2023 05:48:44 GMT  
		Size: 14.9 MB (14868833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a699f70c555443c8ca27c61c24e69278bce270f3fff164e33952e5d0faed1f3`  
		Last Modified: Wed, 16 Aug 2023 23:53:44 GMT  
		Size: 1.8 KB (1815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a850778c634cdedccb69146597185f700edea36c766aa98e0a4ae964b313e9f4`  
		Last Modified: Wed, 16 Aug 2023 23:53:50 GMT  
		Size: 51.6 MB (51613138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b86e25f3dac10abb365d12a9f52ec872c2dd267c27973fe7ab17685ed09b444`  
		Last Modified: Wed, 16 Aug 2023 23:53:44 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74bb233eb2ab3ea0ad082ad01107880dfd8f026fc01b77430174c7595d133b68`  
		Last Modified: Wed, 16 Aug 2023 23:53:44 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35e3a83022048aefb8d842ae47c28ab8d27dcedf0bc63f7022e7a6301e422755`  
		Last Modified: Wed, 16 Aug 2023 23:53:44 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:1.8.10` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:584ab0b8a000f4373c15323c578ba3647054dbab5c0fd92927dc8a375695dace
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.7 MB (120684942 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48de5106000a72d512438fdf3a228295510ea1e7181b0c5c12104af1215f5ad8`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Thu, 07 Sep 2023 00:39:45 GMT
ADD file:6bc001e951ef1280f566a92e65fcff57aefb8a280aa3510b7cd4b4e0a54c5cff in / 
# Thu, 07 Sep 2023 00:39:46 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 06:52:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 11:19:10 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 07 Sep 2023 11:19:10 GMT
ENV INFLUXDB_VERSION=1.8.10
# Thu, 07 Sep 2023 11:19:14 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Thu, 07 Sep 2023 11:19:14 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Thu, 07 Sep 2023 11:19:14 GMT
EXPOSE 8086
# Thu, 07 Sep 2023 11:19:14 GMT
VOLUME [/var/lib/influxdb]
# Thu, 07 Sep 2023 11:19:14 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Thu, 07 Sep 2023 11:19:14 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Thu, 07 Sep 2023 11:19:15 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 07 Sep 2023 11:19:15 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:61c16b7975697b00760ff9536c09eed29b6a76923d4d98be38e9cdc749506417`  
		Last Modified: Thu, 07 Sep 2023 00:43:21 GMT  
		Size: 53.7 MB (53704716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07b3f92a99188e47f7b0b8d38aff11fd0ad90510e0d26506aec007d24fe539b6`  
		Last Modified: Thu, 07 Sep 2023 07:00:19 GMT  
		Size: 15.7 MB (15746623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86a1058b124bfc5691310ba8bebc4a6a722738cac7271a6842486950d9b9e1cd`  
		Last Modified: Thu, 07 Sep 2023 11:19:27 GMT  
		Size: 1.8 KB (1814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e4031ae85f5aab6853a837646384972525a3d4bf457d3849e5391d65ce46d9e`  
		Last Modified: Thu, 07 Sep 2023 11:19:32 GMT  
		Size: 51.2 MB (51230072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ca676fbddf21c566f3f17feac896781502a2311bc6dc91eb7639b5e5bb92871`  
		Last Modified: Thu, 07 Sep 2023 11:19:27 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:797d448641d313380afb1ac2d335cf338845a385f640d6f6a8f551e499b7c5cd`  
		Last Modified: Thu, 07 Sep 2023 11:19:27 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dff151cfd100174cee30417716601835d537b35b9535221c76df5c9bfdfe42c4`  
		Last Modified: Thu, 07 Sep 2023 11:19:27 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.8.10-alpine`

```console
$ docker pull influxdb@sha256:beb60ab73eb378f4ca4eed75c42d33c41ac5949a9c06855dd48cdbc3501aac00
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.8.10-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:42537eee368080ff9273aba4abcb7bfb860564a2331a06db260b1b65a1e9401a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.5 MB (59499656 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ab4fc5517d79ab1b762d452379d20003829754275f8108323d64245ecf27c54`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:26 GMT
ADD file:6dd87346b8be240b21b4f4d9296253bf0d28b6579aa52d2118872e3936963b6b in / 
# Mon, 07 Aug 2023 19:20:26 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 20:30:41 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 09 Aug 2023 01:54:15 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Wed, 09 Aug 2023 01:54:15 GMT
ENV INFLUXDB_VERSION=1.8.10
# Wed, 09 Aug 2023 01:54:23 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     chmod +x /usr/src/influxdb-*/influx              /usr/src/influxdb-*/influx_inspect              /usr/src/influxdb-*/influx_stress              /usr/src/influxdb-*/influxd &&    mv /usr/src/influxdb-*/influx        /usr/src/influxdb-*/influx_inspect        /usr/src/influxdb-*/influx_stress         /usr/src/influxdb-*/influxd        /usr/bin/ &&    gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Wed, 09 Aug 2023 01:54:24 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Wed, 09 Aug 2023 01:54:24 GMT
EXPOSE 8086
# Wed, 09 Aug 2023 01:54:24 GMT
VOLUME [/var/lib/influxdb]
# Wed, 09 Aug 2023 01:54:24 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Wed, 09 Aug 2023 01:54:24 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Wed, 09 Aug 2023 01:54:24 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 09 Aug 2023 01:54:24 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:9398808236ffac29e60c04ec906d8d409af7fa19dc57d8c65ad167e9c4967006`  
		Last Modified: Mon, 07 Aug 2023 19:21:08 GMT  
		Size: 3.4 MB (3378609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bdca2725167af68b5a2e88c072759b23a3bf0e32c8526c7e9b89f616db5a88d`  
		Last Modified: Mon, 07 Aug 2023 20:31:39 GMT  
		Size: 279.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90412949f8cfd74e35fbc8d623c490f3d19ec67abaac2447d3f55007f36a18a1`  
		Last Modified: Wed, 09 Aug 2023 01:56:21 GMT  
		Size: 1.5 MB (1472417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b3ee6940f19b79ffbb97495e04af9f011832edecf8aced034c48e6d77be2cbe`  
		Last Modified: Wed, 09 Aug 2023 01:56:28 GMT  
		Size: 54.6 MB (54646612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a6c289e9975009f2cedf31d0f41faa6e781935e01b092a27aed5840c47d916b`  
		Last Modified: Wed, 09 Aug 2023 01:56:21 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10e6ad59e302d04be331ef8a5fbf491f0f94666bc5de9f9630ecc8e363460d84`  
		Last Modified: Wed, 09 Aug 2023 01:56:21 GMT  
		Size: 208.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18948c75666c74a8a006542797764bbd66c686e06b5ef32a9a0fc091fe0e1ada`  
		Last Modified: Wed, 09 Aug 2023 01:56:21 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.9-data`

```console
$ docker pull influxdb@sha256:f6381cbffec45c1c595080f2549c19d9ce19e8803f847bde7f1c8f264c61d9cf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.9-data` - linux; amd64

```console
$ docker pull influxdb@sha256:df18c30a717f04d6b50114d770b3edfeef63c053bbd3db420225912effc598eb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.0 MB (103996587 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:adea9bbbffbbe3af1627378c687e10e7ef2a20902bdf8fd7b2456b575f93f4a6`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 16 Aug 2023 00:59:57 GMT
ADD file:20f89ff93bfbd6c9fb1a97058a1f3de4485a8974e8a83892072c511fbd2e4134 in / 
# Wed, 16 Aug 2023 00:59:58 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 06:59:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Aug 2023 01:50:12 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 17 Aug 2023 01:50:23 GMT
ENV INFLUXDB_VERSION=1.9.12-c1.9.12
# Thu, 17 Aug 2023 01:50:27 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-data_${INFLUXDB_VERSION}_amd64.deb*
# Thu, 17 Aug 2023 01:50:27 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Thu, 17 Aug 2023 01:50:27 GMT
EXPOSE 8086
# Thu, 17 Aug 2023 01:50:27 GMT
VOLUME [/var/lib/influxdb]
# Thu, 17 Aug 2023 01:50:28 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Thu, 17 Aug 2023 01:50:28 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Thu, 17 Aug 2023 01:50:28 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Aug 2023 01:50:28 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:6a70103cc499a199e10e379794c60aa524d9598587cc2bdfe2995642c2da8df7`  
		Last Modified: Wed, 16 Aug 2023 01:04:50 GMT  
		Size: 55.1 MB (55056621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccb4221e2c63c35bb16b63f6d24c104c7ea5d453997636c2244b66884f540537`  
		Last Modified: Wed, 16 Aug 2023 07:13:46 GMT  
		Size: 15.8 MB (15760534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89b46b2782c35ef5f65808b1b87f49bfe8827c8c03be281c098d7e2f832b617f`  
		Last Modified: Thu, 17 Aug 2023 01:51:49 GMT  
		Size: 1.8 KB (1806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a431c5a1d0f25850e3e114b09ad2de74f2438ca5469dd202cc1c9e5a903328fb`  
		Last Modified: Thu, 17 Aug 2023 01:52:10 GMT  
		Size: 33.2 MB (33175851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b46a892579d2f23717d07e15004211b7f2d63c8bb593c252c102799f799bf58`  
		Last Modified: Thu, 17 Aug 2023 01:52:05 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:312a47dfa5de4d5f0b2deb771f2bb4458c54a5114a3130b0162b83b38c812962`  
		Last Modified: Thu, 17 Aug 2023 01:52:05 GMT  
		Size: 252.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17688447cbd5184e671e7235990e7cf3f9f5a2132c59c7f07282b35a21c4788b`  
		Last Modified: Thu, 17 Aug 2023 01:52:06 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.9-data-alpine`

```console
$ docker pull influxdb@sha256:b02755b0d2f4c0bcca2cfced14fa6333dbe97a47d79020d2ae56113f3b74581d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.9-data-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:1a36205e66928922652b45af980fae69f7806122888fdf2fd3a0e7de536012f8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.0 MB (37987801 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:51599114496c9227d6c38bb9630632071c9a62e223a2e7d580df048e42db26f1`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:26 GMT
ADD file:6dd87346b8be240b21b4f4d9296253bf0d28b6579aa52d2118872e3936963b6b in / 
# Mon, 07 Aug 2023 19:20:26 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 20:30:41 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 09 Aug 2023 01:54:15 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Wed, 09 Aug 2023 01:54:30 GMT
ENV INFLUXDB_VERSION=1.9.12-c1.9.12
# Wed, 09 Aug 2023 01:54:37 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/etc/influxdb/influxdb.conf &&     chmod +x /usr/src/influxdb-*/usr/bin/* &&     cp -a /usr/src/influxdb-*/usr/bin/. /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Wed, 09 Aug 2023 01:54:37 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Wed, 09 Aug 2023 01:54:37 GMT
EXPOSE 8086
# Wed, 09 Aug 2023 01:54:37 GMT
VOLUME [/var/lib/influxdb]
# Wed, 09 Aug 2023 01:54:37 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Wed, 09 Aug 2023 01:54:38 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Wed, 09 Aug 2023 01:54:38 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 09 Aug 2023 01:54:38 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:9398808236ffac29e60c04ec906d8d409af7fa19dc57d8c65ad167e9c4967006`  
		Last Modified: Mon, 07 Aug 2023 19:21:08 GMT  
		Size: 3.4 MB (3378609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bdca2725167af68b5a2e88c072759b23a3bf0e32c8526c7e9b89f616db5a88d`  
		Last Modified: Mon, 07 Aug 2023 20:31:39 GMT  
		Size: 279.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90412949f8cfd74e35fbc8d623c490f3d19ec67abaac2447d3f55007f36a18a1`  
		Last Modified: Wed, 09 Aug 2023 01:56:21 GMT  
		Size: 1.5 MB (1472417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:984b0874086211cd6a4c728b73fcaade388bb5402b089b4fe1c23ea96fdd626f`  
		Last Modified: Wed, 09 Aug 2023 01:56:42 GMT  
		Size: 33.1 MB (33134698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:631323286c70a56626754f45aa992947dd9a2cfdf08fefe6033feeeeac89cee6`  
		Last Modified: Wed, 09 Aug 2023 01:56:37 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8958954bc4803539b1b98e529c2804c6259545809050d90673e440a5d3f2a211`  
		Last Modified: Wed, 09 Aug 2023 01:56:37 GMT  
		Size: 252.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32e28a11b9675a5a7f1a6ed568b4cb13d0b7c503446e0444a346d60726c2a05d`  
		Last Modified: Wed, 09 Aug 2023 01:56:37 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.9-meta`

```console
$ docker pull influxdb@sha256:804ddec2f996c2588869e15b1ee9a10a5b5a797bcdb023a520b43e8b49e54f6f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.9-meta` - linux; amd64

```console
$ docker pull influxdb@sha256:8a5b87a5bdb29f551304093bda360181f1abc899c917f195c6e87ca5801838a3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.4 MB (83437017 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cc0a8c98661fc25c98a84b90f8977135812ed4d46a5a9c973cec4846a5f91469`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Wed, 16 Aug 2023 00:59:57 GMT
ADD file:20f89ff93bfbd6c9fb1a97058a1f3de4485a8974e8a83892072c511fbd2e4134 in / 
# Wed, 16 Aug 2023 00:59:58 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 06:59:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Aug 2023 01:50:12 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 17 Aug 2023 01:50:23 GMT
ENV INFLUXDB_VERSION=1.9.12-c1.9.12
# Thu, 17 Aug 2023 01:50:35 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-meta_${INFLUXDB_VERSION}_amd64.deb*
# Thu, 17 Aug 2023 01:50:36 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Thu, 17 Aug 2023 01:50:36 GMT
EXPOSE 8091
# Thu, 17 Aug 2023 01:50:36 GMT
VOLUME [/var/lib/influxdb]
# Thu, 17 Aug 2023 01:50:36 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Thu, 17 Aug 2023 01:50:36 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Aug 2023 01:50:36 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:6a70103cc499a199e10e379794c60aa524d9598587cc2bdfe2995642c2da8df7`  
		Last Modified: Wed, 16 Aug 2023 01:04:50 GMT  
		Size: 55.1 MB (55056621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccb4221e2c63c35bb16b63f6d24c104c7ea5d453997636c2244b66884f540537`  
		Last Modified: Wed, 16 Aug 2023 07:13:46 GMT  
		Size: 15.8 MB (15760534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89b46b2782c35ef5f65808b1b87f49bfe8827c8c03be281c098d7e2f832b617f`  
		Last Modified: Thu, 17 Aug 2023 01:51:49 GMT  
		Size: 1.8 KB (1806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcde8a16f77d22937a3d7d72f5683dadfd6cdebe88725ec344d01e6e8baa7a30`  
		Last Modified: Thu, 17 Aug 2023 01:52:21 GMT  
		Size: 12.6 MB (12617488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f26d9a2d2c000c0b9a4ef629e4f9f3f24dfb77af671a3534a1c3bb5ce5ce9282`  
		Last Modified: Thu, 17 Aug 2023 01:52:20 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e8f5bd3827a6cc1687356c90d42ff12cfb28638845288a9a9fef1ffff9ad745`  
		Last Modified: Thu, 17 Aug 2023 01:52:19 GMT  
		Size: 375.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.9-meta-alpine`

```console
$ docker pull influxdb@sha256:3a3fc5fcb76f0dc7cd8c45a81a353785f3d16c0cd0312a8da8f17e028fd4bbaa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.9-meta-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:6236faaa93f504f1f9d4e1eabccc637f19cea95dfb3551ffd9d890341e6897b4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.4 MB (17433663 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e014f8c8dd5143533c2d241216b39fab7c413eeaeba5192b638ce24d46c1c96f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:26 GMT
ADD file:6dd87346b8be240b21b4f4d9296253bf0d28b6579aa52d2118872e3936963b6b in / 
# Mon, 07 Aug 2023 19:20:26 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 20:30:41 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 09 Aug 2023 01:54:15 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Wed, 09 Aug 2023 01:54:30 GMT
ENV INFLUXDB_VERSION=1.9.12-c1.9.12
# Wed, 09 Aug 2023 01:54:48 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/etc/influxdb/influxdb-meta.conf &&     chmod +x /usr/src/influxdb-*/usr/bin/* &&     cp -a /usr/src/influxdb-*/usr/bin/. /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Wed, 09 Aug 2023 01:54:48 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Wed, 09 Aug 2023 01:54:48 GMT
EXPOSE 8091
# Wed, 09 Aug 2023 01:54:48 GMT
VOLUME [/var/lib/influxdb]
# Wed, 09 Aug 2023 01:54:48 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Wed, 09 Aug 2023 01:54:48 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 09 Aug 2023 01:54:48 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:9398808236ffac29e60c04ec906d8d409af7fa19dc57d8c65ad167e9c4967006`  
		Last Modified: Mon, 07 Aug 2023 19:21:08 GMT  
		Size: 3.4 MB (3378609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bdca2725167af68b5a2e88c072759b23a3bf0e32c8526c7e9b89f616db5a88d`  
		Last Modified: Mon, 07 Aug 2023 20:31:39 GMT  
		Size: 279.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90412949f8cfd74e35fbc8d623c490f3d19ec67abaac2447d3f55007f36a18a1`  
		Last Modified: Wed, 09 Aug 2023 01:56:21 GMT  
		Size: 1.5 MB (1472417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:617f4e7c957e2e9f40805d4ffbdb1e0d5720329ca768d5323d4c1bfaa759cb8a`  
		Last Modified: Wed, 09 Aug 2023 01:56:53 GMT  
		Size: 12.6 MB (12581763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e80ee0272fb9aac850a9c2ef72a44f063ec1f8c66518dd2d5aab1d714ba1a9eb`  
		Last Modified: Wed, 09 Aug 2023 01:56:51 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:895dc0a2527c7ea6aa44324b28c00248e69a2fdb0a9c64c47cebb2a3f90271a1`  
		Last Modified: Wed, 09 Aug 2023 01:56:51 GMT  
		Size: 375.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.9.12-data`

```console
$ docker pull influxdb@sha256:f6381cbffec45c1c595080f2549c19d9ce19e8803f847bde7f1c8f264c61d9cf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.9.12-data` - linux; amd64

```console
$ docker pull influxdb@sha256:df18c30a717f04d6b50114d770b3edfeef63c053bbd3db420225912effc598eb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.0 MB (103996587 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:adea9bbbffbbe3af1627378c687e10e7ef2a20902bdf8fd7b2456b575f93f4a6`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 16 Aug 2023 00:59:57 GMT
ADD file:20f89ff93bfbd6c9fb1a97058a1f3de4485a8974e8a83892072c511fbd2e4134 in / 
# Wed, 16 Aug 2023 00:59:58 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 06:59:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Aug 2023 01:50:12 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 17 Aug 2023 01:50:23 GMT
ENV INFLUXDB_VERSION=1.9.12-c1.9.12
# Thu, 17 Aug 2023 01:50:27 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-data_${INFLUXDB_VERSION}_amd64.deb*
# Thu, 17 Aug 2023 01:50:27 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Thu, 17 Aug 2023 01:50:27 GMT
EXPOSE 8086
# Thu, 17 Aug 2023 01:50:27 GMT
VOLUME [/var/lib/influxdb]
# Thu, 17 Aug 2023 01:50:28 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Thu, 17 Aug 2023 01:50:28 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Thu, 17 Aug 2023 01:50:28 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Aug 2023 01:50:28 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:6a70103cc499a199e10e379794c60aa524d9598587cc2bdfe2995642c2da8df7`  
		Last Modified: Wed, 16 Aug 2023 01:04:50 GMT  
		Size: 55.1 MB (55056621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccb4221e2c63c35bb16b63f6d24c104c7ea5d453997636c2244b66884f540537`  
		Last Modified: Wed, 16 Aug 2023 07:13:46 GMT  
		Size: 15.8 MB (15760534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89b46b2782c35ef5f65808b1b87f49bfe8827c8c03be281c098d7e2f832b617f`  
		Last Modified: Thu, 17 Aug 2023 01:51:49 GMT  
		Size: 1.8 KB (1806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a431c5a1d0f25850e3e114b09ad2de74f2438ca5469dd202cc1c9e5a903328fb`  
		Last Modified: Thu, 17 Aug 2023 01:52:10 GMT  
		Size: 33.2 MB (33175851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b46a892579d2f23717d07e15004211b7f2d63c8bb593c252c102799f799bf58`  
		Last Modified: Thu, 17 Aug 2023 01:52:05 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:312a47dfa5de4d5f0b2deb771f2bb4458c54a5114a3130b0162b83b38c812962`  
		Last Modified: Thu, 17 Aug 2023 01:52:05 GMT  
		Size: 252.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17688447cbd5184e671e7235990e7cf3f9f5a2132c59c7f07282b35a21c4788b`  
		Last Modified: Thu, 17 Aug 2023 01:52:06 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.9.12-data-alpine`

```console
$ docker pull influxdb@sha256:b02755b0d2f4c0bcca2cfced14fa6333dbe97a47d79020d2ae56113f3b74581d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.9.12-data-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:1a36205e66928922652b45af980fae69f7806122888fdf2fd3a0e7de536012f8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.0 MB (37987801 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:51599114496c9227d6c38bb9630632071c9a62e223a2e7d580df048e42db26f1`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:26 GMT
ADD file:6dd87346b8be240b21b4f4d9296253bf0d28b6579aa52d2118872e3936963b6b in / 
# Mon, 07 Aug 2023 19:20:26 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 20:30:41 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 09 Aug 2023 01:54:15 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Wed, 09 Aug 2023 01:54:30 GMT
ENV INFLUXDB_VERSION=1.9.12-c1.9.12
# Wed, 09 Aug 2023 01:54:37 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/etc/influxdb/influxdb.conf &&     chmod +x /usr/src/influxdb-*/usr/bin/* &&     cp -a /usr/src/influxdb-*/usr/bin/. /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Wed, 09 Aug 2023 01:54:37 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Wed, 09 Aug 2023 01:54:37 GMT
EXPOSE 8086
# Wed, 09 Aug 2023 01:54:37 GMT
VOLUME [/var/lib/influxdb]
# Wed, 09 Aug 2023 01:54:37 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Wed, 09 Aug 2023 01:54:38 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Wed, 09 Aug 2023 01:54:38 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 09 Aug 2023 01:54:38 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:9398808236ffac29e60c04ec906d8d409af7fa19dc57d8c65ad167e9c4967006`  
		Last Modified: Mon, 07 Aug 2023 19:21:08 GMT  
		Size: 3.4 MB (3378609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bdca2725167af68b5a2e88c072759b23a3bf0e32c8526c7e9b89f616db5a88d`  
		Last Modified: Mon, 07 Aug 2023 20:31:39 GMT  
		Size: 279.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90412949f8cfd74e35fbc8d623c490f3d19ec67abaac2447d3f55007f36a18a1`  
		Last Modified: Wed, 09 Aug 2023 01:56:21 GMT  
		Size: 1.5 MB (1472417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:984b0874086211cd6a4c728b73fcaade388bb5402b089b4fe1c23ea96fdd626f`  
		Last Modified: Wed, 09 Aug 2023 01:56:42 GMT  
		Size: 33.1 MB (33134698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:631323286c70a56626754f45aa992947dd9a2cfdf08fefe6033feeeeac89cee6`  
		Last Modified: Wed, 09 Aug 2023 01:56:37 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8958954bc4803539b1b98e529c2804c6259545809050d90673e440a5d3f2a211`  
		Last Modified: Wed, 09 Aug 2023 01:56:37 GMT  
		Size: 252.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32e28a11b9675a5a7f1a6ed568b4cb13d0b7c503446e0444a346d60726c2a05d`  
		Last Modified: Wed, 09 Aug 2023 01:56:37 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.9.12-meta`

```console
$ docker pull influxdb@sha256:804ddec2f996c2588869e15b1ee9a10a5b5a797bcdb023a520b43e8b49e54f6f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.9.12-meta` - linux; amd64

```console
$ docker pull influxdb@sha256:8a5b87a5bdb29f551304093bda360181f1abc899c917f195c6e87ca5801838a3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.4 MB (83437017 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cc0a8c98661fc25c98a84b90f8977135812ed4d46a5a9c973cec4846a5f91469`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Wed, 16 Aug 2023 00:59:57 GMT
ADD file:20f89ff93bfbd6c9fb1a97058a1f3de4485a8974e8a83892072c511fbd2e4134 in / 
# Wed, 16 Aug 2023 00:59:58 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 06:59:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Aug 2023 01:50:12 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 17 Aug 2023 01:50:23 GMT
ENV INFLUXDB_VERSION=1.9.12-c1.9.12
# Thu, 17 Aug 2023 01:50:35 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-meta_${INFLUXDB_VERSION}_amd64.deb*
# Thu, 17 Aug 2023 01:50:36 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Thu, 17 Aug 2023 01:50:36 GMT
EXPOSE 8091
# Thu, 17 Aug 2023 01:50:36 GMT
VOLUME [/var/lib/influxdb]
# Thu, 17 Aug 2023 01:50:36 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Thu, 17 Aug 2023 01:50:36 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Aug 2023 01:50:36 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:6a70103cc499a199e10e379794c60aa524d9598587cc2bdfe2995642c2da8df7`  
		Last Modified: Wed, 16 Aug 2023 01:04:50 GMT  
		Size: 55.1 MB (55056621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccb4221e2c63c35bb16b63f6d24c104c7ea5d453997636c2244b66884f540537`  
		Last Modified: Wed, 16 Aug 2023 07:13:46 GMT  
		Size: 15.8 MB (15760534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89b46b2782c35ef5f65808b1b87f49bfe8827c8c03be281c098d7e2f832b617f`  
		Last Modified: Thu, 17 Aug 2023 01:51:49 GMT  
		Size: 1.8 KB (1806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcde8a16f77d22937a3d7d72f5683dadfd6cdebe88725ec344d01e6e8baa7a30`  
		Last Modified: Thu, 17 Aug 2023 01:52:21 GMT  
		Size: 12.6 MB (12617488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f26d9a2d2c000c0b9a4ef629e4f9f3f24dfb77af671a3534a1c3bb5ce5ce9282`  
		Last Modified: Thu, 17 Aug 2023 01:52:20 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e8f5bd3827a6cc1687356c90d42ff12cfb28638845288a9a9fef1ffff9ad745`  
		Last Modified: Thu, 17 Aug 2023 01:52:19 GMT  
		Size: 375.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.9.12-meta-alpine`

```console
$ docker pull influxdb@sha256:3a3fc5fcb76f0dc7cd8c45a81a353785f3d16c0cd0312a8da8f17e028fd4bbaa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.9.12-meta-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:6236faaa93f504f1f9d4e1eabccc637f19cea95dfb3551ffd9d890341e6897b4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.4 MB (17433663 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e014f8c8dd5143533c2d241216b39fab7c413eeaeba5192b638ce24d46c1c96f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:26 GMT
ADD file:6dd87346b8be240b21b4f4d9296253bf0d28b6579aa52d2118872e3936963b6b in / 
# Mon, 07 Aug 2023 19:20:26 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 20:30:41 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 09 Aug 2023 01:54:15 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Wed, 09 Aug 2023 01:54:30 GMT
ENV INFLUXDB_VERSION=1.9.12-c1.9.12
# Wed, 09 Aug 2023 01:54:48 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/etc/influxdb/influxdb-meta.conf &&     chmod +x /usr/src/influxdb-*/usr/bin/* &&     cp -a /usr/src/influxdb-*/usr/bin/. /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Wed, 09 Aug 2023 01:54:48 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Wed, 09 Aug 2023 01:54:48 GMT
EXPOSE 8091
# Wed, 09 Aug 2023 01:54:48 GMT
VOLUME [/var/lib/influxdb]
# Wed, 09 Aug 2023 01:54:48 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Wed, 09 Aug 2023 01:54:48 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 09 Aug 2023 01:54:48 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:9398808236ffac29e60c04ec906d8d409af7fa19dc57d8c65ad167e9c4967006`  
		Last Modified: Mon, 07 Aug 2023 19:21:08 GMT  
		Size: 3.4 MB (3378609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bdca2725167af68b5a2e88c072759b23a3bf0e32c8526c7e9b89f616db5a88d`  
		Last Modified: Mon, 07 Aug 2023 20:31:39 GMT  
		Size: 279.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90412949f8cfd74e35fbc8d623c490f3d19ec67abaac2447d3f55007f36a18a1`  
		Last Modified: Wed, 09 Aug 2023 01:56:21 GMT  
		Size: 1.5 MB (1472417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:617f4e7c957e2e9f40805d4ffbdb1e0d5720329ca768d5323d4c1bfaa759cb8a`  
		Last Modified: Wed, 09 Aug 2023 01:56:53 GMT  
		Size: 12.6 MB (12581763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e80ee0272fb9aac850a9c2ef72a44f063ec1f8c66518dd2d5aab1d714ba1a9eb`  
		Last Modified: Wed, 09 Aug 2023 01:56:51 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:895dc0a2527c7ea6aa44324b28c00248e69a2fdb0a9c64c47cebb2a3f90271a1`  
		Last Modified: Wed, 09 Aug 2023 01:56:51 GMT  
		Size: 375.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:2.7`

```console
$ docker pull influxdb@sha256:17390018173e18a8b7d0c3c6495a6cc066a82295084d7a427dd32ea2c5928d4a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:2.7` - linux; amd64

```console
$ docker pull influxdb@sha256:e970833ae6d02fe0833367b3fbf8a5c30b881931d1e300ecea4341d8e50a1221
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.6 MB (114639373 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6921cbed08d00461f99a782670f83c8808fa70077c2b33dee20d583a57ac6e50`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Thu, 07 Sep 2023 00:21:13 GMT
ADD file:cb5fcc80c057b356a31492a20c6e3a75b70ed70a663506c8e97ad730ae32a02d in / 
# Thu, 07 Sep 2023 00:21:13 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 01:40:15 GMT
RUN export DEBIAN_FRONTEND=noninteractive &&     apt-get update -y &&     apt-get install -y --no-install-recommends       ca-certificates       curl       gnupg &&     apt-get clean &&     rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 01:40:16 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     curl -fLo /usr/local/bin/dasel "https://github.com/TomWright/dasel/releases/download/v2.1.2/dasel_linux_${arch}" &&     case ${arch} in       amd64) echo 'e4b43d8c7d76904e2401dc81de0900d9cb69b006794ff3901ec5d50e96baa8ef  /usr/local/bin/dasel' ;;       arm64) echo '92b83f30949679197403ff7a7e0f9ef3e458c1c55031d9c1bc112364e487d57d  /usr/local/bin/dasel' ;;     esac | sha256sum -c - &&     chmod +x /usr/local/bin/dasel &&     dasel --version
# Thu, 07 Sep 2023 01:40:17 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --create-home --home-dir=/home/influxdb --shell=/bin/bash influxdb
# Thu, 07 Sep 2023 01:40:17 GMT
ENV GOSU_VER=1.12
# Thu, 07 Sep 2023 01:40:19 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       B42F6819007F00F88E364FD4036A9C25BF357DD4 &&     curl -fLo /usr/local/bin/gosu     "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-${arch}"          -fLo /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-${arch}.asc" &&     gpg --batch --verify /usr/local/bin/gosu.asc                          /usr/local/bin/gosu &&     rm -rf /usr/local/bin/gosu.asc &&     chmod +x /usr/local/bin/gosu &&     gosu --version &&     gosu nobody true
# Thu, 07 Sep 2023 01:40:19 GMT
ENV INFLUXDB_VERSION=2.7.1
# Thu, 07 Sep 2023 01:40:23 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     cp "influxdb2_linux_${arch}/influxd" /usr/local/bin/influxd &&     rm -rf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"            "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"            "influxdb2_linux_${arch}" &&     influxd version
# Thu, 07 Sep 2023 01:40:23 GMT
ENV INFLUX_CLI_VERSION=2.7.3
# Thu, 07 Sep 2023 01:40:25 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     cp influx /usr/local/bin/influx &&     rm -rf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     influx version
# Thu, 07 Sep 2023 01:40:26 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Thu, 07 Sep 2023 01:40:26 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Thu, 07 Sep 2023 01:40:26 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Thu, 07 Sep 2023 01:40:26 GMT
COPY file:3ef80d0bcfdeda3282c98ad7a6b84218cd7593d6a3bbf027c3083db3b7acad32 in /entrypoint.sh 
# Thu, 07 Sep 2023 01:40:26 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 07 Sep 2023 01:40:26 GMT
CMD ["influxd"]
# Thu, 07 Sep 2023 01:40:26 GMT
EXPOSE 8086
# Thu, 07 Sep 2023 01:40:26 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Thu, 07 Sep 2023 01:40:26 GMT
ENV INFLUXD_INIT_PORT=9999
# Thu, 07 Sep 2023 01:40:27 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Thu, 07 Sep 2023 01:40:27 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:7d97e254a0461b0a30b3f443f1daa0d620a3cc6ff4e2714cc1cfd96ace5b7a7e`  
		Last Modified: Thu, 07 Sep 2023 00:26:03 GMT  
		Size: 31.4 MB (31417503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1768238c1d21edcca065dcc4e383b02cac745ff7e9a01c9c82dde121aad8db12`  
		Last Modified: Thu, 07 Sep 2023 01:41:18 GMT  
		Size: 6.3 MB (6327853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a8cf89659e591ba916aa2258a818d30c11630eebc07d2b7426f788db5153402`  
		Last Modified: Thu, 07 Sep 2023 01:41:16 GMT  
		Size: 6.4 MB (6434102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bbbd9ea79cb9c17df3e62a72623699b0f865b231433805f803e80f2f9f56653`  
		Last Modified: Thu, 07 Sep 2023 01:41:15 GMT  
		Size: 4.1 KB (4114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f5bace44f952cfb244599835428862f45f33378893152e887d7a30172b1a048`  
		Last Modified: Thu, 07 Sep 2023 01:41:16 GMT  
		Size: 986.0 KB (985990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cac023e05c09814a2525011e7dca324d1250dd751e504ac730bd204054e916a2`  
		Last Modified: Thu, 07 Sep 2023 01:41:19 GMT  
		Size: 46.3 MB (46334319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eda2b107f008112ca1bd7bc6cce9ba6598e04bdbe0a7e32899d77ce7393cef5b`  
		Last Modified: Thu, 07 Sep 2023 01:41:16 GMT  
		Size: 23.1 MB (23128343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4792803ad3fdb0f7c42ea7612417b7ea4474a31f785fd2cca132bc54d4859f1d`  
		Last Modified: Thu, 07 Sep 2023 01:41:13 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18438cd9981878262b7f8f9151fba89f3e02a7a6fc0d3260749f2309a1a85456`  
		Last Modified: Thu, 07 Sep 2023 01:41:13 GMT  
		Size: 261.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0458408b9bdf79125c7d02ab7f75816379a4061341ed2ad631a0e06e7efbf31a`  
		Last Modified: Thu, 07 Sep 2023 01:41:13 GMT  
		Size: 6.6 KB (6612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:2.7` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:507a6e517b68c2621e9bf4c716314fd3301f22f1e638a54259548d80c6cbad2a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.4 MB (109356541 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e21e8f1eba2f968cb42868da326aa2e29978c5b298c7565bc3033bdd316f68c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Thu, 07 Sep 2023 00:39:53 GMT
ADD file:abd1ad48ae3ebec7a6ecc8ce3016c25be2afcbaedfcb904bc89b1ce59400aef0 in / 
# Thu, 07 Sep 2023 00:39:54 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 05:36:03 GMT
RUN export DEBIAN_FRONTEND=noninteractive &&     apt-get update -y &&     apt-get install -y --no-install-recommends       ca-certificates       curl       gnupg &&     apt-get clean &&     rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 05:36:04 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     curl -fLo /usr/local/bin/dasel "https://github.com/TomWright/dasel/releases/download/v2.1.2/dasel_linux_${arch}" &&     case ${arch} in       amd64) echo 'e4b43d8c7d76904e2401dc81de0900d9cb69b006794ff3901ec5d50e96baa8ef  /usr/local/bin/dasel' ;;       arm64) echo '92b83f30949679197403ff7a7e0f9ef3e458c1c55031d9c1bc112364e487d57d  /usr/local/bin/dasel' ;;     esac | sha256sum -c - &&     chmod +x /usr/local/bin/dasel &&     dasel --version
# Thu, 07 Sep 2023 05:36:04 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --create-home --home-dir=/home/influxdb --shell=/bin/bash influxdb
# Thu, 07 Sep 2023 05:36:05 GMT
ENV GOSU_VER=1.12
# Thu, 07 Sep 2023 05:36:07 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       B42F6819007F00F88E364FD4036A9C25BF357DD4 &&     curl -fLo /usr/local/bin/gosu     "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-${arch}"          -fLo /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-${arch}.asc" &&     gpg --batch --verify /usr/local/bin/gosu.asc                          /usr/local/bin/gosu &&     rm -rf /usr/local/bin/gosu.asc &&     chmod +x /usr/local/bin/gosu &&     gosu --version &&     gosu nobody true
# Thu, 07 Sep 2023 05:36:07 GMT
ENV INFLUXDB_VERSION=2.7.1
# Thu, 07 Sep 2023 05:36:10 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     cp "influxdb2_linux_${arch}/influxd" /usr/local/bin/influxd &&     rm -rf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"            "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"            "influxdb2_linux_${arch}" &&     influxd version
# Thu, 07 Sep 2023 05:36:11 GMT
ENV INFLUX_CLI_VERSION=2.7.3
# Thu, 07 Sep 2023 05:36:13 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     cp influx /usr/local/bin/influx &&     rm -rf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     influx version
# Thu, 07 Sep 2023 05:36:13 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Thu, 07 Sep 2023 05:36:14 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Thu, 07 Sep 2023 05:36:14 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Thu, 07 Sep 2023 05:36:14 GMT
COPY file:3ef80d0bcfdeda3282c98ad7a6b84218cd7593d6a3bbf027c3083db3b7acad32 in /entrypoint.sh 
# Thu, 07 Sep 2023 05:36:14 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 07 Sep 2023 05:36:14 GMT
CMD ["influxd"]
# Thu, 07 Sep 2023 05:36:14 GMT
EXPOSE 8086
# Thu, 07 Sep 2023 05:36:14 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Thu, 07 Sep 2023 05:36:14 GMT
ENV INFLUXD_INIT_PORT=9999
# Thu, 07 Sep 2023 05:36:14 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Thu, 07 Sep 2023 05:36:14 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:f96ab15157043879c2ff23e0556e798eba6a6ff3d7fd5d1384de223bb9f66f1d`  
		Last Modified: Thu, 07 Sep 2023 00:43:41 GMT  
		Size: 30.1 MB (30062903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4abaa895672d07010025a3b438860c732da8a8fccf5dc335a51544fb9025cb95`  
		Last Modified: Thu, 07 Sep 2023 05:36:34 GMT  
		Size: 6.3 MB (6308767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65064d89682d695ed1fdcba8c6b740dd5caae58affe7d753a10a50292efe0d74`  
		Last Modified: Thu, 07 Sep 2023 05:36:32 GMT  
		Size: 6.0 MB (5953765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39608a77e87221c0d4137100cf52ab41b759d953066b2d53aadba26f6e330d06`  
		Last Modified: Thu, 07 Sep 2023 05:36:31 GMT  
		Size: 4.1 KB (4117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8905172f7f9cdd2432cc2f4ab6a11a6a5672939d05a15161091999a0303bb6e`  
		Last Modified: Thu, 07 Sep 2023 05:36:31 GMT  
		Size: 921.5 KB (921471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c99241f70a82d0cca3a38168ab21d0af633024521dac2d196ec22d78d197ac2`  
		Last Modified: Thu, 07 Sep 2023 05:36:33 GMT  
		Size: 44.4 MB (44435781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e34b1ef8e734d97f099114726a375d0365254557f9002c294cf6a398913bfbfc`  
		Last Modified: Thu, 07 Sep 2023 05:36:31 GMT  
		Size: 21.7 MB (21662588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66dae31c3c2091ed8fdb0d77cf7e6fa44c894fbdf33d7568eb1642b69ff1600e`  
		Last Modified: Thu, 07 Sep 2023 05:36:29 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc8f1f5a6f744a26d73cb07dbf19389e31ee3cab6680b9910baf148c9f5a4d05`  
		Last Modified: Thu, 07 Sep 2023 05:36:29 GMT  
		Size: 261.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f81d55cc75ef9ca2dc5e20c1e1b9cecd2d4080cbdbbb77a18c9a6700a93ab32`  
		Last Modified: Thu, 07 Sep 2023 05:36:29 GMT  
		Size: 6.6 KB (6612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:2.7-alpine`

```console
$ docker pull influxdb@sha256:e42bc2a7ab4b905183155906328d0d3a31d56eb72cd7fd8479772f6be862b873
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:2.7-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:8fea506e2c35f4c7a71e8d83c3607305f4f7d7cf8d5ed4ff9780752bf2bd94bd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.9 MB (87874009 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fbf8b4b940b201874dd347e8cf177667077be4e03dd67d87de6d4dacd800d195`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:26 GMT
ADD file:6dd87346b8be240b21b4f4d9296253bf0d28b6579aa52d2118872e3936963b6b in / 
# Mon, 07 Aug 2023 19:20:26 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 20:30:41 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 09 Aug 2023 01:55:45 GMT
RUN apk add --no-cache       bash       ca-certificates       curl       gnupg       run-parts       su-exec       tzdata &&     update-ca-certificates
# Wed, 09 Aug 2023 01:55:46 GMT
RUN case "$(apk --print-arch)" in       x86_64)  arch=amd64 ;;       aarch64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     curl -fLo /usr/local/bin/dasel "https://github.com/TomWright/dasel/releases/download/v2.1.2/dasel_linux_${arch}" &&     case ${arch} in       amd64) echo 'e4b43d8c7d76904e2401dc81de0900d9cb69b006794ff3901ec5d50e96baa8ef  /usr/local/bin/dasel' ;;       arm64) echo '92b83f30949679197403ff7a7e0f9ef3e458c1c55031d9c1bc112364e487d57d  /usr/local/bin/dasel' ;;     esac | sha256sum -c - &&     chmod +x /usr/local/bin/dasel &&     dasel --version
# Wed, 09 Aug 2023 01:55:47 GMT
RUN addgroup -S -g 1000 influxdb &&     adduser -S -G influxdb -u 1000 -h /home/influxdb -s /bin/sh influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Wed, 09 Aug 2023 01:55:47 GMT
ENV INFLUXDB_VERSION=2.7.1
# Wed, 09 Aug 2023 01:55:51 GMT
RUN case "$(apk --print-arch)" in       x86_64)  arch=amd64 ;;       aarch64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&    curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     cp "influxdb2_linux_${arch}/influxd" /usr/local/bin/influxd &&     rm -rf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"            "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"            "influxdb2_linux_${arch}" &&     influxd version
# Wed, 09 Aug 2023 01:55:51 GMT
ENV INFLUX_CLI_VERSION=2.7.3
# Wed, 09 Aug 2023 01:55:54 GMT
RUN case "$(apk --print-arch)" in       x86_64)  arch=amd64 ;;       aarch64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     cp influx /usr/local/bin/influx &&     rm -rf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     influx version
# Wed, 09 Aug 2023 01:55:54 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Wed, 09 Aug 2023 01:55:54 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Wed, 09 Aug 2023 01:55:54 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Wed, 09 Aug 2023 01:55:54 GMT
COPY file:0c651d5752d62a8235f9939458cdfe0447d6491e071a852d95bf87ff7179f6a0 in /entrypoint.sh 
# Wed, 09 Aug 2023 01:55:55 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 09 Aug 2023 01:55:55 GMT
CMD ["influxd"]
# Wed, 09 Aug 2023 01:55:55 GMT
EXPOSE 8086
# Wed, 09 Aug 2023 01:55:55 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Wed, 09 Aug 2023 01:55:55 GMT
ENV INFLUXD_INIT_PORT=9999
# Wed, 09 Aug 2023 01:55:55 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Wed, 09 Aug 2023 01:55:55 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:9398808236ffac29e60c04ec906d8d409af7fa19dc57d8c65ad167e9c4967006`  
		Last Modified: Mon, 07 Aug 2023 19:21:08 GMT  
		Size: 3.4 MB (3378609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bdca2725167af68b5a2e88c072759b23a3bf0e32c8526c7e9b89f616db5a88d`  
		Last Modified: Mon, 07 Aug 2023 20:31:39 GMT  
		Size: 279.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3a3f140b605173ff8cd3e6a398d31f3efae2350a5a0499e145583f931a911e4`  
		Last Modified: Wed, 09 Aug 2023 01:58:02 GMT  
		Size: 8.6 MB (8589935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9676915317d0ca4b6e8eab71c4b574f7733746aeb5b28e341bd7acecb71f46c1`  
		Last Modified: Wed, 09 Aug 2023 01:58:02 GMT  
		Size: 6.4 MB (6434109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3b42598376fb2ab2a87e37e7992992ebafded66021d9ba7079a8fd41d8b070b`  
		Last Modified: Wed, 09 Aug 2023 01:58:01 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb9bd2e16518ad4ff61e5eb77ffef3b5c9d336b5fc84f0310fca6883d7455c2a`  
		Last Modified: Wed, 09 Aug 2023 01:58:05 GMT  
		Size: 46.3 MB (46334322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d52f10fd03bbf4b6ea4d4dc2b178a3285f144fbe25d4a9d60336cc453cfc5e2`  
		Last Modified: Wed, 09 Aug 2023 01:58:02 GMT  
		Size: 23.1 MB (23128342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b5e76f294fdf721006a8c1f05a2753ea3c0aa007477766e76df439ac20752f9`  
		Last Modified: Wed, 09 Aug 2023 01:57:59 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e219547fcd7d310d78a64ffaca570c33363b7faa7f93eb1872c57c2c817c01d5`  
		Last Modified: Wed, 09 Aug 2023 01:57:59 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:945fba015ba45978887d983782965c16cd52f1c40031ef4318f3054579d8fa17`  
		Last Modified: Wed, 09 Aug 2023 01:57:59 GMT  
		Size: 6.6 KB (6609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:2.7-alpine` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:9262eb61ef1304540c4c41bbbd02856de85f9906c9cdb8a4106ca7e16baf8c6f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.8 MB (83829280 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7257778f282477b73bfadf1e535f693f6abd8275fad507d886b7b32874731cb6`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:22 GMT
ADD file:9e054a25c83111adc857a7f988336ee40eea5e1794ed30a80d465e8d472342e2 in / 
# Mon, 07 Aug 2023 19:39:22 GMT
CMD ["/bin/sh"]
# Wed, 09 Aug 2023 00:46:08 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 09 Aug 2023 00:46:10 GMT
RUN apk add --no-cache       bash       ca-certificates       curl       gnupg       run-parts       su-exec       tzdata &&     update-ca-certificates
# Wed, 09 Aug 2023 00:46:11 GMT
RUN case "$(apk --print-arch)" in       x86_64)  arch=amd64 ;;       aarch64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     curl -fLo /usr/local/bin/dasel "https://github.com/TomWright/dasel/releases/download/v2.1.2/dasel_linux_${arch}" &&     case ${arch} in       amd64) echo 'e4b43d8c7d76904e2401dc81de0900d9cb69b006794ff3901ec5d50e96baa8ef  /usr/local/bin/dasel' ;;       arm64) echo '92b83f30949679197403ff7a7e0f9ef3e458c1c55031d9c1bc112364e487d57d  /usr/local/bin/dasel' ;;     esac | sha256sum -c - &&     chmod +x /usr/local/bin/dasel &&     dasel --version
# Wed, 09 Aug 2023 00:46:12 GMT
RUN addgroup -S -g 1000 influxdb &&     adduser -S -G influxdb -u 1000 -h /home/influxdb -s /bin/sh influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Wed, 09 Aug 2023 00:46:12 GMT
ENV INFLUXDB_VERSION=2.7.1
# Wed, 09 Aug 2023 00:46:17 GMT
RUN case "$(apk --print-arch)" in       x86_64)  arch=amd64 ;;       aarch64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&    curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     cp "influxdb2_linux_${arch}/influxd" /usr/local/bin/influxd &&     rm -rf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"            "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"            "influxdb2_linux_${arch}" &&     influxd version
# Wed, 09 Aug 2023 00:46:17 GMT
ENV INFLUX_CLI_VERSION=2.7.3
# Wed, 09 Aug 2023 00:46:20 GMT
RUN case "$(apk --print-arch)" in       x86_64)  arch=amd64 ;;       aarch64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     cp influx /usr/local/bin/influx &&     rm -rf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     influx version
# Wed, 09 Aug 2023 00:46:20 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Wed, 09 Aug 2023 00:46:20 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Wed, 09 Aug 2023 00:46:20 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Wed, 09 Aug 2023 00:46:20 GMT
COPY file:0c651d5752d62a8235f9939458cdfe0447d6491e071a852d95bf87ff7179f6a0 in /entrypoint.sh 
# Wed, 09 Aug 2023 00:46:20 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 09 Aug 2023 00:46:20 GMT
CMD ["influxd"]
# Wed, 09 Aug 2023 00:46:21 GMT
EXPOSE 8086
# Wed, 09 Aug 2023 00:46:21 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Wed, 09 Aug 2023 00:46:21 GMT
ENV INFLUXD_INIT_PORT=9999
# Wed, 09 Aug 2023 00:46:21 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Wed, 09 Aug 2023 00:46:21 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:4060ece20d7ac783f52cbe28a35fd5b06f90f7b4d773bae0d956024e85ff35b6`  
		Last Modified: Mon, 07 Aug 2023 19:39:59 GMT  
		Size: 3.3 MB (3258290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bd1799839c258f2f362340c258c49aa080e354fd0e137266f54d413ef004a1b`  
		Last Modified: Wed, 09 Aug 2023 00:46:37 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f30f1a2fe004c2cdf0167c7d1f5958d25e650840e0625814e3032ecc6973f334`  
		Last Modified: Wed, 09 Aug 2023 00:46:37 GMT  
		Size: 8.5 MB (8510115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebfbe81a9d67236da8399d75342e23015e979e0e1b3e932e7e22f80f3029775b`  
		Last Modified: Wed, 09 Aug 2023 00:46:37 GMT  
		Size: 6.0 MB (5953754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:743e1b62e9110324931cfbd5f8ed76319fe9ca7c484685c263cba135e032e93b`  
		Last Modified: Wed, 09 Aug 2023 00:46:36 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c464170026f8f97d6daafd06f65bd87aa93b8a49b2a5ae5a425e111d63518b0`  
		Last Modified: Wed, 09 Aug 2023 00:46:38 GMT  
		Size: 44.4 MB (44435831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c2b153f7087828fcb85296475fd1d6882853b96d89dc6d3c0f54f82a101552d`  
		Last Modified: Wed, 09 Aug 2023 00:46:37 GMT  
		Size: 21.7 MB (21662595 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77aa542a3877dd874c5d6b906cf4de13de97e274646fb6f55e931e3a228e83f5`  
		Last Modified: Wed, 09 Aug 2023 00:46:34 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f98ade2b5c03a2d4c21d8dfe8af8d1828e19ee709483115c654fa4739935391f`  
		Last Modified: Wed, 09 Aug 2023 00:46:34 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93743bee855eb887605313e1d74fd9b3225325f9cc7f7ca18ec012d9704d8803`  
		Last Modified: Wed, 09 Aug 2023 00:46:34 GMT  
		Size: 6.6 KB (6609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:2.7.1`

```console
$ docker pull influxdb@sha256:17390018173e18a8b7d0c3c6495a6cc066a82295084d7a427dd32ea2c5928d4a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:2.7.1` - linux; amd64

```console
$ docker pull influxdb@sha256:e970833ae6d02fe0833367b3fbf8a5c30b881931d1e300ecea4341d8e50a1221
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.6 MB (114639373 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6921cbed08d00461f99a782670f83c8808fa70077c2b33dee20d583a57ac6e50`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Thu, 07 Sep 2023 00:21:13 GMT
ADD file:cb5fcc80c057b356a31492a20c6e3a75b70ed70a663506c8e97ad730ae32a02d in / 
# Thu, 07 Sep 2023 00:21:13 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 01:40:15 GMT
RUN export DEBIAN_FRONTEND=noninteractive &&     apt-get update -y &&     apt-get install -y --no-install-recommends       ca-certificates       curl       gnupg &&     apt-get clean &&     rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 01:40:16 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     curl -fLo /usr/local/bin/dasel "https://github.com/TomWright/dasel/releases/download/v2.1.2/dasel_linux_${arch}" &&     case ${arch} in       amd64) echo 'e4b43d8c7d76904e2401dc81de0900d9cb69b006794ff3901ec5d50e96baa8ef  /usr/local/bin/dasel' ;;       arm64) echo '92b83f30949679197403ff7a7e0f9ef3e458c1c55031d9c1bc112364e487d57d  /usr/local/bin/dasel' ;;     esac | sha256sum -c - &&     chmod +x /usr/local/bin/dasel &&     dasel --version
# Thu, 07 Sep 2023 01:40:17 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --create-home --home-dir=/home/influxdb --shell=/bin/bash influxdb
# Thu, 07 Sep 2023 01:40:17 GMT
ENV GOSU_VER=1.12
# Thu, 07 Sep 2023 01:40:19 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       B42F6819007F00F88E364FD4036A9C25BF357DD4 &&     curl -fLo /usr/local/bin/gosu     "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-${arch}"          -fLo /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-${arch}.asc" &&     gpg --batch --verify /usr/local/bin/gosu.asc                          /usr/local/bin/gosu &&     rm -rf /usr/local/bin/gosu.asc &&     chmod +x /usr/local/bin/gosu &&     gosu --version &&     gosu nobody true
# Thu, 07 Sep 2023 01:40:19 GMT
ENV INFLUXDB_VERSION=2.7.1
# Thu, 07 Sep 2023 01:40:23 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     cp "influxdb2_linux_${arch}/influxd" /usr/local/bin/influxd &&     rm -rf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"            "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"            "influxdb2_linux_${arch}" &&     influxd version
# Thu, 07 Sep 2023 01:40:23 GMT
ENV INFLUX_CLI_VERSION=2.7.3
# Thu, 07 Sep 2023 01:40:25 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     cp influx /usr/local/bin/influx &&     rm -rf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     influx version
# Thu, 07 Sep 2023 01:40:26 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Thu, 07 Sep 2023 01:40:26 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Thu, 07 Sep 2023 01:40:26 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Thu, 07 Sep 2023 01:40:26 GMT
COPY file:3ef80d0bcfdeda3282c98ad7a6b84218cd7593d6a3bbf027c3083db3b7acad32 in /entrypoint.sh 
# Thu, 07 Sep 2023 01:40:26 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 07 Sep 2023 01:40:26 GMT
CMD ["influxd"]
# Thu, 07 Sep 2023 01:40:26 GMT
EXPOSE 8086
# Thu, 07 Sep 2023 01:40:26 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Thu, 07 Sep 2023 01:40:26 GMT
ENV INFLUXD_INIT_PORT=9999
# Thu, 07 Sep 2023 01:40:27 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Thu, 07 Sep 2023 01:40:27 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:7d97e254a0461b0a30b3f443f1daa0d620a3cc6ff4e2714cc1cfd96ace5b7a7e`  
		Last Modified: Thu, 07 Sep 2023 00:26:03 GMT  
		Size: 31.4 MB (31417503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1768238c1d21edcca065dcc4e383b02cac745ff7e9a01c9c82dde121aad8db12`  
		Last Modified: Thu, 07 Sep 2023 01:41:18 GMT  
		Size: 6.3 MB (6327853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a8cf89659e591ba916aa2258a818d30c11630eebc07d2b7426f788db5153402`  
		Last Modified: Thu, 07 Sep 2023 01:41:16 GMT  
		Size: 6.4 MB (6434102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bbbd9ea79cb9c17df3e62a72623699b0f865b231433805f803e80f2f9f56653`  
		Last Modified: Thu, 07 Sep 2023 01:41:15 GMT  
		Size: 4.1 KB (4114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f5bace44f952cfb244599835428862f45f33378893152e887d7a30172b1a048`  
		Last Modified: Thu, 07 Sep 2023 01:41:16 GMT  
		Size: 986.0 KB (985990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cac023e05c09814a2525011e7dca324d1250dd751e504ac730bd204054e916a2`  
		Last Modified: Thu, 07 Sep 2023 01:41:19 GMT  
		Size: 46.3 MB (46334319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eda2b107f008112ca1bd7bc6cce9ba6598e04bdbe0a7e32899d77ce7393cef5b`  
		Last Modified: Thu, 07 Sep 2023 01:41:16 GMT  
		Size: 23.1 MB (23128343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4792803ad3fdb0f7c42ea7612417b7ea4474a31f785fd2cca132bc54d4859f1d`  
		Last Modified: Thu, 07 Sep 2023 01:41:13 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18438cd9981878262b7f8f9151fba89f3e02a7a6fc0d3260749f2309a1a85456`  
		Last Modified: Thu, 07 Sep 2023 01:41:13 GMT  
		Size: 261.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0458408b9bdf79125c7d02ab7f75816379a4061341ed2ad631a0e06e7efbf31a`  
		Last Modified: Thu, 07 Sep 2023 01:41:13 GMT  
		Size: 6.6 KB (6612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:2.7.1` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:507a6e517b68c2621e9bf4c716314fd3301f22f1e638a54259548d80c6cbad2a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.4 MB (109356541 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e21e8f1eba2f968cb42868da326aa2e29978c5b298c7565bc3033bdd316f68c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Thu, 07 Sep 2023 00:39:53 GMT
ADD file:abd1ad48ae3ebec7a6ecc8ce3016c25be2afcbaedfcb904bc89b1ce59400aef0 in / 
# Thu, 07 Sep 2023 00:39:54 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 05:36:03 GMT
RUN export DEBIAN_FRONTEND=noninteractive &&     apt-get update -y &&     apt-get install -y --no-install-recommends       ca-certificates       curl       gnupg &&     apt-get clean &&     rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 05:36:04 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     curl -fLo /usr/local/bin/dasel "https://github.com/TomWright/dasel/releases/download/v2.1.2/dasel_linux_${arch}" &&     case ${arch} in       amd64) echo 'e4b43d8c7d76904e2401dc81de0900d9cb69b006794ff3901ec5d50e96baa8ef  /usr/local/bin/dasel' ;;       arm64) echo '92b83f30949679197403ff7a7e0f9ef3e458c1c55031d9c1bc112364e487d57d  /usr/local/bin/dasel' ;;     esac | sha256sum -c - &&     chmod +x /usr/local/bin/dasel &&     dasel --version
# Thu, 07 Sep 2023 05:36:04 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --create-home --home-dir=/home/influxdb --shell=/bin/bash influxdb
# Thu, 07 Sep 2023 05:36:05 GMT
ENV GOSU_VER=1.12
# Thu, 07 Sep 2023 05:36:07 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       B42F6819007F00F88E364FD4036A9C25BF357DD4 &&     curl -fLo /usr/local/bin/gosu     "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-${arch}"          -fLo /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-${arch}.asc" &&     gpg --batch --verify /usr/local/bin/gosu.asc                          /usr/local/bin/gosu &&     rm -rf /usr/local/bin/gosu.asc &&     chmod +x /usr/local/bin/gosu &&     gosu --version &&     gosu nobody true
# Thu, 07 Sep 2023 05:36:07 GMT
ENV INFLUXDB_VERSION=2.7.1
# Thu, 07 Sep 2023 05:36:10 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     cp "influxdb2_linux_${arch}/influxd" /usr/local/bin/influxd &&     rm -rf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"            "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"            "influxdb2_linux_${arch}" &&     influxd version
# Thu, 07 Sep 2023 05:36:11 GMT
ENV INFLUX_CLI_VERSION=2.7.3
# Thu, 07 Sep 2023 05:36:13 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     cp influx /usr/local/bin/influx &&     rm -rf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     influx version
# Thu, 07 Sep 2023 05:36:13 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Thu, 07 Sep 2023 05:36:14 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Thu, 07 Sep 2023 05:36:14 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Thu, 07 Sep 2023 05:36:14 GMT
COPY file:3ef80d0bcfdeda3282c98ad7a6b84218cd7593d6a3bbf027c3083db3b7acad32 in /entrypoint.sh 
# Thu, 07 Sep 2023 05:36:14 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 07 Sep 2023 05:36:14 GMT
CMD ["influxd"]
# Thu, 07 Sep 2023 05:36:14 GMT
EXPOSE 8086
# Thu, 07 Sep 2023 05:36:14 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Thu, 07 Sep 2023 05:36:14 GMT
ENV INFLUXD_INIT_PORT=9999
# Thu, 07 Sep 2023 05:36:14 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Thu, 07 Sep 2023 05:36:14 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:f96ab15157043879c2ff23e0556e798eba6a6ff3d7fd5d1384de223bb9f66f1d`  
		Last Modified: Thu, 07 Sep 2023 00:43:41 GMT  
		Size: 30.1 MB (30062903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4abaa895672d07010025a3b438860c732da8a8fccf5dc335a51544fb9025cb95`  
		Last Modified: Thu, 07 Sep 2023 05:36:34 GMT  
		Size: 6.3 MB (6308767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65064d89682d695ed1fdcba8c6b740dd5caae58affe7d753a10a50292efe0d74`  
		Last Modified: Thu, 07 Sep 2023 05:36:32 GMT  
		Size: 6.0 MB (5953765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39608a77e87221c0d4137100cf52ab41b759d953066b2d53aadba26f6e330d06`  
		Last Modified: Thu, 07 Sep 2023 05:36:31 GMT  
		Size: 4.1 KB (4117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8905172f7f9cdd2432cc2f4ab6a11a6a5672939d05a15161091999a0303bb6e`  
		Last Modified: Thu, 07 Sep 2023 05:36:31 GMT  
		Size: 921.5 KB (921471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c99241f70a82d0cca3a38168ab21d0af633024521dac2d196ec22d78d197ac2`  
		Last Modified: Thu, 07 Sep 2023 05:36:33 GMT  
		Size: 44.4 MB (44435781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e34b1ef8e734d97f099114726a375d0365254557f9002c294cf6a398913bfbfc`  
		Last Modified: Thu, 07 Sep 2023 05:36:31 GMT  
		Size: 21.7 MB (21662588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66dae31c3c2091ed8fdb0d77cf7e6fa44c894fbdf33d7568eb1642b69ff1600e`  
		Last Modified: Thu, 07 Sep 2023 05:36:29 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc8f1f5a6f744a26d73cb07dbf19389e31ee3cab6680b9910baf148c9f5a4d05`  
		Last Modified: Thu, 07 Sep 2023 05:36:29 GMT  
		Size: 261.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f81d55cc75ef9ca2dc5e20c1e1b9cecd2d4080cbdbbb77a18c9a6700a93ab32`  
		Last Modified: Thu, 07 Sep 2023 05:36:29 GMT  
		Size: 6.6 KB (6612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:2.7.1-alpine`

```console
$ docker pull influxdb@sha256:e42bc2a7ab4b905183155906328d0d3a31d56eb72cd7fd8479772f6be862b873
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:2.7.1-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:8fea506e2c35f4c7a71e8d83c3607305f4f7d7cf8d5ed4ff9780752bf2bd94bd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.9 MB (87874009 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fbf8b4b940b201874dd347e8cf177667077be4e03dd67d87de6d4dacd800d195`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:26 GMT
ADD file:6dd87346b8be240b21b4f4d9296253bf0d28b6579aa52d2118872e3936963b6b in / 
# Mon, 07 Aug 2023 19:20:26 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 20:30:41 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 09 Aug 2023 01:55:45 GMT
RUN apk add --no-cache       bash       ca-certificates       curl       gnupg       run-parts       su-exec       tzdata &&     update-ca-certificates
# Wed, 09 Aug 2023 01:55:46 GMT
RUN case "$(apk --print-arch)" in       x86_64)  arch=amd64 ;;       aarch64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     curl -fLo /usr/local/bin/dasel "https://github.com/TomWright/dasel/releases/download/v2.1.2/dasel_linux_${arch}" &&     case ${arch} in       amd64) echo 'e4b43d8c7d76904e2401dc81de0900d9cb69b006794ff3901ec5d50e96baa8ef  /usr/local/bin/dasel' ;;       arm64) echo '92b83f30949679197403ff7a7e0f9ef3e458c1c55031d9c1bc112364e487d57d  /usr/local/bin/dasel' ;;     esac | sha256sum -c - &&     chmod +x /usr/local/bin/dasel &&     dasel --version
# Wed, 09 Aug 2023 01:55:47 GMT
RUN addgroup -S -g 1000 influxdb &&     adduser -S -G influxdb -u 1000 -h /home/influxdb -s /bin/sh influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Wed, 09 Aug 2023 01:55:47 GMT
ENV INFLUXDB_VERSION=2.7.1
# Wed, 09 Aug 2023 01:55:51 GMT
RUN case "$(apk --print-arch)" in       x86_64)  arch=amd64 ;;       aarch64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&    curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     cp "influxdb2_linux_${arch}/influxd" /usr/local/bin/influxd &&     rm -rf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"            "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"            "influxdb2_linux_${arch}" &&     influxd version
# Wed, 09 Aug 2023 01:55:51 GMT
ENV INFLUX_CLI_VERSION=2.7.3
# Wed, 09 Aug 2023 01:55:54 GMT
RUN case "$(apk --print-arch)" in       x86_64)  arch=amd64 ;;       aarch64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     cp influx /usr/local/bin/influx &&     rm -rf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     influx version
# Wed, 09 Aug 2023 01:55:54 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Wed, 09 Aug 2023 01:55:54 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Wed, 09 Aug 2023 01:55:54 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Wed, 09 Aug 2023 01:55:54 GMT
COPY file:0c651d5752d62a8235f9939458cdfe0447d6491e071a852d95bf87ff7179f6a0 in /entrypoint.sh 
# Wed, 09 Aug 2023 01:55:55 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 09 Aug 2023 01:55:55 GMT
CMD ["influxd"]
# Wed, 09 Aug 2023 01:55:55 GMT
EXPOSE 8086
# Wed, 09 Aug 2023 01:55:55 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Wed, 09 Aug 2023 01:55:55 GMT
ENV INFLUXD_INIT_PORT=9999
# Wed, 09 Aug 2023 01:55:55 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Wed, 09 Aug 2023 01:55:55 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:9398808236ffac29e60c04ec906d8d409af7fa19dc57d8c65ad167e9c4967006`  
		Last Modified: Mon, 07 Aug 2023 19:21:08 GMT  
		Size: 3.4 MB (3378609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bdca2725167af68b5a2e88c072759b23a3bf0e32c8526c7e9b89f616db5a88d`  
		Last Modified: Mon, 07 Aug 2023 20:31:39 GMT  
		Size: 279.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3a3f140b605173ff8cd3e6a398d31f3efae2350a5a0499e145583f931a911e4`  
		Last Modified: Wed, 09 Aug 2023 01:58:02 GMT  
		Size: 8.6 MB (8589935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9676915317d0ca4b6e8eab71c4b574f7733746aeb5b28e341bd7acecb71f46c1`  
		Last Modified: Wed, 09 Aug 2023 01:58:02 GMT  
		Size: 6.4 MB (6434109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3b42598376fb2ab2a87e37e7992992ebafded66021d9ba7079a8fd41d8b070b`  
		Last Modified: Wed, 09 Aug 2023 01:58:01 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb9bd2e16518ad4ff61e5eb77ffef3b5c9d336b5fc84f0310fca6883d7455c2a`  
		Last Modified: Wed, 09 Aug 2023 01:58:05 GMT  
		Size: 46.3 MB (46334322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d52f10fd03bbf4b6ea4d4dc2b178a3285f144fbe25d4a9d60336cc453cfc5e2`  
		Last Modified: Wed, 09 Aug 2023 01:58:02 GMT  
		Size: 23.1 MB (23128342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b5e76f294fdf721006a8c1f05a2753ea3c0aa007477766e76df439ac20752f9`  
		Last Modified: Wed, 09 Aug 2023 01:57:59 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e219547fcd7d310d78a64ffaca570c33363b7faa7f93eb1872c57c2c817c01d5`  
		Last Modified: Wed, 09 Aug 2023 01:57:59 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:945fba015ba45978887d983782965c16cd52f1c40031ef4318f3054579d8fa17`  
		Last Modified: Wed, 09 Aug 2023 01:57:59 GMT  
		Size: 6.6 KB (6609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:2.7.1-alpine` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:9262eb61ef1304540c4c41bbbd02856de85f9906c9cdb8a4106ca7e16baf8c6f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.8 MB (83829280 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7257778f282477b73bfadf1e535f693f6abd8275fad507d886b7b32874731cb6`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:22 GMT
ADD file:9e054a25c83111adc857a7f988336ee40eea5e1794ed30a80d465e8d472342e2 in / 
# Mon, 07 Aug 2023 19:39:22 GMT
CMD ["/bin/sh"]
# Wed, 09 Aug 2023 00:46:08 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 09 Aug 2023 00:46:10 GMT
RUN apk add --no-cache       bash       ca-certificates       curl       gnupg       run-parts       su-exec       tzdata &&     update-ca-certificates
# Wed, 09 Aug 2023 00:46:11 GMT
RUN case "$(apk --print-arch)" in       x86_64)  arch=amd64 ;;       aarch64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     curl -fLo /usr/local/bin/dasel "https://github.com/TomWright/dasel/releases/download/v2.1.2/dasel_linux_${arch}" &&     case ${arch} in       amd64) echo 'e4b43d8c7d76904e2401dc81de0900d9cb69b006794ff3901ec5d50e96baa8ef  /usr/local/bin/dasel' ;;       arm64) echo '92b83f30949679197403ff7a7e0f9ef3e458c1c55031d9c1bc112364e487d57d  /usr/local/bin/dasel' ;;     esac | sha256sum -c - &&     chmod +x /usr/local/bin/dasel &&     dasel --version
# Wed, 09 Aug 2023 00:46:12 GMT
RUN addgroup -S -g 1000 influxdb &&     adduser -S -G influxdb -u 1000 -h /home/influxdb -s /bin/sh influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Wed, 09 Aug 2023 00:46:12 GMT
ENV INFLUXDB_VERSION=2.7.1
# Wed, 09 Aug 2023 00:46:17 GMT
RUN case "$(apk --print-arch)" in       x86_64)  arch=amd64 ;;       aarch64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&    curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     cp "influxdb2_linux_${arch}/influxd" /usr/local/bin/influxd &&     rm -rf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"            "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"            "influxdb2_linux_${arch}" &&     influxd version
# Wed, 09 Aug 2023 00:46:17 GMT
ENV INFLUX_CLI_VERSION=2.7.3
# Wed, 09 Aug 2023 00:46:20 GMT
RUN case "$(apk --print-arch)" in       x86_64)  arch=amd64 ;;       aarch64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     cp influx /usr/local/bin/influx &&     rm -rf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     influx version
# Wed, 09 Aug 2023 00:46:20 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Wed, 09 Aug 2023 00:46:20 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Wed, 09 Aug 2023 00:46:20 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Wed, 09 Aug 2023 00:46:20 GMT
COPY file:0c651d5752d62a8235f9939458cdfe0447d6491e071a852d95bf87ff7179f6a0 in /entrypoint.sh 
# Wed, 09 Aug 2023 00:46:20 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 09 Aug 2023 00:46:20 GMT
CMD ["influxd"]
# Wed, 09 Aug 2023 00:46:21 GMT
EXPOSE 8086
# Wed, 09 Aug 2023 00:46:21 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Wed, 09 Aug 2023 00:46:21 GMT
ENV INFLUXD_INIT_PORT=9999
# Wed, 09 Aug 2023 00:46:21 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Wed, 09 Aug 2023 00:46:21 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:4060ece20d7ac783f52cbe28a35fd5b06f90f7b4d773bae0d956024e85ff35b6`  
		Last Modified: Mon, 07 Aug 2023 19:39:59 GMT  
		Size: 3.3 MB (3258290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bd1799839c258f2f362340c258c49aa080e354fd0e137266f54d413ef004a1b`  
		Last Modified: Wed, 09 Aug 2023 00:46:37 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f30f1a2fe004c2cdf0167c7d1f5958d25e650840e0625814e3032ecc6973f334`  
		Last Modified: Wed, 09 Aug 2023 00:46:37 GMT  
		Size: 8.5 MB (8510115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebfbe81a9d67236da8399d75342e23015e979e0e1b3e932e7e22f80f3029775b`  
		Last Modified: Wed, 09 Aug 2023 00:46:37 GMT  
		Size: 6.0 MB (5953754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:743e1b62e9110324931cfbd5f8ed76319fe9ca7c484685c263cba135e032e93b`  
		Last Modified: Wed, 09 Aug 2023 00:46:36 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c464170026f8f97d6daafd06f65bd87aa93b8a49b2a5ae5a425e111d63518b0`  
		Last Modified: Wed, 09 Aug 2023 00:46:38 GMT  
		Size: 44.4 MB (44435831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c2b153f7087828fcb85296475fd1d6882853b96d89dc6d3c0f54f82a101552d`  
		Last Modified: Wed, 09 Aug 2023 00:46:37 GMT  
		Size: 21.7 MB (21662595 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77aa542a3877dd874c5d6b906cf4de13de97e274646fb6f55e931e3a228e83f5`  
		Last Modified: Wed, 09 Aug 2023 00:46:34 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f98ade2b5c03a2d4c21d8dfe8af8d1828e19ee709483115c654fa4739935391f`  
		Last Modified: Wed, 09 Aug 2023 00:46:34 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93743bee855eb887605313e1d74fd9b3225325f9cc7f7ca18ec012d9704d8803`  
		Last Modified: Wed, 09 Aug 2023 00:46:34 GMT  
		Size: 6.6 KB (6609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:alpine`

```console
$ docker pull influxdb@sha256:e42bc2a7ab4b905183155906328d0d3a31d56eb72cd7fd8479772f6be862b873
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:8fea506e2c35f4c7a71e8d83c3607305f4f7d7cf8d5ed4ff9780752bf2bd94bd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.9 MB (87874009 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fbf8b4b940b201874dd347e8cf177667077be4e03dd67d87de6d4dacd800d195`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:26 GMT
ADD file:6dd87346b8be240b21b4f4d9296253bf0d28b6579aa52d2118872e3936963b6b in / 
# Mon, 07 Aug 2023 19:20:26 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 20:30:41 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 09 Aug 2023 01:55:45 GMT
RUN apk add --no-cache       bash       ca-certificates       curl       gnupg       run-parts       su-exec       tzdata &&     update-ca-certificates
# Wed, 09 Aug 2023 01:55:46 GMT
RUN case "$(apk --print-arch)" in       x86_64)  arch=amd64 ;;       aarch64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     curl -fLo /usr/local/bin/dasel "https://github.com/TomWright/dasel/releases/download/v2.1.2/dasel_linux_${arch}" &&     case ${arch} in       amd64) echo 'e4b43d8c7d76904e2401dc81de0900d9cb69b006794ff3901ec5d50e96baa8ef  /usr/local/bin/dasel' ;;       arm64) echo '92b83f30949679197403ff7a7e0f9ef3e458c1c55031d9c1bc112364e487d57d  /usr/local/bin/dasel' ;;     esac | sha256sum -c - &&     chmod +x /usr/local/bin/dasel &&     dasel --version
# Wed, 09 Aug 2023 01:55:47 GMT
RUN addgroup -S -g 1000 influxdb &&     adduser -S -G influxdb -u 1000 -h /home/influxdb -s /bin/sh influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Wed, 09 Aug 2023 01:55:47 GMT
ENV INFLUXDB_VERSION=2.7.1
# Wed, 09 Aug 2023 01:55:51 GMT
RUN case "$(apk --print-arch)" in       x86_64)  arch=amd64 ;;       aarch64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&    curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     cp "influxdb2_linux_${arch}/influxd" /usr/local/bin/influxd &&     rm -rf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"            "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"            "influxdb2_linux_${arch}" &&     influxd version
# Wed, 09 Aug 2023 01:55:51 GMT
ENV INFLUX_CLI_VERSION=2.7.3
# Wed, 09 Aug 2023 01:55:54 GMT
RUN case "$(apk --print-arch)" in       x86_64)  arch=amd64 ;;       aarch64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     cp influx /usr/local/bin/influx &&     rm -rf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     influx version
# Wed, 09 Aug 2023 01:55:54 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Wed, 09 Aug 2023 01:55:54 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Wed, 09 Aug 2023 01:55:54 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Wed, 09 Aug 2023 01:55:54 GMT
COPY file:0c651d5752d62a8235f9939458cdfe0447d6491e071a852d95bf87ff7179f6a0 in /entrypoint.sh 
# Wed, 09 Aug 2023 01:55:55 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 09 Aug 2023 01:55:55 GMT
CMD ["influxd"]
# Wed, 09 Aug 2023 01:55:55 GMT
EXPOSE 8086
# Wed, 09 Aug 2023 01:55:55 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Wed, 09 Aug 2023 01:55:55 GMT
ENV INFLUXD_INIT_PORT=9999
# Wed, 09 Aug 2023 01:55:55 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Wed, 09 Aug 2023 01:55:55 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:9398808236ffac29e60c04ec906d8d409af7fa19dc57d8c65ad167e9c4967006`  
		Last Modified: Mon, 07 Aug 2023 19:21:08 GMT  
		Size: 3.4 MB (3378609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bdca2725167af68b5a2e88c072759b23a3bf0e32c8526c7e9b89f616db5a88d`  
		Last Modified: Mon, 07 Aug 2023 20:31:39 GMT  
		Size: 279.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3a3f140b605173ff8cd3e6a398d31f3efae2350a5a0499e145583f931a911e4`  
		Last Modified: Wed, 09 Aug 2023 01:58:02 GMT  
		Size: 8.6 MB (8589935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9676915317d0ca4b6e8eab71c4b574f7733746aeb5b28e341bd7acecb71f46c1`  
		Last Modified: Wed, 09 Aug 2023 01:58:02 GMT  
		Size: 6.4 MB (6434109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3b42598376fb2ab2a87e37e7992992ebafded66021d9ba7079a8fd41d8b070b`  
		Last Modified: Wed, 09 Aug 2023 01:58:01 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb9bd2e16518ad4ff61e5eb77ffef3b5c9d336b5fc84f0310fca6883d7455c2a`  
		Last Modified: Wed, 09 Aug 2023 01:58:05 GMT  
		Size: 46.3 MB (46334322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d52f10fd03bbf4b6ea4d4dc2b178a3285f144fbe25d4a9d60336cc453cfc5e2`  
		Last Modified: Wed, 09 Aug 2023 01:58:02 GMT  
		Size: 23.1 MB (23128342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b5e76f294fdf721006a8c1f05a2753ea3c0aa007477766e76df439ac20752f9`  
		Last Modified: Wed, 09 Aug 2023 01:57:59 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e219547fcd7d310d78a64ffaca570c33363b7faa7f93eb1872c57c2c817c01d5`  
		Last Modified: Wed, 09 Aug 2023 01:57:59 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:945fba015ba45978887d983782965c16cd52f1c40031ef4318f3054579d8fa17`  
		Last Modified: Wed, 09 Aug 2023 01:57:59 GMT  
		Size: 6.6 KB (6609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:alpine` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:9262eb61ef1304540c4c41bbbd02856de85f9906c9cdb8a4106ca7e16baf8c6f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.8 MB (83829280 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7257778f282477b73bfadf1e535f693f6abd8275fad507d886b7b32874731cb6`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:22 GMT
ADD file:9e054a25c83111adc857a7f988336ee40eea5e1794ed30a80d465e8d472342e2 in / 
# Mon, 07 Aug 2023 19:39:22 GMT
CMD ["/bin/sh"]
# Wed, 09 Aug 2023 00:46:08 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 09 Aug 2023 00:46:10 GMT
RUN apk add --no-cache       bash       ca-certificates       curl       gnupg       run-parts       su-exec       tzdata &&     update-ca-certificates
# Wed, 09 Aug 2023 00:46:11 GMT
RUN case "$(apk --print-arch)" in       x86_64)  arch=amd64 ;;       aarch64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     curl -fLo /usr/local/bin/dasel "https://github.com/TomWright/dasel/releases/download/v2.1.2/dasel_linux_${arch}" &&     case ${arch} in       amd64) echo 'e4b43d8c7d76904e2401dc81de0900d9cb69b006794ff3901ec5d50e96baa8ef  /usr/local/bin/dasel' ;;       arm64) echo '92b83f30949679197403ff7a7e0f9ef3e458c1c55031d9c1bc112364e487d57d  /usr/local/bin/dasel' ;;     esac | sha256sum -c - &&     chmod +x /usr/local/bin/dasel &&     dasel --version
# Wed, 09 Aug 2023 00:46:12 GMT
RUN addgroup -S -g 1000 influxdb &&     adduser -S -G influxdb -u 1000 -h /home/influxdb -s /bin/sh influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Wed, 09 Aug 2023 00:46:12 GMT
ENV INFLUXDB_VERSION=2.7.1
# Wed, 09 Aug 2023 00:46:17 GMT
RUN case "$(apk --print-arch)" in       x86_64)  arch=amd64 ;;       aarch64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&    curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     cp "influxdb2_linux_${arch}/influxd" /usr/local/bin/influxd &&     rm -rf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"            "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"            "influxdb2_linux_${arch}" &&     influxd version
# Wed, 09 Aug 2023 00:46:17 GMT
ENV INFLUX_CLI_VERSION=2.7.3
# Wed, 09 Aug 2023 00:46:20 GMT
RUN case "$(apk --print-arch)" in       x86_64)  arch=amd64 ;;       aarch64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     cp influx /usr/local/bin/influx &&     rm -rf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     influx version
# Wed, 09 Aug 2023 00:46:20 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Wed, 09 Aug 2023 00:46:20 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Wed, 09 Aug 2023 00:46:20 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Wed, 09 Aug 2023 00:46:20 GMT
COPY file:0c651d5752d62a8235f9939458cdfe0447d6491e071a852d95bf87ff7179f6a0 in /entrypoint.sh 
# Wed, 09 Aug 2023 00:46:20 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 09 Aug 2023 00:46:20 GMT
CMD ["influxd"]
# Wed, 09 Aug 2023 00:46:21 GMT
EXPOSE 8086
# Wed, 09 Aug 2023 00:46:21 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Wed, 09 Aug 2023 00:46:21 GMT
ENV INFLUXD_INIT_PORT=9999
# Wed, 09 Aug 2023 00:46:21 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Wed, 09 Aug 2023 00:46:21 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:4060ece20d7ac783f52cbe28a35fd5b06f90f7b4d773bae0d956024e85ff35b6`  
		Last Modified: Mon, 07 Aug 2023 19:39:59 GMT  
		Size: 3.3 MB (3258290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bd1799839c258f2f362340c258c49aa080e354fd0e137266f54d413ef004a1b`  
		Last Modified: Wed, 09 Aug 2023 00:46:37 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f30f1a2fe004c2cdf0167c7d1f5958d25e650840e0625814e3032ecc6973f334`  
		Last Modified: Wed, 09 Aug 2023 00:46:37 GMT  
		Size: 8.5 MB (8510115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebfbe81a9d67236da8399d75342e23015e979e0e1b3e932e7e22f80f3029775b`  
		Last Modified: Wed, 09 Aug 2023 00:46:37 GMT  
		Size: 6.0 MB (5953754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:743e1b62e9110324931cfbd5f8ed76319fe9ca7c484685c263cba135e032e93b`  
		Last Modified: Wed, 09 Aug 2023 00:46:36 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c464170026f8f97d6daafd06f65bd87aa93b8a49b2a5ae5a425e111d63518b0`  
		Last Modified: Wed, 09 Aug 2023 00:46:38 GMT  
		Size: 44.4 MB (44435831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c2b153f7087828fcb85296475fd1d6882853b96d89dc6d3c0f54f82a101552d`  
		Last Modified: Wed, 09 Aug 2023 00:46:37 GMT  
		Size: 21.7 MB (21662595 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77aa542a3877dd874c5d6b906cf4de13de97e274646fb6f55e931e3a228e83f5`  
		Last Modified: Wed, 09 Aug 2023 00:46:34 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f98ade2b5c03a2d4c21d8dfe8af8d1828e19ee709483115c654fa4739935391f`  
		Last Modified: Wed, 09 Aug 2023 00:46:34 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93743bee855eb887605313e1d74fd9b3225325f9cc7f7ca18ec012d9704d8803`  
		Last Modified: Wed, 09 Aug 2023 00:46:34 GMT  
		Size: 6.6 KB (6609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:latest`

```console
$ docker pull influxdb@sha256:17390018173e18a8b7d0c3c6495a6cc066a82295084d7a427dd32ea2c5928d4a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:latest` - linux; amd64

```console
$ docker pull influxdb@sha256:e970833ae6d02fe0833367b3fbf8a5c30b881931d1e300ecea4341d8e50a1221
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.6 MB (114639373 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6921cbed08d00461f99a782670f83c8808fa70077c2b33dee20d583a57ac6e50`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Thu, 07 Sep 2023 00:21:13 GMT
ADD file:cb5fcc80c057b356a31492a20c6e3a75b70ed70a663506c8e97ad730ae32a02d in / 
# Thu, 07 Sep 2023 00:21:13 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 01:40:15 GMT
RUN export DEBIAN_FRONTEND=noninteractive &&     apt-get update -y &&     apt-get install -y --no-install-recommends       ca-certificates       curl       gnupg &&     apt-get clean &&     rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 01:40:16 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     curl -fLo /usr/local/bin/dasel "https://github.com/TomWright/dasel/releases/download/v2.1.2/dasel_linux_${arch}" &&     case ${arch} in       amd64) echo 'e4b43d8c7d76904e2401dc81de0900d9cb69b006794ff3901ec5d50e96baa8ef  /usr/local/bin/dasel' ;;       arm64) echo '92b83f30949679197403ff7a7e0f9ef3e458c1c55031d9c1bc112364e487d57d  /usr/local/bin/dasel' ;;     esac | sha256sum -c - &&     chmod +x /usr/local/bin/dasel &&     dasel --version
# Thu, 07 Sep 2023 01:40:17 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --create-home --home-dir=/home/influxdb --shell=/bin/bash influxdb
# Thu, 07 Sep 2023 01:40:17 GMT
ENV GOSU_VER=1.12
# Thu, 07 Sep 2023 01:40:19 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       B42F6819007F00F88E364FD4036A9C25BF357DD4 &&     curl -fLo /usr/local/bin/gosu     "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-${arch}"          -fLo /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-${arch}.asc" &&     gpg --batch --verify /usr/local/bin/gosu.asc                          /usr/local/bin/gosu &&     rm -rf /usr/local/bin/gosu.asc &&     chmod +x /usr/local/bin/gosu &&     gosu --version &&     gosu nobody true
# Thu, 07 Sep 2023 01:40:19 GMT
ENV INFLUXDB_VERSION=2.7.1
# Thu, 07 Sep 2023 01:40:23 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     cp "influxdb2_linux_${arch}/influxd" /usr/local/bin/influxd &&     rm -rf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"            "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"            "influxdb2_linux_${arch}" &&     influxd version
# Thu, 07 Sep 2023 01:40:23 GMT
ENV INFLUX_CLI_VERSION=2.7.3
# Thu, 07 Sep 2023 01:40:25 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     cp influx /usr/local/bin/influx &&     rm -rf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     influx version
# Thu, 07 Sep 2023 01:40:26 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Thu, 07 Sep 2023 01:40:26 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Thu, 07 Sep 2023 01:40:26 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Thu, 07 Sep 2023 01:40:26 GMT
COPY file:3ef80d0bcfdeda3282c98ad7a6b84218cd7593d6a3bbf027c3083db3b7acad32 in /entrypoint.sh 
# Thu, 07 Sep 2023 01:40:26 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 07 Sep 2023 01:40:26 GMT
CMD ["influxd"]
# Thu, 07 Sep 2023 01:40:26 GMT
EXPOSE 8086
# Thu, 07 Sep 2023 01:40:26 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Thu, 07 Sep 2023 01:40:26 GMT
ENV INFLUXD_INIT_PORT=9999
# Thu, 07 Sep 2023 01:40:27 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Thu, 07 Sep 2023 01:40:27 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:7d97e254a0461b0a30b3f443f1daa0d620a3cc6ff4e2714cc1cfd96ace5b7a7e`  
		Last Modified: Thu, 07 Sep 2023 00:26:03 GMT  
		Size: 31.4 MB (31417503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1768238c1d21edcca065dcc4e383b02cac745ff7e9a01c9c82dde121aad8db12`  
		Last Modified: Thu, 07 Sep 2023 01:41:18 GMT  
		Size: 6.3 MB (6327853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a8cf89659e591ba916aa2258a818d30c11630eebc07d2b7426f788db5153402`  
		Last Modified: Thu, 07 Sep 2023 01:41:16 GMT  
		Size: 6.4 MB (6434102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bbbd9ea79cb9c17df3e62a72623699b0f865b231433805f803e80f2f9f56653`  
		Last Modified: Thu, 07 Sep 2023 01:41:15 GMT  
		Size: 4.1 KB (4114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f5bace44f952cfb244599835428862f45f33378893152e887d7a30172b1a048`  
		Last Modified: Thu, 07 Sep 2023 01:41:16 GMT  
		Size: 986.0 KB (985990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cac023e05c09814a2525011e7dca324d1250dd751e504ac730bd204054e916a2`  
		Last Modified: Thu, 07 Sep 2023 01:41:19 GMT  
		Size: 46.3 MB (46334319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eda2b107f008112ca1bd7bc6cce9ba6598e04bdbe0a7e32899d77ce7393cef5b`  
		Last Modified: Thu, 07 Sep 2023 01:41:16 GMT  
		Size: 23.1 MB (23128343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4792803ad3fdb0f7c42ea7612417b7ea4474a31f785fd2cca132bc54d4859f1d`  
		Last Modified: Thu, 07 Sep 2023 01:41:13 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18438cd9981878262b7f8f9151fba89f3e02a7a6fc0d3260749f2309a1a85456`  
		Last Modified: Thu, 07 Sep 2023 01:41:13 GMT  
		Size: 261.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0458408b9bdf79125c7d02ab7f75816379a4061341ed2ad631a0e06e7efbf31a`  
		Last Modified: Thu, 07 Sep 2023 01:41:13 GMT  
		Size: 6.6 KB (6612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:latest` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:507a6e517b68c2621e9bf4c716314fd3301f22f1e638a54259548d80c6cbad2a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.4 MB (109356541 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e21e8f1eba2f968cb42868da326aa2e29978c5b298c7565bc3033bdd316f68c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Thu, 07 Sep 2023 00:39:53 GMT
ADD file:abd1ad48ae3ebec7a6ecc8ce3016c25be2afcbaedfcb904bc89b1ce59400aef0 in / 
# Thu, 07 Sep 2023 00:39:54 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 05:36:03 GMT
RUN export DEBIAN_FRONTEND=noninteractive &&     apt-get update -y &&     apt-get install -y --no-install-recommends       ca-certificates       curl       gnupg &&     apt-get clean &&     rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 05:36:04 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     curl -fLo /usr/local/bin/dasel "https://github.com/TomWright/dasel/releases/download/v2.1.2/dasel_linux_${arch}" &&     case ${arch} in       amd64) echo 'e4b43d8c7d76904e2401dc81de0900d9cb69b006794ff3901ec5d50e96baa8ef  /usr/local/bin/dasel' ;;       arm64) echo '92b83f30949679197403ff7a7e0f9ef3e458c1c55031d9c1bc112364e487d57d  /usr/local/bin/dasel' ;;     esac | sha256sum -c - &&     chmod +x /usr/local/bin/dasel &&     dasel --version
# Thu, 07 Sep 2023 05:36:04 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --create-home --home-dir=/home/influxdb --shell=/bin/bash influxdb
# Thu, 07 Sep 2023 05:36:05 GMT
ENV GOSU_VER=1.12
# Thu, 07 Sep 2023 05:36:07 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       B42F6819007F00F88E364FD4036A9C25BF357DD4 &&     curl -fLo /usr/local/bin/gosu     "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-${arch}"          -fLo /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-${arch}.asc" &&     gpg --batch --verify /usr/local/bin/gosu.asc                          /usr/local/bin/gosu &&     rm -rf /usr/local/bin/gosu.asc &&     chmod +x /usr/local/bin/gosu &&     gosu --version &&     gosu nobody true
# Thu, 07 Sep 2023 05:36:07 GMT
ENV INFLUXDB_VERSION=2.7.1
# Thu, 07 Sep 2023 05:36:10 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     cp "influxdb2_linux_${arch}/influxd" /usr/local/bin/influxd &&     rm -rf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"            "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"            "influxdb2_linux_${arch}" &&     influxd version
# Thu, 07 Sep 2023 05:36:11 GMT
ENV INFLUX_CLI_VERSION=2.7.3
# Thu, 07 Sep 2023 05:36:13 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     cp influx /usr/local/bin/influx &&     rm -rf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     influx version
# Thu, 07 Sep 2023 05:36:13 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Thu, 07 Sep 2023 05:36:14 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Thu, 07 Sep 2023 05:36:14 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Thu, 07 Sep 2023 05:36:14 GMT
COPY file:3ef80d0bcfdeda3282c98ad7a6b84218cd7593d6a3bbf027c3083db3b7acad32 in /entrypoint.sh 
# Thu, 07 Sep 2023 05:36:14 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 07 Sep 2023 05:36:14 GMT
CMD ["influxd"]
# Thu, 07 Sep 2023 05:36:14 GMT
EXPOSE 8086
# Thu, 07 Sep 2023 05:36:14 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Thu, 07 Sep 2023 05:36:14 GMT
ENV INFLUXD_INIT_PORT=9999
# Thu, 07 Sep 2023 05:36:14 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Thu, 07 Sep 2023 05:36:14 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:f96ab15157043879c2ff23e0556e798eba6a6ff3d7fd5d1384de223bb9f66f1d`  
		Last Modified: Thu, 07 Sep 2023 00:43:41 GMT  
		Size: 30.1 MB (30062903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4abaa895672d07010025a3b438860c732da8a8fccf5dc335a51544fb9025cb95`  
		Last Modified: Thu, 07 Sep 2023 05:36:34 GMT  
		Size: 6.3 MB (6308767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65064d89682d695ed1fdcba8c6b740dd5caae58affe7d753a10a50292efe0d74`  
		Last Modified: Thu, 07 Sep 2023 05:36:32 GMT  
		Size: 6.0 MB (5953765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39608a77e87221c0d4137100cf52ab41b759d953066b2d53aadba26f6e330d06`  
		Last Modified: Thu, 07 Sep 2023 05:36:31 GMT  
		Size: 4.1 KB (4117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8905172f7f9cdd2432cc2f4ab6a11a6a5672939d05a15161091999a0303bb6e`  
		Last Modified: Thu, 07 Sep 2023 05:36:31 GMT  
		Size: 921.5 KB (921471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c99241f70a82d0cca3a38168ab21d0af633024521dac2d196ec22d78d197ac2`  
		Last Modified: Thu, 07 Sep 2023 05:36:33 GMT  
		Size: 44.4 MB (44435781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e34b1ef8e734d97f099114726a375d0365254557f9002c294cf6a398913bfbfc`  
		Last Modified: Thu, 07 Sep 2023 05:36:31 GMT  
		Size: 21.7 MB (21662588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66dae31c3c2091ed8fdb0d77cf7e6fa44c894fbdf33d7568eb1642b69ff1600e`  
		Last Modified: Thu, 07 Sep 2023 05:36:29 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc8f1f5a6f744a26d73cb07dbf19389e31ee3cab6680b9910baf148c9f5a4d05`  
		Last Modified: Thu, 07 Sep 2023 05:36:29 GMT  
		Size: 261.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f81d55cc75ef9ca2dc5e20c1e1b9cecd2d4080cbdbbb77a18c9a6700a93ab32`  
		Last Modified: Thu, 07 Sep 2023 05:36:29 GMT  
		Size: 6.6 KB (6612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
