## `dart:stable`

```console
$ docker pull dart@sha256:c43ba4eab9a9bcf98dd696325161dc404c1f9113afa7523a9fc6ded7d4753fe7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `dart:stable` - linux; amd64

```console
$ docker pull dart@sha256:c5e7f2d3aba811cb7bfbcd9ebc2d09f216cf3a70241111673bf8800e6092ef03
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **289.1 MB (289067021 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dafa97570ca67acf6ea6175168d0f77e317878fe4fa1eb2be9700fc4dafc2280`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Oct 2021 01:21:05 GMT
ADD file:910392427fdf089bc26b64d6dc450ff3d020c7c1a474d85b2f9298134d0007bd in / 
# Tue, 12 Oct 2021 01:21:05 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 09:48:58 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 09:48:59 GMT
RUN set -eux;     for f in         /etc/nsswitch.conf         /etc/ssl/certs         /lib/x86_64-linux-gnu/libc.so.6         /lib/x86_64-linux-gnu/libdl.so.2         /lib/x86_64-linux-gnu/libm.so.6         /lib/x86_64-linux-gnu/libnss_dns.so.2         /lib/x86_64-linux-gnu/libpthread.so.0         /lib/x86_64-linux-gnu/libresolv.so.2         /lib/x86_64-linux-gnu/librt.so.1         /lib64/ld-linux-x86-64.so.2         /usr/share/ca-certificates     ; do         dir="$(dirname "$f")";         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 12 Oct 2021 09:49:00 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 12 Oct 2021 09:49:00 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Oct 2021 09:49:00 GMT
WORKDIR /root
# Thu, 14 Oct 2021 19:28:10 GMT
RUN set -eux;     ARCH=$(case "$(dpkg --print-architecture)" in amd64) echo "x64";; esac;);     SDK="dartsdk-linux-$ARCH-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.14.4/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "49b6a98008ef546cb9c221461529d6c02cf2474bff098e0dc7e4ff1ef0f8a289 *$SDK"     | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK";
```

-	Layers:
	-	`sha256:b380bbd43752f83945df8b5d1074fef8dd044820e7d3aef33b655a2483e030c7`  
		Last Modified: Tue, 12 Oct 2021 01:26:51 GMT  
		Size: 27.1 MB (27139510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c0967f1c7a0cff360e1b4b316d95f992ede8dd65a5ce3d015aeabaad78b097d`  
		Last Modified: Tue, 12 Oct 2021 09:50:01 GMT  
		Size: 49.6 MB (49582550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b872aeb4f5e62a618c7ffe96a15e50654b6f1cbf9539b6756b5302f93a0c928`  
		Last Modified: Tue, 12 Oct 2021 09:49:53 GMT  
		Size: 2.4 MB (2359146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e380f9d37c3826f39569576a6f6cb872d7b55a1d9149f8a6fc343831ce619c44`  
		Last Modified: Thu, 14 Oct 2021 19:29:15 GMT  
		Size: 210.0 MB (209985815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
