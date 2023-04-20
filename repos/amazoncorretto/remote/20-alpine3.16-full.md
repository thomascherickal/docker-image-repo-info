## `amazoncorretto:20-alpine3.16-full`

```console
$ docker pull amazoncorretto@sha256:54cb4295292ad317420887d5ff53ee8327923e7b6b899cd36dd705caeba3ca0e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:20-alpine3.16-full` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:30813ea522e4a3107a9c49058593bcbfbabc9a8b541f3f69e086693caedc3005
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **206.5 MB (206535716 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd1226c058ef1c4cdaba485f1f8f22dbc9eb3f1076b82856745c58be6b5f593a`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:28 GMT
ADD file:970e6b2578ef73457ffed1189e8ba128b0211cabd3174b8c7d3afd8fb58ad614 in / 
# Wed, 29 Mar 2023 18:19:28 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 19:20:08 GMT
ARG version=20.0.0.36.1
# Wed, 29 Mar 2023 19:20:13 GMT
# ARGS: version=20.0.0.36.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-20=$version-r0
# Wed, 29 Mar 2023 19:20:14 GMT
ENV LANG=C.UTF-8
# Wed, 29 Mar 2023 19:20:14 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Wed, 29 Mar 2023 19:20:14 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:91d30c5bc19582de1415b18f1ec5bcbf52a558b62cf6cc201c9669df9f748c22`  
		Last Modified: Wed, 29 Mar 2023 18:20:09 GMT  
		Size: 2.8 MB (2807803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:056315cc7de389ed5d0f45582ce8d7e6d8971e940d4de65194a57ffd3649b995`  
		Last Modified: Wed, 29 Mar 2023 19:30:36 GMT  
		Size: 203.7 MB (203727913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:20-alpine3.16-full` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:dba639f357e18b6798bb9553d979db18eb076474c3183f26877752396e3d9d4d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **204.4 MB (204441295 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b599b817801a50cb89a6a928299eee521141ed929c04cb7d215bfd6267429846`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 29 Mar 2023 17:39:20 GMT
ADD file:a6a2f69b60d7d27bc6e2b9b7e9910dabdc3f5e3702c2345d26a7dc8c603ae595 in / 
# Wed, 29 Mar 2023 17:39:20 GMT
CMD ["/bin/sh"]
# Thu, 20 Apr 2023 17:45:28 GMT
ARG version=20.0.1.9.1
# Thu, 20 Apr 2023 17:45:33 GMT
# ARGS: version=20.0.1.9.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-20=$version-r0
# Thu, 20 Apr 2023 17:45:35 GMT
ENV LANG=C.UTF-8
# Thu, 20 Apr 2023 17:45:35 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Thu, 20 Apr 2023 17:45:36 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:547446be3368f442c50ff95e2a2a9c85110b6b41bbb3c75b7e5ebb115f478b57`  
		Last Modified: Wed, 29 Mar 2023 17:39:56 GMT  
		Size: 2.7 MB (2709344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5da6200fbe5de2d08d5465ebed13ab1ad7632232f8e1e52d57b69e2ab74f136b`  
		Last Modified: Thu, 20 Apr 2023 17:57:36 GMT  
		Size: 201.7 MB (201731951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
