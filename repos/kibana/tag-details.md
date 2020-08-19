<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `kibana`

-	[`kibana:6.8.12`](#kibana6812)
-	[`kibana:7.9.0`](#kibana790)

## `kibana:6.8.12`

```console
$ docker pull kibana@sha256:b82ddf3ba69ea030702993a368306a744ca532347d2d00f21b4f6439ab64bb0e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kibana:6.8.12` - linux; amd64

```console
$ docker pull kibana@sha256:6b4d3c1a8b6e3eaaedfd3d81637a273877355b17938f41954f46fcaba788b756
```

-	Docker Version: 19.03.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **275.8 MB (275759911 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4227d845381f42d8884c0fe00099691efe653d6679976a632ed66410a935c9de`
-	Default Command: `["\/usr\/local\/bin\/kibana-docker"]`

```dockerfile
# Mon, 10 Aug 2020 18:20:08 GMT
ADD file:61908381d3142ffba798ae9a904476d19b197ab79d0338f14bec0f76649df8d4 in / 
# Mon, 10 Aug 2020 18:20:09 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20200809 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-08-09 00:00:00+01:00
# Mon, 10 Aug 2020 18:20:09 GMT
CMD ["/bin/bash"]
# Wed, 12 Aug 2020 08:18:33 GMT
EXPOSE 5601
# Wed, 12 Aug 2020 08:18:46 GMT
RUN yum update -y && yum install -y fontconfig freetype && yum clean all
# Wed, 12 Aug 2020 08:19:32 GMT
COPY --chown=1000:0dir:aaf12d5b2b623394c1178c4c2bb82e74abe0db0ddb95a085c41446962b4a2fea in /usr/share/kibana 
# Wed, 12 Aug 2020 08:19:33 GMT
WORKDIR /usr/share/kibana
# Wed, 12 Aug 2020 08:19:38 GMT
RUN ln -s /usr/share/kibana /opt/kibana
# Wed, 12 Aug 2020 08:19:38 GMT
ENV ELASTIC_CONTAINER=true
# Wed, 12 Aug 2020 08:19:38 GMT
ENV PATH=/usr/share/kibana/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 Aug 2020 08:19:39 GMT
COPY --chown=1000:0file:60b6181f28c99b362092ea6139b6d4112ddd0bef32d52563c33b26bdc2b51318 in /usr/share/kibana/config/kibana.yml 
# Wed, 12 Aug 2020 08:19:39 GMT
COPY --chown=1000:0file:7d472d1939e23e2f10e7c5fd1e9166eefd646214aa0d8a1c09d92af71c9cbd87 in /usr/local/bin/ 
# Wed, 12 Aug 2020 08:19:42 GMT
RUN chmod g+ws /usr/share/kibana && find /usr/share/kibana -gid 0 -and -not -perm /g+w -exec chmod g+w {} \;
# Wed, 12 Aug 2020 08:19:44 GMT
RUN groupadd --gid 1000 kibana && useradd --uid 1000 --gid 1000 --home-dir /usr/share/kibana --no-create-home kibana
# Wed, 12 Aug 2020 08:19:44 GMT
USER kibana
# Wed, 12 Aug 2020 08:19:45 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.vendor=Elastic org.label-schema.name=kibana org.label-schema.version=6.8.12 org.label-schema.url=https://www.elastic.co/products/kibana org.label-schema.vcs-url=https://github.com/elastic/kibana org.label-schema.license=Elastic License license=Elastic License
# Wed, 12 Aug 2020 08:19:45 GMT
CMD ["/usr/local/bin/kibana-docker"]
```

-	Layers:
	-	`sha256:75f829a71a1c5277a7abf55495ac8d16759691d980bf1d931795e5eb68a294c0`  
		Last Modified: Mon, 10 Aug 2020 18:21:46 GMT  
		Size: 75.9 MB (75863188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ae3692e2bce8770380160b51df0a5e91a2858ea47e542c9b973e93064b95356`  
		Last Modified: Wed, 19 Aug 2020 21:36:38 GMT  
		Size: 10.0 MB (9978517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:932a0bf8c03a6542c0ac8a560daaf7f752df4089bc798a2dde560ae30e37134f`  
		Last Modified: Wed, 19 Aug 2020 21:37:15 GMT  
		Size: 189.9 MB (189913467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6acea4293b251dff6ff3f3efa114856c0b2d0ef12ead303b45eefb5735bcfb09`  
		Last Modified: Wed, 19 Aug 2020 21:36:34 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bd647c0da003b3d0e5c904f7547c9f91ed7237654caa99af3079a59df7aae9c`  
		Last Modified: Wed, 19 Aug 2020 21:36:34 GMT  
		Size: 392.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c126949930cea80b9b663a44838654d557054de4765c5ccae77405623a6fe09`  
		Last Modified: Wed, 19 Aug 2020 21:36:34 GMT  
		Size: 2.3 KB (2257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1319ec5a92666214bb9da7dc210375a7c5366402545edf38aa035d4d78d57a1`  
		Last Modified: Wed, 19 Aug 2020 21:36:34 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37183b6c21cce0d08cda644ca1fc67ac1eee89721065b07a569d5548e52a5890`  
		Last Modified: Wed, 19 Aug 2020 21:36:34 GMT  
		Size: 1.8 KB (1811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kibana:7.9.0`

```console
$ docker pull kibana@sha256:3c862af59a293645b669dc12d98500316c6ac099f560f7f5822fb2444be1aa94
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kibana:7.9.0` - linux; amd64

```console
$ docker pull kibana@sha256:3945265d00733d5e9c6254fc9f4af6dc1ca2e6efc74351bf4bb855af5b6bfead
```

-	Docker Version: 19.03.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **385.9 MB (385903790 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f6c0975b6473c9c29a9cc8b267ab9e97e6c6ce2e9e1776f387566be40cb7f33`
-	Entrypoint: `["\/usr\/local\/bin\/dumb-init","--"]`
-	Default Command: `["\/usr\/local\/bin\/kibana-docker"]`

```dockerfile
# Mon, 10 Aug 2020 18:20:08 GMT
ADD file:61908381d3142ffba798ae9a904476d19b197ab79d0338f14bec0f76649df8d4 in / 
# Mon, 10 Aug 2020 18:20:09 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20200809 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-08-09 00:00:00+01:00
# Mon, 10 Aug 2020 18:20:09 GMT
CMD ["/bin/bash"]
# Tue, 11 Aug 2020 23:03:36 GMT
EXPOSE 5601
# Tue, 11 Aug 2020 23:03:49 GMT
RUN yum update -y && yum install -y fontconfig freetype shadow-utils && yum clean all
# Tue, 11 Aug 2020 23:03:52 GMT
RUN curl -L -o /usr/local/bin/dumb-init https://github.com/Yelp/dumb-init/releases/download/v1.2.2/dumb-init_1.2.2_amd64
# Tue, 11 Aug 2020 23:03:57 GMT
RUN echo "37f2c1f0372a45554f1b89924fbb134fc24c3756efaedf11e07f599494e0eff9  /usr/local/bin/dumb-init" | sha256sum -c -
# Tue, 11 Aug 2020 23:03:59 GMT
RUN chmod +x /usr/local/bin/dumb-init
# Tue, 11 Aug 2020 23:05:31 GMT
COPY --chown=1000:0dir:b67937f93fdd7c51eb52c6a6b2e8588014e6ad525375fb9706ea370b059cc802 in /usr/share/kibana 
# Tue, 11 Aug 2020 23:05:34 GMT
WORKDIR /usr/share/kibana
# Tue, 11 Aug 2020 23:05:36 GMT
RUN ln -s /usr/share/kibana /opt/kibana
# Tue, 11 Aug 2020 23:05:36 GMT
ENV ELASTIC_CONTAINER=true
# Tue, 11 Aug 2020 23:05:37 GMT
ENV PATH=/usr/share/kibana/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 11 Aug 2020 23:05:37 GMT
COPY --chown=1000:0file:ea1f294356f14dfc1a50e3303613e69f187589962058569d5b3282460d7f28cb in /usr/share/kibana/config/kibana.yml 
# Tue, 11 Aug 2020 23:05:37 GMT
COPY --chown=1000:0file:e6ed2bdd7e66442401f740a3f75cd7792da59a22af03c368d3b73796feeb80d4 in /usr/local/bin/ 
# Tue, 11 Aug 2020 23:05:40 GMT
RUN chmod g+ws /usr/share/kibana && find /usr/share/kibana -gid 0 -and -not -perm /g+w -exec chmod g+w {} \;
# Tue, 11 Aug 2020 23:05:43 GMT
RUN find / -xdev -perm -4000 -exec chmod u-s {} +
# Tue, 11 Aug 2020 23:05:46 GMT
RUN groupadd --gid 1000 kibana && useradd --uid 1000 --gid 1000 --home-dir /usr/share/kibana --no-create-home kibana
# Tue, 11 Aug 2020 23:05:47 GMT
USER kibana
# Tue, 11 Aug 2020 23:05:47 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.vendor=Elastic org.label-schema.name=kibana org.label-schema.version=7.9.0 org.label-schema.url=https://www.elastic.co/products/kibana org.label-schema.vcs-url=https://github.com/elastic/kibana org.label-schema.license=Elastic License org.label-schema.usage=https://www.elastic.co/guide/en/kibana/index.html org.label-schema.build-date=2020-08-11T22:59:37.145Z license=Elastic License
# Tue, 11 Aug 2020 23:05:48 GMT
ENTRYPOINT ["/usr/local/bin/dumb-init" "--"]
# Tue, 11 Aug 2020 23:05:48 GMT
CMD ["/usr/local/bin/kibana-docker"]
```

-	Layers:
	-	`sha256:75f829a71a1c5277a7abf55495ac8d16759691d980bf1d931795e5eb68a294c0`  
		Last Modified: Mon, 10 Aug 2020 18:21:46 GMT  
		Size: 75.9 MB (75863188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c12ff40b598fa090c482a9b7f28a26d91a0a5fa0f3b857cb46ddf613cb5d0b55`  
		Last Modified: Tue, 18 Aug 2020 21:38:13 GMT  
		Size: 10.0 MB (9980294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a9b41b6987c2b52228e0a64c4b155593a4c477905e31c4a20fe53fdf7b09eaa`  
		Last Modified: Tue, 18 Aug 2020 21:38:10 GMT  
		Size: 31.7 KB (31686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c6d6755776a61c3c7b0316ddcab852c0ade8feb74f3753727b6cfd4d34e2226`  
		Last Modified: Tue, 18 Aug 2020 21:38:10 GMT  
		Size: 30.2 KB (30192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a6eeb2ae3e3ba450b9f5aa4248bc8fd8f4aea7c527e7534f93adda7098b9ab6`  
		Last Modified: Wed, 19 Aug 2020 21:36:30 GMT  
		Size: 299.8 MB (299792320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5172362ef8a284dc5d97a8079720f3591255cb747829b8f3121354ca0f65994`  
		Last Modified: Wed, 19 Aug 2020 21:35:16 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88d5c9b4212464d3dafad5905fd7633696b64660c5d611a4add44f2caad9b905`  
		Last Modified: Wed, 19 Aug 2020 21:35:15 GMT  
		Size: 385.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d01865fddf2f19548acf7489b0ef128cb529e6856e8458ad2e2cbefb6b68bd5f`  
		Last Modified: Wed, 19 Aug 2020 21:35:16 GMT  
		Size: 3.0 KB (3024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa818bacfab61d1255a224ea26f2e7839c025dba79d389cb9b39f43785dbe049`  
		Last Modified: Wed, 19 Aug 2020 21:35:15 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcd37bbbf3c653db4b72a03e483522d83e101093a4daca26c25d26a0becdd0bb`  
		Last Modified: Tue, 18 Aug 2020 21:38:07 GMT  
		Size: 200.6 KB (200608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67fb41c0d0e2cf3470e5b7515bfcb15a19baf65e5d9a3519604c40c95c9f3f00`  
		Last Modified: Wed, 19 Aug 2020 21:35:15 GMT  
		Size: 1.8 KB (1813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
