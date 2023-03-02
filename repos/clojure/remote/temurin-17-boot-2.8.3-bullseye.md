## `clojure:temurin-17-boot-2.8.3-bullseye`

```console
$ docker pull clojure@sha256:9e85705ce5a2583c4784baf4bef90af200120f619438b8c621cb0a7765a626b1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-17-boot-2.8.3-bullseye` - linux; amd64

```console
$ docker pull clojure@sha256:8857bc037344a04b30acc2baf6f5bf36bbfb6919100433513c893c6a1918c498
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **308.7 MB (308666284 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:63e0898835540939f37c24cea0e1fc6f348bc69099967a7314f629e8e91d17c3`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Wed, 01 Mar 2023 04:09:45 GMT
ADD file:513c5d5e501279c21a05c1d8b66e5f0b02ee4b27f0b928706d92fd9ce11c1be6 in / 
# Wed, 01 Mar 2023 04:09:46 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 07:40:41 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 01 Mar 2023 07:46:48 GMT
COPY dir:5cf52f938fe415b0022fbccb8cf978562c503c0b8313cc9dedf46c1c4edb35cf in /opt/java/openjdk 
# Wed, 01 Mar 2023 07:46:49 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Mar 2023 07:46:49 GMT
ENV BOOT_VERSION=2.8.3
# Wed, 01 Mar 2023 07:46:49 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Wed, 01 Mar 2023 07:46:50 GMT
WORKDIR /tmp
# Wed, 01 Mar 2023 07:46:55 GMT
RUN apt-get update && apt-get install -y make wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Wed, 01 Mar 2023 07:46:55 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Wed, 01 Mar 2023 07:46:55 GMT
ENV BOOT_AS_ROOT=yes
# Wed, 01 Mar 2023 07:47:13 GMT
RUN boot
# Wed, 01 Mar 2023 07:47:13 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Wed, 01 Mar 2023 07:47:13 GMT
ENTRYPOINT ["entrypoint"]
# Wed, 01 Mar 2023 07:47:13 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:32fb02163b6bb519a30f909008e852354dae10bdfd6b34190dbdfe8f15403ea0`  
		Last Modified: Wed, 01 Mar 2023 04:13:58 GMT  
		Size: 55.0 MB (55045922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e2398cb32ac1a57ed5e07eacb837ab8e304b5c7c8726bc0e525810f442bb47c`  
		Last Modified: Wed, 01 Mar 2023 07:58:35 GMT  
		Size: 192.4 MB (192438071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b287ca4bbd790d594f8ba5070b55e4c2f604c2839c9093f53a813e973517e3f7`  
		Last Modified: Wed, 01 Mar 2023 07:58:21 GMT  
		Size: 2.4 MB (2361569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5de3213985b9bdefcfb642c991e9f1cc455f4cdf71da3df25ca35e915d27af55`  
		Last Modified: Wed, 01 Mar 2023 07:58:24 GMT  
		Size: 58.8 MB (58820322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47428a5d9277ccf7210bd8114735d99e72dbb8d41f1d313e7253f14d8ba234e8`  
		Last Modified: Wed, 01 Mar 2023 07:58:20 GMT  
		Size: 400.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-17-boot-2.8.3-bullseye` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:f652aa3666a3e2b7bbdae1b33aa2f8352688c21e05122c7566017cb0855658c3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **306.1 MB (306135724 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eec642b0729a773838f30027ff7e81a9225f70d6749ee8adb29029a70a64b5a0`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Wed, 01 Mar 2023 02:20:30 GMT
ADD file:a6a1df499d0d5b07fb366d776a11c42ddee6261e2425a921041b38e868192770 in / 
# Wed, 01 Mar 2023 02:20:30 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 03:01:14 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 02 Mar 2023 07:06:32 GMT
COPY dir:47c117bbc947c5c1164b5a20eeec0ba16c306f5991a85f22c54db31ca24ce4a8 in /opt/java/openjdk 
# Thu, 02 Mar 2023 07:06:36 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 02 Mar 2023 07:06:36 GMT
ENV BOOT_VERSION=2.8.3
# Thu, 02 Mar 2023 07:06:36 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Thu, 02 Mar 2023 07:06:36 GMT
WORKDIR /tmp
# Thu, 02 Mar 2023 07:06:41 GMT
RUN apt-get update && apt-get install -y make wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Thu, 02 Mar 2023 07:06:41 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Thu, 02 Mar 2023 07:06:41 GMT
ENV BOOT_AS_ROOT=yes
# Thu, 02 Mar 2023 07:06:58 GMT
RUN boot
# Thu, 02 Mar 2023 07:06:59 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Thu, 02 Mar 2023 07:06:59 GMT
ENTRYPOINT ["entrypoint"]
# Thu, 02 Mar 2023 07:06:59 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:0f5fe16b1836feccd4765ac5685fc7a7b9c73445cac94fc595d2ffbc3cb59a7a`  
		Last Modified: Wed, 01 Mar 2023 02:23:53 GMT  
		Size: 53.7 MB (53703215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6d4bb35cb769be425f0d1c938b7ff57112e361f17e432495be72cb2032f4d92`  
		Last Modified: Thu, 02 Mar 2023 07:20:00 GMT  
		Size: 191.3 MB (191260440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6ad538cbfa3ca3cda6ff54422768d6c0750cee9d8560f044d5c5c77086d17fc`  
		Last Modified: Thu, 02 Mar 2023 07:19:50 GMT  
		Size: 2.4 MB (2351070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c18970ebe7e7190e5dade8940e35f7f5d390215908fdf1c3ac20b7000ce4121`  
		Last Modified: Thu, 02 Mar 2023 07:19:53 GMT  
		Size: 58.8 MB (58820598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:881a1fd110a14425007f14e3311c9f0a25390623f9e0278c8a31ab48ca8d65d2`  
		Last Modified: Thu, 02 Mar 2023 07:19:49 GMT  
		Size: 401.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
