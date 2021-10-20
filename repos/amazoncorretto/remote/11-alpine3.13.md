## `amazoncorretto:11-alpine3.13`

```console
$ docker pull amazoncorretto@sha256:5cc7f4f85fa57b598b872354d3dc35805c791e6caaa91f8058e4f8eab5f7b52b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazoncorretto:11-alpine3.13` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:aaede93ee5537dbbec275662d3a3b969aa09774e4ee4b425800f0dffb4908b4b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **196.1 MB (196136914 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dce29dc9c79b2c09ee0d013caa750bf53bcdec203e013787265a76246cacece7`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 31 Aug 2021 23:18:16 GMT
ADD file:ecdfb91a737d6c292265c1b77ffd3d82ba810dd43ea4ef79714b66b1da74a5aa in / 
# Tue, 31 Aug 2021 23:18:16 GMT
CMD ["/bin/sh"]
# Wed, 20 Oct 2021 18:21:10 GMT
ARG version=11.0.13.8.1
# Wed, 20 Oct 2021 18:21:16 GMT
# ARGS: version=11.0.13.8.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-11=$version-r0
# Wed, 20 Oct 2021 18:21:16 GMT
ENV LANG=C.UTF-8
# Wed, 20 Oct 2021 18:21:17 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Wed, 20 Oct 2021 18:21:17 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:4e9f2cdf438714c2c4533e28c6c41a89cc6c1b46cf77e54c488db30ca4f5b6f3`  
		Last Modified: Tue, 31 Aug 2021 23:18:55 GMT  
		Size: 2.8 MB (2814079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e341d136aa16dfd5dcf1bfe106c87461fb0ee94580d27f5d3aeedf02d500daf`  
		Last Modified: Wed, 20 Oct 2021 18:27:04 GMT  
		Size: 193.3 MB (193322835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
