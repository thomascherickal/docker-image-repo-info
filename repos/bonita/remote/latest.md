## `bonita:latest`

```console
$ docker pull bonita@sha256:7b91a7d8721867c77fcdf25372e5e03408be1c456b6d35fc8a6b0fb48421b36f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:latest` - linux; amd64

```console
$ docker pull bonita@sha256:af5ce478262df702bb04b790e131a237ccda60a8479b2e0828d4ff823d74be86
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **235.0 MB (234967761 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc08f7f52f12153165ce8759404b4521aaec0b3785c8e7f3ae86611de8d453b8`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Fri, 01 Oct 2021 02:23:23 GMT
ADD file:0d82cd095966e8ee78b593cb47a352eec842edb7bd9d9468e8a70154522447d1 in / 
# Fri, 01 Oct 2021 02:23:24 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 03:22:15 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Thu, 07 Oct 2021 18:20:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends       curl       gnupg2       mysql-client-core-5.7       openjdk-11-jre-headless       postgresql-client       unzip       zip   && rm -rf /var/lib/apt/lists/*
# Thu, 07 Oct 2021 18:20:38 GMT
RUN mkdir /opt/custom-init.d/
# Thu, 07 Oct 2021 18:20:39 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Thu, 07 Oct 2021 18:20:47 GMT
RUN gpg --keyserver keyserver.ubuntu.com --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Thu, 07 Oct 2021 18:20:48 GMT
ARG BONITA_VERSION
# Thu, 07 Oct 2021 18:20:48 GMT
ARG BRANDING_VERSION
# Thu, 07 Oct 2021 18:20:48 GMT
ARG BONITA_SHA256
# Thu, 07 Oct 2021 18:20:48 GMT
ARG BASE_URL
# Thu, 07 Oct 2021 18:20:48 GMT
ARG BONITA_URL
# Thu, 07 Oct 2021 18:20:49 GMT
ENV BONITA_VERSION=7.13.0
# Thu, 07 Oct 2021 18:20:49 GMT
ENV BRANDING_VERSION=2021.2-u0
# Thu, 07 Oct 2021 18:20:49 GMT
ENV BONITA_SHA256=e4f279765cd729885a4e353d96d1d85c5f69fef63f79183e0ccf3ffaa0cb2417
# Thu, 07 Oct 2021 18:20:49 GMT
ENV ZIP_FILE=BonitaCommunity-2021.2-u0.zip
# Thu, 07 Oct 2021 18:20:49 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Thu, 07 Oct 2021 18:20:49 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.2-u0/BonitaCommunity-2021.2-u0.zip
# Thu, 07 Oct 2021 18:20:50 GMT
RUN mkdir /opt/files
# Thu, 07 Oct 2021 18:20:50 GMT
COPY dir:6250b774ea0abc098d97c259e44608a8bf8835310bd84b47cecb5b027fb6826b in /opt/files 
# Thu, 07 Oct 2021 18:20:57 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi   && sha256sum /opt/files/${ZIP_FILE}   && echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && unzip /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war -d /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita/   && rm /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip
# Thu, 07 Oct 2021 18:20:58 GMT
ENV HTTP_API=false
# Thu, 07 Oct 2021 18:20:58 GMT
VOLUME [/opt/bonita]
# Thu, 07 Oct 2021 18:20:58 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Thu, 07 Oct 2021 18:20:59 GMT
EXPOSE 8080
# Thu, 07 Oct 2021 18:20:59 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:284055322776031bac33723839acb0db2d063a525ba4fa1fd268a831c7553b26`  
		Last Modified: Fri, 01 Oct 2021 02:25:02 GMT  
		Size: 26.7 MB (26705075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e24fcd4d81ab22a61d90fa3bfbb89af68aa309392e4f52d6bcbcf5c6fbd38770`  
		Last Modified: Thu, 07 Oct 2021 18:21:42 GMT  
		Size: 93.5 MB (93524392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79d6cf7b55d5976ac40200f242794d1b0abd86ebb8b117e886057a4b0bd2ff9d`  
		Last Modified: Thu, 07 Oct 2021 18:21:28 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:497eacbda8af032090ea52ce9eeb03cc21c69cb0080cab7200ff4aeaf4662d8c`  
		Last Modified: Thu, 07 Oct 2021 18:21:28 GMT  
		Size: 1.9 KB (1880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e57b5a3ebad692905253ff80476bd2d68ca2b6c4086b3093d58bb0e9994bef0`  
		Last Modified: Thu, 07 Oct 2021 18:21:26 GMT  
		Size: 1.0 MB (1003184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0ec65fae91ba331dd75198a508d34f30f126ef69c1f19bd8c1e1785a5c714cb`  
		Last Modified: Thu, 07 Oct 2021 18:21:26 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da27adaf28f89990b9156f44e7aa987fba745e165e3d77bcb66645fa394c45dc`  
		Last Modified: Thu, 07 Oct 2021 18:21:26 GMT  
		Size: 3.3 KB (3300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a33fc04d83dc027d9d39a63c1aa735851748ea94da41038c6dd23711e831152`  
		Last Modified: Thu, 07 Oct 2021 18:21:33 GMT  
		Size: 113.7 MB (113727914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0cfecb680351bec0f2c6a48de52b17f4059d5381e605253facd873acd86454b`  
		Last Modified: Thu, 07 Oct 2021 18:21:26 GMT  
		Size: 1.7 KB (1712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:latest` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:46e0b04d4e8fc91647ef1e2ecb67b2c41c5e5ddf9a2561b8d1164e9fffb43cd8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **224.0 MB (224023724 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ff07d25ae52d95240b3379f292cd339cc5c7f01d7924a5685cbcbd9c39b79c5f`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Fri, 01 Oct 2021 02:43:40 GMT
ADD file:35e2504756850fc1add00516fa89b0499b59c348457a96708eedb61313e7b25e in / 
# Fri, 01 Oct 2021 02:43:41 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 03:11:18 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Thu, 07 Oct 2021 18:39:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends       curl       gnupg2       mysql-client-core-5.7       openjdk-11-jre-headless       postgresql-client       unzip       zip   && rm -rf /var/lib/apt/lists/*
# Thu, 07 Oct 2021 18:39:55 GMT
RUN mkdir /opt/custom-init.d/
# Thu, 07 Oct 2021 18:39:56 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Thu, 07 Oct 2021 18:39:58 GMT
RUN gpg --keyserver keyserver.ubuntu.com --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Thu, 07 Oct 2021 18:39:58 GMT
ARG BONITA_VERSION
# Thu, 07 Oct 2021 18:39:59 GMT
ARG BRANDING_VERSION
# Thu, 07 Oct 2021 18:39:59 GMT
ARG BONITA_SHA256
# Thu, 07 Oct 2021 18:39:59 GMT
ARG BASE_URL
# Thu, 07 Oct 2021 18:39:59 GMT
ARG BONITA_URL
# Thu, 07 Oct 2021 18:39:59 GMT
ENV BONITA_VERSION=7.13.0
# Thu, 07 Oct 2021 18:39:59 GMT
ENV BRANDING_VERSION=2021.2-u0
# Thu, 07 Oct 2021 18:40:00 GMT
ENV BONITA_SHA256=e4f279765cd729885a4e353d96d1d85c5f69fef63f79183e0ccf3ffaa0cb2417
# Thu, 07 Oct 2021 18:40:00 GMT
ENV ZIP_FILE=BonitaCommunity-2021.2-u0.zip
# Thu, 07 Oct 2021 18:40:00 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Thu, 07 Oct 2021 18:40:00 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.2-u0/BonitaCommunity-2021.2-u0.zip
# Thu, 07 Oct 2021 18:40:01 GMT
RUN mkdir /opt/files
# Thu, 07 Oct 2021 18:40:01 GMT
COPY dir:6250b774ea0abc098d97c259e44608a8bf8835310bd84b47cecb5b027fb6826b in /opt/files 
# Thu, 07 Oct 2021 18:40:07 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi   && sha256sum /opt/files/${ZIP_FILE}   && echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && unzip /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war -d /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita/   && rm /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip
# Thu, 07 Oct 2021 18:40:07 GMT
ENV HTTP_API=false
# Thu, 07 Oct 2021 18:40:08 GMT
VOLUME [/opt/bonita]
# Thu, 07 Oct 2021 18:40:08 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Thu, 07 Oct 2021 18:40:09 GMT
EXPOSE 8080
# Thu, 07 Oct 2021 18:40:09 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:f46992f278c2dd50c481ff60ce8528b6eb59016ac6243e1a7fb385c79c5944b9`  
		Last Modified: Fri, 01 Oct 2021 02:45:30 GMT  
		Size: 23.7 MB (23727476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dc50417f8766e71952102927194ac113f5e2e860c3ff70e83408a76bb03b769`  
		Last Modified: Thu, 07 Oct 2021 18:40:59 GMT  
		Size: 85.6 MB (85633002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cc2b063dc6bebc7066b64b77109b370b3dc8091eec286991a68d9e7b6765129`  
		Last Modified: Thu, 07 Oct 2021 18:40:46 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e44274edbceca1900ba7de25a5a5f7a9195be987ab1ae0f1f5b3f9f7e40e828b`  
		Last Modified: Thu, 07 Oct 2021 18:40:46 GMT  
		Size: 1.9 KB (1887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56aea4ff7509ac8f174916c1b125b5e23ef218b83b8b9f71d2b6db88cda7be72`  
		Last Modified: Thu, 07 Oct 2021 18:40:44 GMT  
		Size: 928.1 KB (928124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4c8d1ec3b6c31dff6298f3288830bfa110ed9224aea1a4a380a975aedf55977`  
		Last Modified: Thu, 07 Oct 2021 18:40:44 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70cb476674d933991b2211ed6f32cfbf43a6e6ca21cebb9b78e78a90988825cd`  
		Last Modified: Thu, 07 Oct 2021 18:40:44 GMT  
		Size: 3.3 KB (3303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9112d52252e5249d5c722bee3bbc779d928730ba0032e26c574cb24cfebc8130`  
		Last Modified: Thu, 07 Oct 2021 18:40:52 GMT  
		Size: 113.7 MB (113727919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1257c5b7ab916e8bc56ed191b582193e3bbca564bca8b00cae30ce2f13f3a314`  
		Last Modified: Thu, 07 Oct 2021 18:40:44 GMT  
		Size: 1.7 KB (1709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:latest` - linux; ppc64le

```console
$ docker pull bonita@sha256:8f84286a16f847ace8b3ba19ce8ad3610d7cee0ee4fe2949cb336a18dd5a32e9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **231.5 MB (231509285 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e940107c65dc134dd59beb4e8fd39205865773d8dee6a0452f3d2436591ac92`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Tue, 05 Oct 2021 11:07:29 GMT
ADD file:fd96554dfb72307c3cf9292c343050a8b9f0848735b7555820f0068914ebd758 in / 
# Tue, 05 Oct 2021 11:07:35 GMT
CMD ["bash"]
# Wed, 06 Oct 2021 17:43:30 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Thu, 07 Oct 2021 19:19:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends       curl       gnupg2       mysql-client-core-5.7       openjdk-11-jre-headless       postgresql-client       unzip       zip   && rm -rf /var/lib/apt/lists/*
# Thu, 07 Oct 2021 19:20:09 GMT
RUN mkdir /opt/custom-init.d/
# Thu, 07 Oct 2021 19:20:16 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Thu, 07 Oct 2021 19:20:37 GMT
RUN gpg --keyserver keyserver.ubuntu.com --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Thu, 07 Oct 2021 19:20:44 GMT
ARG BONITA_VERSION
# Thu, 07 Oct 2021 19:20:50 GMT
ARG BRANDING_VERSION
# Thu, 07 Oct 2021 19:20:53 GMT
ARG BONITA_SHA256
# Thu, 07 Oct 2021 19:20:57 GMT
ARG BASE_URL
# Thu, 07 Oct 2021 19:21:00 GMT
ARG BONITA_URL
# Thu, 07 Oct 2021 19:21:01 GMT
ENV BONITA_VERSION=7.13.0
# Thu, 07 Oct 2021 19:21:05 GMT
ENV BRANDING_VERSION=2021.2-u0
# Thu, 07 Oct 2021 19:21:11 GMT
ENV BONITA_SHA256=e4f279765cd729885a4e353d96d1d85c5f69fef63f79183e0ccf3ffaa0cb2417
# Thu, 07 Oct 2021 19:21:15 GMT
ENV ZIP_FILE=BonitaCommunity-2021.2-u0.zip
# Thu, 07 Oct 2021 19:21:18 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Thu, 07 Oct 2021 19:21:20 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.2-u0/BonitaCommunity-2021.2-u0.zip
# Thu, 07 Oct 2021 19:21:26 GMT
RUN mkdir /opt/files
# Thu, 07 Oct 2021 19:21:28 GMT
COPY dir:6250b774ea0abc098d97c259e44608a8bf8835310bd84b47cecb5b027fb6826b in /opt/files 
# Thu, 07 Oct 2021 19:21:44 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi   && sha256sum /opt/files/${ZIP_FILE}   && echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && unzip /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war -d /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita/   && rm /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip
# Thu, 07 Oct 2021 19:21:49 GMT
ENV HTTP_API=false
# Thu, 07 Oct 2021 19:21:57 GMT
VOLUME [/opt/bonita]
# Thu, 07 Oct 2021 19:21:58 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Thu, 07 Oct 2021 19:22:03 GMT
EXPOSE 8080
# Thu, 07 Oct 2021 19:22:09 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:db28fc1e594e5598e665c54ac1b7fd602d86dddaf8bb237a72303cec22a9185c`  
		Last Modified: Tue, 05 Oct 2021 11:10:31 GMT  
		Size: 30.4 MB (30432921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17d89d6ede66e22e682b17c5fb5b2665ee97d7f7d155861dda91815620662729`  
		Last Modified: Thu, 07 Oct 2021 19:23:14 GMT  
		Size: 86.4 MB (86437046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:008fce009be160a4fe12d228556c91a26fda3281f23c16ec6136dea0a080ad37`  
		Last Modified: Thu, 07 Oct 2021 19:22:59 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4a62824290cee741a0aeb9676745be2c616eaa8dcd4ce7b949df063b35a1e16`  
		Last Modified: Thu, 07 Oct 2021 19:22:59 GMT  
		Size: 1.9 KB (1883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdc3250c10bd3ceef93513e091b435d9897e902f8ea3ea62f967eb4dc76a75b7`  
		Last Modified: Thu, 07 Oct 2021 19:22:57 GMT  
		Size: 904.2 KB (904197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0e4b367f2ce3d9341f43a189bb7c26cbf78cc7c571661df9d2d1793e1ef2914`  
		Last Modified: Thu, 07 Oct 2021 19:22:57 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:045f6914c214de6daae2dd2e975b43ded87b3e54adb9560308f7769d1607bea7`  
		Last Modified: Thu, 07 Oct 2021 19:22:57 GMT  
		Size: 3.3 KB (3308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73e28e1cffdb6e7a72d3e63da9a49539242b8d4fa50dbecec5ff825c8942f0a6`  
		Last Modified: Thu, 07 Oct 2021 19:23:07 GMT  
		Size: 113.7 MB (113727917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccc8bb2f32fefca639b2ccaffdf8d9cf883c5d510e0093ee31525ccbbf1df8d5`  
		Last Modified: Thu, 07 Oct 2021 19:22:57 GMT  
		Size: 1.7 KB (1709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
