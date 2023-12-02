## `clojure:temurin-17-boot-bookworm`

```console
$ docker pull clojure@sha256:dbeb1c614ea52bc80a4354617a09948ecb603dfa3a6e80aa088747f78cf0b02a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-17-boot-bookworm` - linux; amd64

```console
$ docker pull clojure@sha256:62a97297528cc69e198a08ecd22cb8c656c53399df2046a818f6e61f2f5024f2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **258.8 MB (258807232 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ed7a1470bdc86503b767f321bb8f416acd1a1649939474159e4b140053f38e7`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Tue, 21 Nov 2023 05:21:24 GMT
ADD file:39d17d28c5de0bd629e5b7c8190228e5a445d61d668e189b7523e90e68f78244 in / 
# Tue, 21 Nov 2023 05:21:25 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 10:07:35 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 21 Nov 2023 10:18:47 GMT
COPY dir:33a61da93c3e1252ff87d5fd5f9955ca53f9f7f200758827548096d130b4307b in /opt/java/openjdk 
# Tue, 21 Nov 2023 10:18:48 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Nov 2023 10:18:48 GMT
ENV BOOT_VERSION=2.8.3
# Tue, 21 Nov 2023 10:18:48 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Tue, 21 Nov 2023 10:18:48 GMT
WORKDIR /tmp
# Tue, 21 Nov 2023 10:18:54 GMT
RUN apt-get update && apt-get install -y make wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Tue, 21 Nov 2023 10:18:54 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Tue, 21 Nov 2023 10:18:54 GMT
ENV BOOT_AS_ROOT=yes
# Tue, 21 Nov 2023 10:19:11 GMT
RUN boot
# Tue, 21 Nov 2023 10:19:12 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Tue, 21 Nov 2023 10:19:12 GMT
ENTRYPOINT ["entrypoint"]
# Tue, 21 Nov 2023 10:19:12 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:90e5e7d8b87a34877f61c2b86d053db1c4f440b9054cf49573e3be5d6a674a47`  
		Last Modified: Tue, 21 Nov 2023 05:25:34 GMT  
		Size: 49.6 MB (49582225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:584a59c8aee6beabb9a28978d412b9cda10c78ebfad3f1537ffb2d4299e1e9b0`  
		Last Modified: Tue, 21 Nov 2023 10:35:15 GMT  
		Size: 144.9 MB (144873904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b98ba6a4a2e52463c699ee5e38db12141a44f1770408e20c956915901bf4d037`  
		Last Modified: Tue, 21 Nov 2023 10:35:05 GMT  
		Size: 5.5 MB (5530348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bf26582829883de429ca0ab047f02484540d33c34ed06f0adb4312555e64085`  
		Last Modified: Tue, 21 Nov 2023 10:35:07 GMT  
		Size: 58.8 MB (58820356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c228d95ad7e7d8068d234fdae54c083e0d376c467a330672405e5473583df40c`  
		Last Modified: Tue, 21 Nov 2023 10:35:03 GMT  
		Size: 399.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-17-boot-bookworm` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:06604be2eaa776e87d6d1f56fe553b03d55f05dc0576014d0e031b7610b7b7eb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **257.5 MB (257468725 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9506087ec734f9451f390a9bb9ac6c891e58df105401b70ea5a0a0f1aaef15cc`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Tue, 21 Nov 2023 06:26:54 GMT
ADD file:6550a7c17e64067114283d098e85f9a74d4707f2879b53c2e4cae99f329c9025 in / 
# Tue, 21 Nov 2023 06:26:55 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 07:20:15 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sat, 02 Dec 2023 08:52:59 GMT
COPY dir:b97789a1c2e6d715436236e063679209ed5b51287e172faadc90d7cbd7bc1135 in /opt/java/openjdk 
# Sat, 02 Dec 2023 08:53:03 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 02 Dec 2023 08:53:03 GMT
ENV BOOT_VERSION=2.8.3
# Sat, 02 Dec 2023 08:53:03 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Sat, 02 Dec 2023 08:53:03 GMT
WORKDIR /tmp
# Sat, 02 Dec 2023 08:53:08 GMT
RUN apt-get update && apt-get install -y make wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Sat, 02 Dec 2023 08:53:08 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Sat, 02 Dec 2023 08:53:08 GMT
ENV BOOT_AS_ROOT=yes
# Sat, 02 Dec 2023 08:53:25 GMT
RUN boot
# Sat, 02 Dec 2023 08:53:25 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Sat, 02 Dec 2023 08:53:25 GMT
ENTRYPOINT ["entrypoint"]
# Sat, 02 Dec 2023 08:53:25 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:df2021ddb7d686bdbb125598b2a6163d63035f080356b3014595f354ea0b40d6`  
		Last Modified: Tue, 21 Nov 2023 06:30:07 GMT  
		Size: 49.6 MB (49612650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36f02d73e685ee8484944282e77adf6fe8d1c76564b2f529abde1e7d5f24493f`  
		Last Modified: Sat, 02 Dec 2023 09:07:54 GMT  
		Size: 143.7 MB (143681757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f429cd9ce65ad3f82b89d1dea37317d8ed9acaadfc8c56ab1e9f7fa1ee2e2c78`  
		Last Modified: Sat, 02 Dec 2023 09:07:45 GMT  
		Size: 5.4 MB (5353323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81fb4845db719ffa01afa257b081d5c3fa8001080f6d0ff02a50dc9b0a3fb452`  
		Last Modified: Sat, 02 Dec 2023 09:07:47 GMT  
		Size: 58.8 MB (58820594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d03b83b4e12ed6e67a4bf0c97cf42a1fae52f4ee22949b5516dbe4fd3584226`  
		Last Modified: Sat, 02 Dec 2023 09:07:44 GMT  
		Size: 401.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
