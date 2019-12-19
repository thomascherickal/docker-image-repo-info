<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `elasticsearch`

-	[`elasticsearch:6.8.6`](#elasticsearch686)
-	[`elasticsearch:7.5.1`](#elasticsearch751)

## `elasticsearch:6.8.6`

```console
$ docker pull elasticsearch@sha256:be763d0b98b58a963f0496677be546211ec9aa336b0981ede98cec63325f55ef
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `elasticsearch:6.8.6` - linux; amd64

```console
$ docker pull elasticsearch@sha256:ae5006dce6042a234c0bc96ec1634925aae5d1ef590dab62f93d67761f36d694
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **465.2 MB (465193810 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c8b4938e5db23c1062a38ed72bfea1b764e388c7480d095b8040ca2fe350a5e3`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["eswrapper"]`

```dockerfile
# Tue, 12 Nov 2019 00:20:33 GMT
ADD file:45a381049c52b5664e5e911dead277b25fadbae689c0bb35be3c42dff0f2dffe in / 
# Tue, 12 Nov 2019 00:20:33 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20191001
# Tue, 12 Nov 2019 00:20:33 GMT
CMD ["/bin/bash"]
# Fri, 13 Dec 2019 17:16:36 GMT
ENV ELASTIC_CONTAINER=true
# Fri, 13 Dec 2019 17:16:37 GMT
ENV JAVA_HOME=/opt/jdk-13.0.1+9
# Fri, 13 Dec 2019 17:16:45 GMT
COPY dir:9ae941118a30a34d70aaead6ea1e85696e8f9d5331e6fccee2ff5817fb22eb15 in /opt/jdk-13.0.1+9 
# Fri, 13 Dec 2019 17:17:10 GMT
RUN for iter in {1..10}; do yum update  --setopt=tsflags=nodocs -y &&     yum install -y  --setopt=tsflags=nodocs nc unzip wget which &&     yum clean all && exit_code=0 && break || exit_code=\$? && echo "yum error: retry $iter in 10s" && sleep 10; done;     (exit $exit_code)
# Fri, 13 Dec 2019 17:17:12 GMT
RUN groupadd -g 1000 elasticsearch &&     adduser -u 1000 -g 1000 -G 0 -d /usr/share/elasticsearch elasticsearch &&     chmod 0775 /usr/share/elasticsearch &&     chgrp 0 /usr/share/elasticsearch
# Fri, 13 Dec 2019 17:17:12 GMT
WORKDIR /usr/share/elasticsearch
# Fri, 13 Dec 2019 17:17:17 GMT
COPY --chown=1000:0dir:85bcbd97e60b7f2a7d1d96552f66473e1f261250fa6fc535ecd8181651ccb03a in /usr/share/elasticsearch 
# Fri, 13 Dec 2019 17:17:19 GMT
ENV PATH=/usr/share/elasticsearch/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 13 Dec 2019 17:17:20 GMT
COPY --chown=1000:0file:08193f849fc25f29db1438eff6d5c9fe1d63237aeb07a3e0009e8ba554f97c31 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 13 Dec 2019 17:17:22 GMT
RUN chgrp 0 /usr/local/bin/docker-entrypoint.sh &&     chmod g=u /etc/passwd &&     chmod 0775 /usr/local/bin/docker-entrypoint.sh
# Fri, 13 Dec 2019 17:17:23 GMT
EXPOSE 9200 9300
# Fri, 13 Dec 2019 17:17:23 GMT
LABEL org.label-schema.build-date=2019-12-13T17:11:52.013738Z org.label-schema.license=Elastic-License org.label-schema.name=Elasticsearch org.label-schema.schema-version=1.0 org.label-schema.url=https://www.elastic.co/products/elasticsearch org.label-schema.usage=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.label-schema.vcs-ref=3d9f765bcad28244dc4c8eb8e8b7ba97ba5408f1 org.label-schema.vcs-url=https://github.com/elastic/elasticsearch org.label-schema.vendor=Elastic org.label-schema.version=6.8.6 org.opencontainers.image.created=2019-12-13T17:11:52.013738Z org.opencontainers.image.documentation=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.opencontainers.image.licenses=Elastic-License org.opencontainers.image.revision=3d9f765bcad28244dc4c8eb8e8b7ba97ba5408f1 org.opencontainers.image.source=https://github.com/elastic/elasticsearch org.opencontainers.image.title=Elasticsearch org.opencontainers.image.url=https://www.elastic.co/products/elasticsearch org.opencontainers.image.vendor=Elastic org.opencontainers.image.version=6.8.6
# Fri, 13 Dec 2019 17:17:23 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Fri, 13 Dec 2019 17:17:23 GMT
CMD ["eswrapper"]
```

-	Layers:
	-	`sha256:ab5ef0e5819490abe86106fd9f4381123e37a03e80e650be39f7938d30ecb530`  
		Last Modified: Tue, 12 Nov 2019 00:23:38 GMT  
		Size: 75.8 MB (75780712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30cb0e53690c527d4f2213474e7e9d356d74eca131af3367af3c01a993a27a16`  
		Last Modified: Wed, 18 Dec 2019 18:41:55 GMT  
		Size: 208.5 MB (208485142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fbe49af2e052fc15d0d9b010ea5208ef4f20b5914c96382137ff5dd382b9388`  
		Last Modified: Wed, 18 Dec 2019 18:41:51 GMT  
		Size: 30.4 MB (30383567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5c2f84a28532ad57f599eeb33c4dcd10416730a521120a5e8f716057d84feb9`  
		Last Modified: Wed, 18 Dec 2019 18:41:33 GMT  
		Size: 2.3 KB (2328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5abe907f1981b69082a672cbfb0df3f6caefc6d67fc8044c9a89c7be6d4a1a47`  
		Last Modified: Wed, 18 Dec 2019 18:41:54 GMT  
		Size: 150.5 MB (150537564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af265c640f776a25613348dae3e11786dd002226598997e92bbfdd1257cafb76`  
		Last Modified: Wed, 18 Dec 2019 18:41:28 GMT  
		Size: 2.1 KB (2080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02437bb6d8162fb9fcc460b210525a0b700646c88e2bf57b61a7e338477d9300`  
		Last Modified: Wed, 18 Dec 2019 18:41:28 GMT  
		Size: 2.4 KB (2417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `elasticsearch:7.5.1`

```console
$ docker pull elasticsearch@sha256:2a9b8bf9f1378bb72bb03ac7bf29f7ed094a6b0e402433279f68bf0589a4c64f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `elasticsearch:7.5.1` - linux; amd64

```console
$ docker pull elasticsearch@sha256:c75ed9b9718b803449a020744d0fc776e45386ec191a3c6f1faf898fb0b680b5
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **397.5 MB (397489123 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2bd69c322e9876cfd5adac78a9fd365954412ca8cf91b203b646c397e057f942`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["eswrapper"]`

```dockerfile
# Tue, 12 Nov 2019 00:20:33 GMT
ADD file:45a381049c52b5664e5e911dead277b25fadbae689c0bb35be3c42dff0f2dffe in / 
# Tue, 12 Nov 2019 00:20:33 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20191001
# Tue, 12 Nov 2019 00:20:33 GMT
CMD ["/bin/bash"]
# Mon, 16 Dec 2019 23:02:12 GMT
ENV ELASTIC_CONTAINER=true
# Mon, 16 Dec 2019 23:02:49 GMT
RUN for iter in {1..10}; do yum update  --setopt=tsflags=nodocs -y &&     yum install -y  --setopt=tsflags=nodocs nc &&     yum clean all && exit_code=0 && break || exit_code=$? && echo "yum error: retry $iter in 10s" && sleep 10; done;     (exit $exit_code)
# Mon, 16 Dec 2019 23:02:52 GMT
RUN groupadd -g 1000 elasticsearch &&     adduser -u 1000 -g 1000 -G 0 -d /usr/share/elasticsearch elasticsearch &&     chmod 0775 /usr/share/elasticsearch &&     chgrp 0 /usr/share/elasticsearch
# Mon, 16 Dec 2019 23:02:53 GMT
WORKDIR /usr/share/elasticsearch
# Mon, 16 Dec 2019 23:03:02 GMT
COPY --chown=1000:0dir:ef286cd06f0525ba5e717359a18106f87e36ed49664b955fee316af3a0a4c087 in /usr/share/elasticsearch 
# Mon, 16 Dec 2019 23:03:05 GMT
RUN ln -sf /etc/pki/ca-trust/extracted/java/cacerts /usr/share/elasticsearch/jdk/lib/security/cacerts
# Mon, 16 Dec 2019 23:03:06 GMT
ENV PATH=/usr/share/elasticsearch/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 16 Dec 2019 23:03:06 GMT
COPY --chown=1000:0file:8aaf8c70cc610ac6e2caadd743341d4590a184092390227b9bfc69044c733e28 in /usr/local/bin/docker-entrypoint.sh 
# Mon, 16 Dec 2019 23:03:08 GMT
RUN chgrp 0 /usr/local/bin/docker-entrypoint.sh &&     chmod g=u /etc/passwd &&     chmod 0775 /usr/local/bin/docker-entrypoint.sh
# Mon, 16 Dec 2019 23:03:08 GMT
EXPOSE 9200 9300
# Mon, 16 Dec 2019 23:03:08 GMT
LABEL org.label-schema.build-date=2019-12-16T22:57:37.839371Z org.label-schema.license=Elastic-License org.label-schema.name=Elasticsearch org.label-schema.schema-version=1.0 org.label-schema.url=https://www.elastic.co/products/elasticsearch org.label-schema.usage=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.label-schema.vcs-ref=3ae9ac9a93c95bd0cdc054951cf95d88e1e18d96 org.label-schema.vcs-url=https://github.com/elastic/elasticsearch org.label-schema.vendor=Elastic org.label-schema.version=7.5.1 org.opencontainers.image.created=2019-12-16T22:57:37.839371Z org.opencontainers.image.documentation=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.opencontainers.image.licenses=Elastic-License org.opencontainers.image.revision=3ae9ac9a93c95bd0cdc054951cf95d88e1e18d96 org.opencontainers.image.source=https://github.com/elastic/elasticsearch org.opencontainers.image.title=Elasticsearch org.opencontainers.image.url=https://www.elastic.co/products/elasticsearch org.opencontainers.image.vendor=Elastic org.opencontainers.image.version=7.5.1
# Mon, 16 Dec 2019 23:03:09 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Mon, 16 Dec 2019 23:03:09 GMT
CMD ["eswrapper"]
```

-	Layers:
	-	`sha256:ab5ef0e5819490abe86106fd9f4381123e37a03e80e650be39f7938d30ecb530`  
		Last Modified: Tue, 12 Nov 2019 00:23:38 GMT  
		Size: 75.8 MB (75780712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29c9c908c343c14198d53e460710b6c1603cbc7764d29836a9f1b4fe21140bae`  
		Last Modified: Wed, 18 Dec 2019 19:21:41 GMT  
		Size: 30.0 MB (30004283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4de40ab1455464b1de1211cd211eed1fcbb2940350859153569adf8f715a3796`  
		Last Modified: Wed, 18 Dec 2019 19:20:37 GMT  
		Size: 2.3 KB (2329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9facd5b26e16b61fa9c4ce50d7522c89b4427fa293da42c29cbfdc7679176e1`  
		Last Modified: Wed, 18 Dec 2019 19:28:03 GMT  
		Size: 291.7 MB (291697022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:885429ae08e8f0d7b86ed207a8647720de24dddd0a0e75a715624655e268f960`  
		Last Modified: Wed, 18 Dec 2019 19:20:32 GMT  
		Size: 291.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5df846ea1ead47fb964d67bb67361e4372394775067e666c6a8c679ed637533`  
		Last Modified: Wed, 18 Dec 2019 19:20:29 GMT  
		Size: 2.1 KB (2073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ec75ecc3688d77e402f68ba412dc6d04b9da857397b32909dccc752d3001251`  
		Last Modified: Wed, 18 Dec 2019 19:20:25 GMT  
		Size: 2.4 KB (2413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
