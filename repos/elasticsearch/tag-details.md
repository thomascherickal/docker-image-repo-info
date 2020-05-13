<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `elasticsearch`

-	[`elasticsearch:6.8.9`](#elasticsearch689)
-	[`elasticsearch:7.7.0`](#elasticsearch770)

## `elasticsearch:6.8.9`

```console
$ docker pull elasticsearch@sha256:4f38f1f2e0f5cc6666b8f965fe7157502d07ce76c95ed7e6f9ad043bf42a96cd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `elasticsearch:6.8.9` - linux; amd64

```console
$ docker pull elasticsearch@sha256:2f83ea3ff5c72b3459e535797aa63a1a3ce6006e85953a00e80605176ebd31df
```

-	Docker Version: 19.03.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **500.2 MB (500194277 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f057ebddf832dc6a5f463eb941c17e9d218090b623e21dcb530b4e0fe134c5f2`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["eswrapper"]`

```dockerfile
# Tue, 12 Nov 2019 00:20:33 GMT
ADD file:45a381049c52b5664e5e911dead277b25fadbae689c0bb35be3c42dff0f2dffe in / 
# Tue, 12 Nov 2019 00:20:33 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20191001
# Tue, 12 Nov 2019 00:20:33 GMT
CMD ["/bin/bash"]
# Mon, 04 May 2020 17:06:05 GMT
ENV ELASTIC_CONTAINER=true
# Mon, 04 May 2020 17:06:05 GMT
ENV JAVA_HOME=/opt/jdk-14+36
# Mon, 04 May 2020 17:06:13 GMT
COPY dir:2a7b0465219886ee3c466980289fa8f28d70f58035a0c65f440be7c461e6cb1b in /opt/jdk-14+36 
# Mon, 04 May 2020 17:07:40 GMT
RUN for iter in {1..10}; do yum update  --setopt=tsflags=nodocs -y &&     yum install -y  --setopt=tsflags=nodocs nc unzip wget which &&     yum clean all && exit_code=0 && break || exit_code=\$? && echo "yum error: retry $iter in 10s" && sleep 10; done;     (exit $exit_code)
# Mon, 04 May 2020 17:07:43 GMT
RUN groupadd -g 1000 elasticsearch &&     adduser -u 1000 -g 1000 -G 0 -d /usr/share/elasticsearch elasticsearch &&     chmod 0775 /usr/share/elasticsearch &&     chgrp 0 /usr/share/elasticsearch
# Mon, 04 May 2020 17:07:44 GMT
WORKDIR /usr/share/elasticsearch
# Mon, 04 May 2020 17:07:49 GMT
COPY --chown=1000:0dir:e9ddf48c14c84e788357a873afc2c5725ddd90fe6a8257ba0d82588cb69f16a9 in /usr/share/elasticsearch 
# Mon, 04 May 2020 17:07:49 GMT
ENV PATH=/usr/share/elasticsearch/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 04 May 2020 17:07:50 GMT
COPY --chown=1000:0file:08193f849fc25f29db1438eff6d5c9fe1d63237aeb07a3e0009e8ba554f97c31 in /usr/local/bin/docker-entrypoint.sh 
# Mon, 04 May 2020 17:07:52 GMT
RUN chgrp 0 /usr/local/bin/docker-entrypoint.sh &&     chmod g=u /etc/passwd &&     chmod 0775 /usr/local/bin/docker-entrypoint.sh
# Mon, 04 May 2020 17:07:53 GMT
EXPOSE 9200 9300
# Mon, 04 May 2020 17:07:54 GMT
LABEL org.label-schema.build-date=2020-05-04T17:00:34.323820Z org.label-schema.license=Elastic-License org.label-schema.name=Elasticsearch org.label-schema.schema-version=1.0 org.label-schema.url=https://www.elastic.co/products/elasticsearch org.label-schema.usage=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.label-schema.vcs-ref=be2c7bf0f8427387e84c68ad8d2d9abbc60a64da org.label-schema.vcs-url=https://github.com/elastic/elasticsearch org.label-schema.vendor=Elastic org.label-schema.version=6.8.9 org.opencontainers.image.created=2020-05-04T17:00:34.323820Z org.opencontainers.image.documentation=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.opencontainers.image.licenses=Elastic-License org.opencontainers.image.revision=be2c7bf0f8427387e84c68ad8d2d9abbc60a64da org.opencontainers.image.source=https://github.com/elastic/elasticsearch org.opencontainers.image.title=Elasticsearch org.opencontainers.image.url=https://www.elastic.co/products/elasticsearch org.opencontainers.image.vendor=Elastic org.opencontainers.image.version=6.8.9
# Mon, 04 May 2020 17:07:54 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Mon, 04 May 2020 17:07:54 GMT
CMD ["eswrapper"]
```

-	Layers:
	-	`sha256:ab5ef0e5819490abe86106fd9f4381123e37a03e80e650be39f7938d30ecb530`  
		Last Modified: Tue, 12 Nov 2019 00:23:38 GMT  
		Size: 75.8 MB (75780712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82c6075c8485d68950491217271a4b5e1761091463122d9ace4ef02fc11f5a0d`  
		Last Modified: Wed, 13 May 2020 14:57:46 GMT  
		Size: 217.3 MB (217331890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:013653038408c7606950eedf78df7fc9b89d759eedf65f9452e2247ac18de65b`  
		Last Modified: Wed, 13 May 2020 14:57:36 GMT  
		Size: 56.1 MB (56118365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68d00c8bb084a5b215a04c03627f240f29a4f1524c60e562883d8579c4d85d72`  
		Last Modified: Wed, 13 May 2020 14:57:08 GMT  
		Size: 2.3 KB (2278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdb2603bc306a75102eb4c1e375e71c92fa6e134e0293679188b9bae208227d0`  
		Last Modified: Wed, 13 May 2020 14:57:34 GMT  
		Size: 151.0 MB (150956572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48a4070ba159ea3e891020c295eae7087e2929b28a2faf51e6e7813931cdb40c`  
		Last Modified: Wed, 13 May 2020 14:57:06 GMT  
		Size: 2.1 KB (2061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:735876063771fcffa0e27be0e33d56d6d59b369745256cb7f637266ff8c66b74`  
		Last Modified: Wed, 13 May 2020 14:57:06 GMT  
		Size: 2.4 KB (2399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `elasticsearch:7.7.0`

```console
$ docker pull elasticsearch@sha256:ce6d341f95af5c1fdefae53789d92b6dd978f605ade2eea41381162d21c9f938
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `elasticsearch:7.7.0` - linux; amd64

```console
$ docker pull elasticsearch@sha256:e93505e5a277480995bd682b8e0e91e16deba9dd6b190015c48134eff519f15a
```

-	Docker Version: 19.03.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **399.5 MB (399519981 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ec4f35ab452cc25d01d9db6b89cbbd5a7ca37eb1f35017b50377874cd08a83e`
-	Entrypoint: `["\/tini","--","\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["eswrapper"]`

```dockerfile
# Tue, 05 May 2020 21:20:06 GMT
ADD file:38e2d2a1a0cd8694bd5086f257fdf7504f0c2481bf4f746c9bd1c8d9f3f6430d in / 
# Tue, 05 May 2020 21:20:06 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20200504 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-05-04 00:00:00+01:00
# Tue, 05 May 2020 21:20:07 GMT
CMD ["/bin/bash"]
# Tue, 12 May 2020 02:06:02 GMT
ENV ELASTIC_CONTAINER=true
# Tue, 12 May 2020 02:06:03 GMT
COPY file:df9158ae8b9b283e8ea5bd72d1e344c08dea733e283f9f0941833f467466323c in /tini 
# Tue, 12 May 2020 02:06:25 GMT
RUN for iter in {1..10}; do yum update --setopt=tsflags=nodocs -y &&     yum install --setopt=tsflags=nodocs -y nc shadow-utils zip unzip &&     yum clean all && exit_code=0 && break || exit_code=$? && echo "yum error: retry $iter in 10s" && sleep 10; done;     (exit $exit_code)
# Tue, 12 May 2020 02:06:27 GMT
RUN groupadd -g 1000 elasticsearch &&     adduser -u 1000 -g 1000 -G 0 -d /usr/share/elasticsearch elasticsearch &&     chmod 0775 /usr/share/elasticsearch &&     chgrp 0 /usr/share/elasticsearch
# Tue, 12 May 2020 02:06:28 GMT
WORKDIR /usr/share/elasticsearch
# Tue, 12 May 2020 02:06:37 GMT
COPY --chown=1000:0dir:bed49b52ff66beec2cce7072b72192865f48507f32d5ce0f85aa38f10129fbdb in /usr/share/elasticsearch 
# Tue, 12 May 2020 02:06:39 GMT
RUN ln -sf /etc/pki/ca-trust/extracted/java/cacerts /usr/share/elasticsearch/jdk/lib/security/cacerts
# Tue, 12 May 2020 02:06:40 GMT
ENV PATH=/usr/share/elasticsearch/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 May 2020 02:06:41 GMT
COPY file:d964df1452418918baf1d29ee20df18c9648ca6c9d51764640fca470bd9a9366 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 12 May 2020 02:06:44 GMT
RUN chmod g=u /etc/passwd &&     chmod 0775 /usr/local/bin/docker-entrypoint.sh
# Tue, 12 May 2020 02:06:45 GMT
RUN find / -xdev -perm -4000 -exec chmod ug-s {} +
# Tue, 12 May 2020 02:06:46 GMT
EXPOSE 9200 9300
# Tue, 12 May 2020 02:06:46 GMT
LABEL org.label-schema.build-date=2020-05-12T02:01:37.602180Z org.label-schema.license=Elastic-License org.label-schema.name=Elasticsearch org.label-schema.schema-version=1.0 org.label-schema.url=https://www.elastic.co/products/elasticsearch org.label-schema.usage=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.label-schema.vcs-ref=81a1e9eda8e6183f5237786246f6dced26a10eaf org.label-schema.vcs-url=https://github.com/elastic/elasticsearch org.label-schema.vendor=Elastic org.label-schema.version=7.7.0 org.opencontainers.image.created=2020-05-12T02:01:37.602180Z org.opencontainers.image.documentation=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.opencontainers.image.licenses=Elastic-License org.opencontainers.image.revision=81a1e9eda8e6183f5237786246f6dced26a10eaf org.opencontainers.image.source=https://github.com/elastic/elasticsearch org.opencontainers.image.title=Elasticsearch org.opencontainers.image.url=https://www.elastic.co/products/elasticsearch org.opencontainers.image.vendor=Elastic org.opencontainers.image.version=7.7.0
# Tue, 12 May 2020 02:06:46 GMT
ENTRYPOINT ["/tini" "--" "/usr/local/bin/docker-entrypoint.sh"]
# Tue, 12 May 2020 02:06:46 GMT
CMD ["eswrapper"]
```

-	Layers:
	-	`sha256:524b0c1e57f8ee5fee01a1decba2f301c324a6513ca3551021264e3aa7341ebc`  
		Last Modified: Tue, 05 May 2020 21:23:14 GMT  
		Size: 75.9 MB (75880141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f79045bc94aaaa1467cc2932e15d52087c3764c7f2c96e3576db0bf8cf1a339`  
		Last Modified: Wed, 06 May 2020 14:38:52 GMT  
		Size: 9.5 KB (9461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bfd159f5e061f248db32430920e0cb7407630e5c374686e5cbe45f69fe90cd0`  
		Last Modified: Wed, 13 May 2020 14:09:00 GMT  
		Size: 7.2 MB (7249743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e00e3b68a1583803a5afe8a8f8b3fea96c4aa187855da45e905b3d6c65e8150d`  
		Last Modified: Wed, 13 May 2020 14:08:59 GMT  
		Size: 2.3 KB (2279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33b005156da627fcd66e0492f44ca40809e77bbe4bbf3e8b1886aa7786a4d917`  
		Last Modified: Wed, 13 May 2020 14:09:24 GMT  
		Size: 316.2 MB (316173676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4bd472226801e3376c42e2dfa13db3847bd6953db87069ebc80d82e6f6f5062`  
		Last Modified: Wed, 13 May 2020 14:08:57 GMT  
		Size: 281.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6433b34e08c264604cf56b6cb52a7b884877a9236df0ec81d7b296f95fc008b2`  
		Last Modified: Wed, 13 May 2020 14:08:57 GMT  
		Size: 1.7 KB (1722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc6ab638f272e23d5a3ade2a7cb05bee20f9d4b2753a898b710c3dfd0f2da8b3`  
		Last Modified: Wed, 13 May 2020 14:08:57 GMT  
		Size: 2.1 KB (2067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca0dbaf728404a8b2cc6adf17c4cb481241488f1643f5aa21f14c57412ab76e8`  
		Last Modified: Wed, 13 May 2020 14:08:57 GMT  
		Size: 200.6 KB (200611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
