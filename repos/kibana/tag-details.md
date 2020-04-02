<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `kibana`

-	[`kibana:6.8.8`](#kibana688)
-	[`kibana:7.6.2`](#kibana762)

## `kibana:6.8.8`

```console
$ docker pull kibana@sha256:53891a7457becef4a21e339d225f9fa1ad143cab23898366e1ddd4d2a9de85dd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kibana:6.8.8` - linux; amd64

```console
$ docker pull kibana@sha256:0e5958b8648a36eb8fe6cabd76980fe489eae6d7f65705b665618d43281ba004
```

-	Docker Version: 19.03.6
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **300.3 MB (300314573 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c39b4e97559ebe51e4e6ecb40298f4421c45dd0acac3616967f1f1a550027783`
-	Default Command: `["\/usr\/local\/bin\/kibana-docker"]`

```dockerfile
# Tue, 12 Nov 2019 00:20:33 GMT
ADD file:45a381049c52b5664e5e911dead277b25fadbae689c0bb35be3c42dff0f2dffe in / 
# Tue, 12 Nov 2019 00:20:33 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20191001
# Tue, 12 Nov 2019 00:20:33 GMT
CMD ["/bin/bash"]
# Thu, 19 Mar 2020 00:08:19 GMT
EXPOSE 5601
# Thu, 19 Mar 2020 00:09:02 GMT
RUN yum update -y && yum install -y fontconfig freetype && yum clean all
# Thu, 19 Mar 2020 00:09:49 GMT
COPY --chown=1000:0dir:5abb9761e39023efcda6c1cb7ff20636ee78a404028832904316bdc1a68338da in /usr/share/kibana 
# Thu, 19 Mar 2020 00:09:50 GMT
WORKDIR /usr/share/kibana
# Thu, 19 Mar 2020 00:09:54 GMT
RUN ln -s /usr/share/kibana /opt/kibana
# Thu, 19 Mar 2020 00:09:54 GMT
ENV ELASTIC_CONTAINER=true
# Thu, 19 Mar 2020 00:09:55 GMT
ENV PATH=/usr/share/kibana/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 19 Mar 2020 00:09:56 GMT
COPY --chown=1000:0file:60b6181f28c99b362092ea6139b6d4112ddd0bef32d52563c33b26bdc2b51318 in /usr/share/kibana/config/kibana.yml 
# Thu, 19 Mar 2020 00:09:57 GMT
COPY --chown=1000:0file:af2bc419b515a5fca0bc857249c43a0e082e6cb60c394519993854e4bc8048ca in /usr/local/bin/ 
# Thu, 19 Mar 2020 00:10:00 GMT
RUN chmod g+ws /usr/share/kibana && find /usr/share/kibana -gid 0 -and -not -perm /g+w -exec chmod g+w {} \;
# Thu, 19 Mar 2020 00:10:02 GMT
RUN groupadd --gid 1000 kibana && useradd --uid 1000 --gid 1000 --home-dir /usr/share/kibana --no-create-home kibana
# Thu, 19 Mar 2020 00:10:02 GMT
USER kibana
# Thu, 19 Mar 2020 00:10:03 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.vendor=Elastic org.label-schema.name=kibana org.label-schema.version=6.8.8 org.label-schema.url=https://www.elastic.co/products/kibana org.label-schema.vcs-url=https://github.com/elastic/kibana org.label-schema.license=Elastic License license=Elastic License
# Thu, 19 Mar 2020 00:10:03 GMT
CMD ["/usr/local/bin/kibana-docker"]
```

-	Layers:
	-	`sha256:ab5ef0e5819490abe86106fd9f4381123e37a03e80e650be39f7938d30ecb530`  
		Last Modified: Tue, 12 Nov 2019 00:23:38 GMT  
		Size: 75.8 MB (75780712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b47f63f7f2e11bdea5c985bc301a03a771d26f30b6d659004ffee54876da5651`  
		Last Modified: Tue, 31 Mar 2020 16:06:42 GMT  
		Size: 33.7 MB (33718450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9228ca7ca7541b87ff583761ca97d98815859a8ac0a5882c2a5ce0884eb3a7b`  
		Last Modified: Tue, 31 Mar 2020 16:07:03 GMT  
		Size: 190.8 MB (190810594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3036e6504fe06cddd8501cf1b33c317f3a1c676d5ca9ca109b20d582bd5adaf`  
		Last Modified: Tue, 31 Mar 2020 16:06:32 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb19e8c828d120d3b2ea529330a83b3371c8eeb6fd2f8340d031defd78a8ce32`  
		Last Modified: Tue, 31 Mar 2020 16:06:33 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f4a23909a5093a3a9736c21862fadd6555dbe317fb13a42e2fd5c1b5469e630`  
		Last Modified: Tue, 31 Mar 2020 16:06:32 GMT  
		Size: 2.3 KB (2257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eeb991ba9f7d4c58d92a55c95692e08c481e90f56901aa25a739341c5e901973`  
		Last Modified: Tue, 31 Mar 2020 16:06:32 GMT  
		Size: 166.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:833f9ef9a53a94087c8d08550025b2e90ef88cb16cb2ac83892e77fe31a03065`  
		Last Modified: Tue, 31 Mar 2020 16:06:32 GMT  
		Size: 1.9 KB (1850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kibana:7.6.2`

```console
$ docker pull kibana@sha256:097e2b7f33f353a8fc19bbf2a6558431c63637113fdc625e6d34fc46f96c0130
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kibana:7.6.2` - linux; amd64

```console
$ docker pull kibana@sha256:efec1f93595d1fa29b2144bf8f4cdee22ab77ca88903b6c6f285def17203c2a2
```

-	Docker Version: 19.03.6
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **361.5 MB (361473105 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f70986bc519117ae1c1135725b58e21ab17cda87400637c0d9a4d3ecbe0ad6c0`
-	Entrypoint: `["\/usr\/local\/bin\/dumb-init","--"]`
-	Default Command: `["\/usr\/local\/bin\/kibana-docker"]`

```dockerfile
# Tue, 12 Nov 2019 00:20:33 GMT
ADD file:45a381049c52b5664e5e911dead277b25fadbae689c0bb35be3c42dff0f2dffe in / 
# Tue, 12 Nov 2019 00:20:33 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20191001
# Tue, 12 Nov 2019 00:20:33 GMT
CMD ["/bin/bash"]
# Thu, 26 Mar 2020 07:53:21 GMT
EXPOSE 5601
# Thu, 26 Mar 2020 07:53:51 GMT
RUN yum update -y && yum install -y fontconfig freetype shadow-utils && yum clean all
# Thu, 26 Mar 2020 07:53:54 GMT
RUN curl -L -o /usr/local/bin/dumb-init https://github.com/Yelp/dumb-init/releases/download/v1.2.2/dumb-init_1.2.2_amd64
# Thu, 26 Mar 2020 07:53:57 GMT
RUN echo "37f2c1f0372a45554f1b89924fbb134fc24c3756efaedf11e07f599494e0eff9  /usr/local/bin/dumb-init" | sha256sum -c -
# Thu, 26 Mar 2020 07:53:59 GMT
RUN chmod +x /usr/local/bin/dumb-init
# Thu, 26 Mar 2020 07:55:35 GMT
COPY --chown=1000:0dir:70e3c94c1a5a3807b3a2f694353b2f6349acfec2a226bc4642224e822fb17576 in /usr/share/kibana 
# Thu, 26 Mar 2020 07:55:36 GMT
WORKDIR /usr/share/kibana
# Thu, 26 Mar 2020 07:55:41 GMT
RUN ln -s /usr/share/kibana /opt/kibana
# Thu, 26 Mar 2020 07:55:42 GMT
ENV ELASTIC_CONTAINER=true
# Thu, 26 Mar 2020 07:55:42 GMT
ENV PATH=/usr/share/kibana/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 26 Mar 2020 07:55:43 GMT
COPY --chown=1000:0file:60b6181f28c99b362092ea6139b6d4112ddd0bef32d52563c33b26bdc2b51318 in /usr/share/kibana/config/kibana.yml 
# Thu, 26 Mar 2020 07:55:44 GMT
COPY --chown=1000:0file:0d24c5e38b0b17ceeb1508e02edbf4be9a750e9c5fa6853e5f9cbed55c4b17d2 in /usr/local/bin/ 
# Thu, 26 Mar 2020 07:55:48 GMT
RUN chmod g+ws /usr/share/kibana && find /usr/share/kibana -gid 0 -and -not -perm /g+w -exec chmod g+w {} \;
# Thu, 26 Mar 2020 07:55:51 GMT
RUN groupadd --gid 1000 kibana && useradd --uid 1000 --gid 1000 --home-dir /usr/share/kibana --no-create-home kibana
# Thu, 26 Mar 2020 07:55:51 GMT
USER kibana
# Thu, 26 Mar 2020 07:55:51 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.vendor=Elastic org.label-schema.name=kibana org.label-schema.version=7.6.2 org.label-schema.url=https://www.elastic.co/products/kibana org.label-schema.vcs-url=https://github.com/elastic/kibana org.label-schema.license=Elastic License org.label-schema.usage=https://www.elastic.co/guide/en/kibana/index.html org.label-schema.build-date=2020-03-26T07:47:43.654Z license=Elastic License
# Thu, 26 Mar 2020 07:55:51 GMT
ENTRYPOINT ["/usr/local/bin/dumb-init" "--"]
# Thu, 26 Mar 2020 07:55:51 GMT
CMD ["/usr/local/bin/kibana-docker"]
```

-	Layers:
	-	`sha256:ab5ef0e5819490abe86106fd9f4381123e37a03e80e650be39f7938d30ecb530`  
		Last Modified: Tue, 12 Nov 2019 00:23:38 GMT  
		Size: 75.8 MB (75780712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c64d415fc4c46007a026a68c61c64296171da3612c442cf8d71f32c5d865e956`  
		Last Modified: Tue, 31 Mar 2020 16:20:12 GMT  
		Size: 33.7 MB (33722246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40a228497f8722bd4fefe218a44fea5e8caf6229056063ed63caf1806ffedc54`  
		Last Modified: Tue, 31 Mar 2020 16:20:04 GMT  
		Size: 31.7 KB (31688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:047cebeb3d2b8b3419ac20392a65cc775cd60bb8833a22c550df7d947fbd55e4`  
		Last Modified: Tue, 31 Mar 2020 16:20:04 GMT  
		Size: 30.2 KB (30201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1e90407e5228775949396692e883b25b96f17e718b117af0619a4ca72b9add7`  
		Last Modified: Tue, 31 Mar 2020 16:20:44 GMT  
		Size: 251.9 MB (251902743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b665bda75e65b1153c35bddf23fa7b76f208a8aa15735ae75495f611b3b8c630`  
		Last Modified: Tue, 31 Mar 2020 16:20:02 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12bc27d9cfdc8c51840a4bdd4c3a63b31e33331d0371f379862ff3d9fcb2da68`  
		Last Modified: Tue, 31 Mar 2020 16:20:02 GMT  
		Size: 403.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2611a8427d9d9fa99ba49a78d61c2313336e020c00658983e3997f833e49953a`  
		Last Modified: Tue, 31 Mar 2020 16:20:02 GMT  
		Size: 3.0 KB (2961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12efd486dee3fbd68595ee114ccf695d409c5724f2427046a468b48e050e55a9`  
		Last Modified: Tue, 31 Mar 2020 16:20:02 GMT  
		Size: 167.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2dfc5062b56548c691bb4cb8b6acebb77e859d706b5ea1088b569da0883ed55`  
		Last Modified: Tue, 31 Mar 2020 16:20:02 GMT  
		Size: 1.8 KB (1845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
