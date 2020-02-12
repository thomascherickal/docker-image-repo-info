<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `kibana`

-	[`kibana:6.8.6`](#kibana686)
-	[`kibana:7.6.0`](#kibana760)

## `kibana:6.8.6`

```console
$ docker pull kibana@sha256:f773d11d6a4304d1795d63b6877cf7e21bbcb4703d57444325f0a906163a408c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kibana:6.8.6` - linux; amd64

```console
$ docker pull kibana@sha256:0a831b9e3251e777615aed743ba46ebd2b0253cd6e39c7636246515710f78379
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **298.9 MB (298870006 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:adfab5632ef4cb6f1458f27dc9e580bb4c6ff04f3d219c9ddb7c92c77e312ea8`
-	Default Command: `["\/usr\/local\/bin\/kibana-docker"]`

```dockerfile
# Tue, 12 Nov 2019 00:20:33 GMT
ADD file:45a381049c52b5664e5e911dead277b25fadbae689c0bb35be3c42dff0f2dffe in / 
# Tue, 12 Nov 2019 00:20:33 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20191001
# Tue, 12 Nov 2019 00:20:33 GMT
CMD ["/bin/bash"]
# Fri, 13 Dec 2019 17:58:37 GMT
EXPOSE 5601
# Fri, 13 Dec 2019 17:59:22 GMT
RUN yum update -y && yum install -y fontconfig freetype && yum clean all
# Fri, 13 Dec 2019 18:00:09 GMT
COPY --chown=1000:0dir:b7add46674939973162bad0e77bc7e684546e7577015c708dc2a8dad71ebd2f1 in /usr/share/kibana 
# Fri, 13 Dec 2019 18:00:10 GMT
WORKDIR /usr/share/kibana
# Fri, 13 Dec 2019 18:00:13 GMT
RUN ln -s /usr/share/kibana /opt/kibana
# Fri, 13 Dec 2019 18:00:13 GMT
ENV ELASTIC_CONTAINER=true
# Fri, 13 Dec 2019 18:00:14 GMT
ENV PATH=/usr/share/kibana/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 13 Dec 2019 18:00:16 GMT
COPY --chown=1000:0file:60b6181f28c99b362092ea6139b6d4112ddd0bef32d52563c33b26bdc2b51318 in /usr/share/kibana/config/kibana.yml 
# Fri, 13 Dec 2019 18:00:17 GMT
COPY --chown=1000:0file:af2bc419b515a5fca0bc857249c43a0e082e6cb60c394519993854e4bc8048ca in /usr/local/bin/ 
# Fri, 13 Dec 2019 18:00:20 GMT
RUN chmod g+ws /usr/share/kibana && find /usr/share/kibana -gid 0 -and -not -perm /g+w -exec chmod g+w {} \;
# Fri, 13 Dec 2019 18:00:23 GMT
RUN groupadd --gid 1000 kibana && useradd --uid 1000 --gid 1000 --home-dir /usr/share/kibana --no-create-home kibana
# Fri, 13 Dec 2019 18:00:23 GMT
USER kibana
# Fri, 13 Dec 2019 18:00:24 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.vendor=Elastic org.label-schema.name=kibana org.label-schema.version=6.8.6 org.label-schema.url=https://www.elastic.co/products/kibana org.label-schema.vcs-url=https://github.com/elastic/kibana org.label-schema.license=Elastic License license=Elastic License
# Fri, 13 Dec 2019 18:00:25 GMT
CMD ["/usr/local/bin/kibana-docker"]
```

-	Layers:
	-	`sha256:ab5ef0e5819490abe86106fd9f4381123e37a03e80e650be39f7938d30ecb530`  
		Last Modified: Tue, 12 Nov 2019 00:23:38 GMT  
		Size: 75.8 MB (75780712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40057de213d2c47a5d196cba4b2e8911f7caba1e0e40ddc45ff5ff1fcda7f560`  
		Last Modified: Wed, 18 Dec 2019 22:13:01 GMT  
		Size: 33.1 MB (33136094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:434b62b0636c274e666fc1bc6c3577a35b48747a0bb19f61a3237bce06a61ada`  
		Last Modified: Wed, 18 Dec 2019 22:13:17 GMT  
		Size: 189.9 MB (189948389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7370972a467b446b5ca4da1b7148e5002914f5c9a4fe4e8d1a5c1cc6c3ecbcd3`  
		Last Modified: Wed, 18 Dec 2019 22:12:49 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e1767103506c625b66853d42b82fe0998a8db43557a61d2ed7ad5bfaedfaac4`  
		Last Modified: Wed, 18 Dec 2019 22:12:49 GMT  
		Size: 401.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83c66d66f9304e3a4ccfd6b61323890268da91f9253179406f2b3ece8f4c4f73`  
		Last Modified: Wed, 18 Dec 2019 22:12:49 GMT  
		Size: 2.3 KB (2259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:590781aeb7f42c4f7573d916a9448a8f3acb4133bf8452c914c7c89cfed95a3f`  
		Last Modified: Wed, 18 Dec 2019 22:12:49 GMT  
		Size: 165.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1efa205edea3066282cf9cd02991379b868214fce810c0260cf0fda78968056`  
		Last Modified: Wed, 18 Dec 2019 22:12:49 GMT  
		Size: 1.8 KB (1847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kibana:7.6.0`

```console
$ docker pull kibana@sha256:71224955f60c9b71e633b332da41046891841b205e93763d845514c174287967
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kibana:7.6.0` - linux; amd64

```console
$ docker pull kibana@sha256:038e0084f26a2265118f837104e5411c89f7cd3e9500b8878bef10aa63e3e70e
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **361.2 MB (361215795 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b36db011e72cafa3a11e3ee35fcd529310cb76c053a103ee0689033a5a548c02`
-	Entrypoint: `["\/usr\/local\/bin\/dumb-init","--"]`
-	Default Command: `["\/usr\/local\/bin\/kibana-docker"]`

```dockerfile
# Tue, 12 Nov 2019 00:20:33 GMT
ADD file:45a381049c52b5664e5e911dead277b25fadbae689c0bb35be3c42dff0f2dffe in / 
# Tue, 12 Nov 2019 00:20:33 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20191001
# Tue, 12 Nov 2019 00:20:33 GMT
CMD ["/bin/bash"]
# Thu, 06 Feb 2020 01:02:35 GMT
EXPOSE 5601
# Thu, 06 Feb 2020 01:03:14 GMT
RUN yum update -y && yum install -y fontconfig freetype shadow-utils && yum clean all
# Thu, 06 Feb 2020 01:03:18 GMT
RUN curl -L -o /usr/local/bin/dumb-init https://github.com/Yelp/dumb-init/releases/download/v1.2.2/dumb-init_1.2.2_amd64
# Thu, 06 Feb 2020 01:03:18 GMT
RUN echo "37f2c1f0372a45554f1b89924fbb134fc24c3756efaedf11e07f599494e0eff9  /usr/local/bin/dumb-init" | sha256sum -c -
# Thu, 06 Feb 2020 01:03:19 GMT
RUN chmod +x /usr/local/bin/dumb-init
# Thu, 06 Feb 2020 01:04:07 GMT
COPY --chown=1000:0dir:62869a42e93f360b535e6133a09983d3f73966432fbe8a1b56668205183f8cd4 in /usr/share/kibana 
# Thu, 06 Feb 2020 01:04:09 GMT
WORKDIR /usr/share/kibana
# Thu, 06 Feb 2020 01:04:10 GMT
RUN ln -s /usr/share/kibana /opt/kibana
# Thu, 06 Feb 2020 01:04:11 GMT
ENV ELASTIC_CONTAINER=true
# Thu, 06 Feb 2020 01:04:11 GMT
ENV PATH=/usr/share/kibana/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Feb 2020 01:04:11 GMT
COPY --chown=1000:0file:60b6181f28c99b362092ea6139b6d4112ddd0bef32d52563c33b26bdc2b51318 in /usr/share/kibana/config/kibana.yml 
# Thu, 06 Feb 2020 01:04:12 GMT
COPY --chown=1000:0file:7e3757ed72f2811325115d3fa9113960d73d97954bee415c986b47983e1ca231 in /usr/local/bin/ 
# Thu, 06 Feb 2020 01:04:14 GMT
RUN chmod g+ws /usr/share/kibana && find /usr/share/kibana -gid 0 -and -not -perm /g+w -exec chmod g+w {} \;
# Thu, 06 Feb 2020 01:04:15 GMT
RUN groupadd --gid 1000 kibana && useradd --uid 1000 --gid 1000 --home-dir /usr/share/kibana --no-create-home kibana
# Thu, 06 Feb 2020 01:04:15 GMT
USER kibana
# Thu, 06 Feb 2020 01:04:15 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.vendor=Elastic org.label-schema.name=kibana org.label-schema.version=7.6.0 org.label-schema.url=https://www.elastic.co/products/kibana org.label-schema.vcs-url=https://github.com/elastic/kibana org.label-schema.license=Elastic License org.label-schema.usage=https://www.elastic.co/guide/en/kibana/index.html org.label-schema.build-date=2020-02-06T00:59:55.664Z license=Elastic License
# Thu, 06 Feb 2020 01:04:15 GMT
ENTRYPOINT ["/usr/local/bin/dumb-init" "--"]
# Thu, 06 Feb 2020 01:04:15 GMT
CMD ["/usr/local/bin/kibana-docker"]
```

-	Layers:
	-	`sha256:ab5ef0e5819490abe86106fd9f4381123e37a03e80e650be39f7938d30ecb530`  
		Last Modified: Tue, 12 Nov 2019 00:23:38 GMT  
		Size: 75.8 MB (75780712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a92ac72d98206c0d2cfa9795dcaabee723d58ad80aa0b8eab416e15bc82d53b`  
		Last Modified: Tue, 11 Feb 2020 16:07:58 GMT  
		Size: 33.6 MB (33575104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3610a99415df16166d137ab4f9703e9743666934e7229d240de425c3d8cbb67`  
		Last Modified: Tue, 11 Feb 2020 16:07:52 GMT  
		Size: 31.7 KB (31698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ea5080d6dc3f303930552cfab5cdf2e67e4163eefe2d1365db04795c93923d7`  
		Last Modified: Tue, 11 Feb 2020 16:07:51 GMT  
		Size: 30.2 KB (30205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5f63ed4caa0addcae0b5d393d15bce50f78b7e967614e4e8fae8aaf66668839`  
		Last Modified: Tue, 11 Feb 2020 16:08:28 GMT  
		Size: 251.8 MB (251792573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c64c037065d614588fc391b6eaf4cdee144a47a6f9df7f825a3757284fa11353`  
		Last Modified: Tue, 11 Feb 2020 16:07:48 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0b46544cee9fb74b341cbd38094cc6e684e56a7ed5dd8f4442b05c6b502fa72`  
		Last Modified: Tue, 11 Feb 2020 16:07:48 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b084b06bf8c5a3d5cc5014388addfa27a490311bbb36ff80241a6dd45fd8e6a`  
		Last Modified: Tue, 11 Feb 2020 16:07:48 GMT  
		Size: 2.9 KB (2946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:911c7214ed1538b60aee0b23e16469da83a745a3f04ccb319872773a80f66f24`  
		Last Modified: Tue, 11 Feb 2020 16:07:48 GMT  
		Size: 166.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dcfd483854e60c1d8a57f66b7cbbe1623bbc1fd88d690e2bfc3eb33fd67d1a6`  
		Last Modified: Tue, 11 Feb 2020 16:07:49 GMT  
		Size: 1.8 KB (1849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
