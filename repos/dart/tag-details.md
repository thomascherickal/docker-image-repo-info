<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `dart`

-	[`dart:2`](#dart2)
-	[`dart:2-sdk`](#dart2-sdk)
-	[`dart:2.14`](#dart214)
-	[`dart:2.14-sdk`](#dart214-sdk)
-	[`dart:2.14.3`](#dart2143)
-	[`dart:2.14.3-sdk`](#dart2143-sdk)
-	[`dart:2.15.0-82.2.beta`](#dart2150-822beta)
-	[`dart:2.15.0-82.2.beta-sdk`](#dart2150-822beta-sdk)
-	[`dart:beta`](#dartbeta)
-	[`dart:beta-sdk`](#dartbeta-sdk)
-	[`dart:latest`](#dartlatest)
-	[`dart:sdk`](#dartsdk)
-	[`dart:stable`](#dartstable)
-	[`dart:stable-sdk`](#dartstable-sdk)

## `dart:2`

```console
$ docker pull dart@sha256:4f321ebb13ee952810c7dab53e8439547dd0e413c827b382a7f2b5b3cd447da3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `dart:2` - linux; amd64

```console
$ docker pull dart@sha256:398c325b807d3d0481c7b0b3249d8d0db26263b6ad15b8bda93188255938d9cc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **289.1 MB (289063576 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a541608b7bdf2e8455d39e762bd0b61bcf72438a12a0f41d8a692e1e513481d6`
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
# Tue, 12 Oct 2021 09:49:13 GMT
RUN set -eux;     ARCH=$(case "$(dpkg --print-architecture)" in amd64) echo "x64";; esac;);     SDK="dartsdk-linux-$ARCH-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.14.3/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "cad36ec238af96c8048bbcec4cff7e69fcb1b895620010ca1762674ca4ade171 *$SDK"     | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK";
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
	-	`sha256:d2d33d8b9592194e7f0147e607d97c522691a0b68850ee994e112126dba7975e`  
		Last Modified: Tue, 12 Oct 2021 09:50:24 GMT  
		Size: 210.0 MB (209982370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:2-sdk`

```console
$ docker pull dart@sha256:4f321ebb13ee952810c7dab53e8439547dd0e413c827b382a7f2b5b3cd447da3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `dart:2-sdk` - linux; amd64

```console
$ docker pull dart@sha256:398c325b807d3d0481c7b0b3249d8d0db26263b6ad15b8bda93188255938d9cc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **289.1 MB (289063576 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a541608b7bdf2e8455d39e762bd0b61bcf72438a12a0f41d8a692e1e513481d6`
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
# Tue, 12 Oct 2021 09:49:13 GMT
RUN set -eux;     ARCH=$(case "$(dpkg --print-architecture)" in amd64) echo "x64";; esac;);     SDK="dartsdk-linux-$ARCH-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.14.3/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "cad36ec238af96c8048bbcec4cff7e69fcb1b895620010ca1762674ca4ade171 *$SDK"     | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK";
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
	-	`sha256:d2d33d8b9592194e7f0147e607d97c522691a0b68850ee994e112126dba7975e`  
		Last Modified: Tue, 12 Oct 2021 09:50:24 GMT  
		Size: 210.0 MB (209982370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:2.14`

```console
$ docker pull dart@sha256:4f321ebb13ee952810c7dab53e8439547dd0e413c827b382a7f2b5b3cd447da3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `dart:2.14` - linux; amd64

```console
$ docker pull dart@sha256:398c325b807d3d0481c7b0b3249d8d0db26263b6ad15b8bda93188255938d9cc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **289.1 MB (289063576 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a541608b7bdf2e8455d39e762bd0b61bcf72438a12a0f41d8a692e1e513481d6`
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
# Tue, 12 Oct 2021 09:49:13 GMT
RUN set -eux;     ARCH=$(case "$(dpkg --print-architecture)" in amd64) echo "x64";; esac;);     SDK="dartsdk-linux-$ARCH-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.14.3/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "cad36ec238af96c8048bbcec4cff7e69fcb1b895620010ca1762674ca4ade171 *$SDK"     | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK";
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
	-	`sha256:d2d33d8b9592194e7f0147e607d97c522691a0b68850ee994e112126dba7975e`  
		Last Modified: Tue, 12 Oct 2021 09:50:24 GMT  
		Size: 210.0 MB (209982370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:2.14-sdk`

```console
$ docker pull dart@sha256:4f321ebb13ee952810c7dab53e8439547dd0e413c827b382a7f2b5b3cd447da3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `dart:2.14-sdk` - linux; amd64

```console
$ docker pull dart@sha256:398c325b807d3d0481c7b0b3249d8d0db26263b6ad15b8bda93188255938d9cc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **289.1 MB (289063576 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a541608b7bdf2e8455d39e762bd0b61bcf72438a12a0f41d8a692e1e513481d6`
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
# Tue, 12 Oct 2021 09:49:13 GMT
RUN set -eux;     ARCH=$(case "$(dpkg --print-architecture)" in amd64) echo "x64";; esac;);     SDK="dartsdk-linux-$ARCH-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.14.3/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "cad36ec238af96c8048bbcec4cff7e69fcb1b895620010ca1762674ca4ade171 *$SDK"     | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK";
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
	-	`sha256:d2d33d8b9592194e7f0147e607d97c522691a0b68850ee994e112126dba7975e`  
		Last Modified: Tue, 12 Oct 2021 09:50:24 GMT  
		Size: 210.0 MB (209982370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:2.14.3`

```console
$ docker pull dart@sha256:4f321ebb13ee952810c7dab53e8439547dd0e413c827b382a7f2b5b3cd447da3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `dart:2.14.3` - linux; amd64

```console
$ docker pull dart@sha256:398c325b807d3d0481c7b0b3249d8d0db26263b6ad15b8bda93188255938d9cc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **289.1 MB (289063576 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a541608b7bdf2e8455d39e762bd0b61bcf72438a12a0f41d8a692e1e513481d6`
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
# Tue, 12 Oct 2021 09:49:13 GMT
RUN set -eux;     ARCH=$(case "$(dpkg --print-architecture)" in amd64) echo "x64";; esac;);     SDK="dartsdk-linux-$ARCH-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.14.3/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "cad36ec238af96c8048bbcec4cff7e69fcb1b895620010ca1762674ca4ade171 *$SDK"     | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK";
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
	-	`sha256:d2d33d8b9592194e7f0147e607d97c522691a0b68850ee994e112126dba7975e`  
		Last Modified: Tue, 12 Oct 2021 09:50:24 GMT  
		Size: 210.0 MB (209982370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:2.14.3-sdk`

```console
$ docker pull dart@sha256:4f321ebb13ee952810c7dab53e8439547dd0e413c827b382a7f2b5b3cd447da3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `dart:2.14.3-sdk` - linux; amd64

```console
$ docker pull dart@sha256:398c325b807d3d0481c7b0b3249d8d0db26263b6ad15b8bda93188255938d9cc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **289.1 MB (289063576 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a541608b7bdf2e8455d39e762bd0b61bcf72438a12a0f41d8a692e1e513481d6`
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
# Tue, 12 Oct 2021 09:49:13 GMT
RUN set -eux;     ARCH=$(case "$(dpkg --print-architecture)" in amd64) echo "x64";; esac;);     SDK="dartsdk-linux-$ARCH-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.14.3/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "cad36ec238af96c8048bbcec4cff7e69fcb1b895620010ca1762674ca4ade171 *$SDK"     | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK";
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
	-	`sha256:d2d33d8b9592194e7f0147e607d97c522691a0b68850ee994e112126dba7975e`  
		Last Modified: Tue, 12 Oct 2021 09:50:24 GMT  
		Size: 210.0 MB (209982370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:2.15.0-82.2.beta`

```console
$ docker pull dart@sha256:f169fa8c0db9b1ef1b5a169b58a50f0dc4d0119312a9d90b69c8a3afb21c2dae
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `dart:2.15.0-82.2.beta` - linux; amd64

```console
$ docker pull dart@sha256:adcf2affa501ab0abf1999a0b47678916006a8de6cb6907c5d8b8b090f5137f1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **280.4 MB (280351762 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e6ec45b28777157cbc146ce1785393332368229dbae8a081be428cd2ae1f1d1`
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
# Tue, 12 Oct 2021 09:49:31 GMT
RUN set -eux;     ARCH=$(case "$(dpkg --print-architecture)" in amd64) echo "x64";; esac;);     SDK="dartsdk-linux-$ARCH-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/2.15.0-82.2.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "3f23b4ca6d7ffeadad21cd69577eabcfb5d872cbd005f04b5d4f58c1866dcf04 *$SDK"     | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK";
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
	-	`sha256:6aeaad304f6dfa13e8130b1de4eb81625045bc83f8ab2f6fe4424c8805346d6a`  
		Last Modified: Tue, 12 Oct 2021 09:51:22 GMT  
		Size: 201.3 MB (201270556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:2.15.0-82.2.beta-sdk`

```console
$ docker pull dart@sha256:f169fa8c0db9b1ef1b5a169b58a50f0dc4d0119312a9d90b69c8a3afb21c2dae
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `dart:2.15.0-82.2.beta-sdk` - linux; amd64

```console
$ docker pull dart@sha256:adcf2affa501ab0abf1999a0b47678916006a8de6cb6907c5d8b8b090f5137f1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **280.4 MB (280351762 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e6ec45b28777157cbc146ce1785393332368229dbae8a081be428cd2ae1f1d1`
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
# Tue, 12 Oct 2021 09:49:31 GMT
RUN set -eux;     ARCH=$(case "$(dpkg --print-architecture)" in amd64) echo "x64";; esac;);     SDK="dartsdk-linux-$ARCH-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/2.15.0-82.2.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "3f23b4ca6d7ffeadad21cd69577eabcfb5d872cbd005f04b5d4f58c1866dcf04 *$SDK"     | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK";
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
	-	`sha256:6aeaad304f6dfa13e8130b1de4eb81625045bc83f8ab2f6fe4424c8805346d6a`  
		Last Modified: Tue, 12 Oct 2021 09:51:22 GMT  
		Size: 201.3 MB (201270556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:beta`

```console
$ docker pull dart@sha256:f169fa8c0db9b1ef1b5a169b58a50f0dc4d0119312a9d90b69c8a3afb21c2dae
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `dart:beta` - linux; amd64

```console
$ docker pull dart@sha256:adcf2affa501ab0abf1999a0b47678916006a8de6cb6907c5d8b8b090f5137f1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **280.4 MB (280351762 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e6ec45b28777157cbc146ce1785393332368229dbae8a081be428cd2ae1f1d1`
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
# Tue, 12 Oct 2021 09:49:31 GMT
RUN set -eux;     ARCH=$(case "$(dpkg --print-architecture)" in amd64) echo "x64";; esac;);     SDK="dartsdk-linux-$ARCH-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/2.15.0-82.2.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "3f23b4ca6d7ffeadad21cd69577eabcfb5d872cbd005f04b5d4f58c1866dcf04 *$SDK"     | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK";
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
	-	`sha256:6aeaad304f6dfa13e8130b1de4eb81625045bc83f8ab2f6fe4424c8805346d6a`  
		Last Modified: Tue, 12 Oct 2021 09:51:22 GMT  
		Size: 201.3 MB (201270556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:beta-sdk`

```console
$ docker pull dart@sha256:f169fa8c0db9b1ef1b5a169b58a50f0dc4d0119312a9d90b69c8a3afb21c2dae
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `dart:beta-sdk` - linux; amd64

```console
$ docker pull dart@sha256:adcf2affa501ab0abf1999a0b47678916006a8de6cb6907c5d8b8b090f5137f1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **280.4 MB (280351762 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e6ec45b28777157cbc146ce1785393332368229dbae8a081be428cd2ae1f1d1`
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
# Tue, 12 Oct 2021 09:49:31 GMT
RUN set -eux;     ARCH=$(case "$(dpkg --print-architecture)" in amd64) echo "x64";; esac;);     SDK="dartsdk-linux-$ARCH-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/2.15.0-82.2.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "3f23b4ca6d7ffeadad21cd69577eabcfb5d872cbd005f04b5d4f58c1866dcf04 *$SDK"     | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK";
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
	-	`sha256:6aeaad304f6dfa13e8130b1de4eb81625045bc83f8ab2f6fe4424c8805346d6a`  
		Last Modified: Tue, 12 Oct 2021 09:51:22 GMT  
		Size: 201.3 MB (201270556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:latest`

```console
$ docker pull dart@sha256:4f321ebb13ee952810c7dab53e8439547dd0e413c827b382a7f2b5b3cd447da3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `dart:latest` - linux; amd64

```console
$ docker pull dart@sha256:398c325b807d3d0481c7b0b3249d8d0db26263b6ad15b8bda93188255938d9cc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **289.1 MB (289063576 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a541608b7bdf2e8455d39e762bd0b61bcf72438a12a0f41d8a692e1e513481d6`
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
# Tue, 12 Oct 2021 09:49:13 GMT
RUN set -eux;     ARCH=$(case "$(dpkg --print-architecture)" in amd64) echo "x64";; esac;);     SDK="dartsdk-linux-$ARCH-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.14.3/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "cad36ec238af96c8048bbcec4cff7e69fcb1b895620010ca1762674ca4ade171 *$SDK"     | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK";
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
	-	`sha256:d2d33d8b9592194e7f0147e607d97c522691a0b68850ee994e112126dba7975e`  
		Last Modified: Tue, 12 Oct 2021 09:50:24 GMT  
		Size: 210.0 MB (209982370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:sdk`

```console
$ docker pull dart@sha256:4f321ebb13ee952810c7dab53e8439547dd0e413c827b382a7f2b5b3cd447da3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `dart:sdk` - linux; amd64

```console
$ docker pull dart@sha256:398c325b807d3d0481c7b0b3249d8d0db26263b6ad15b8bda93188255938d9cc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **289.1 MB (289063576 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a541608b7bdf2e8455d39e762bd0b61bcf72438a12a0f41d8a692e1e513481d6`
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
# Tue, 12 Oct 2021 09:49:13 GMT
RUN set -eux;     ARCH=$(case "$(dpkg --print-architecture)" in amd64) echo "x64";; esac;);     SDK="dartsdk-linux-$ARCH-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.14.3/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "cad36ec238af96c8048bbcec4cff7e69fcb1b895620010ca1762674ca4ade171 *$SDK"     | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK";
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
	-	`sha256:d2d33d8b9592194e7f0147e607d97c522691a0b68850ee994e112126dba7975e`  
		Last Modified: Tue, 12 Oct 2021 09:50:24 GMT  
		Size: 210.0 MB (209982370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:stable`

```console
$ docker pull dart@sha256:4f321ebb13ee952810c7dab53e8439547dd0e413c827b382a7f2b5b3cd447da3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `dart:stable` - linux; amd64

```console
$ docker pull dart@sha256:398c325b807d3d0481c7b0b3249d8d0db26263b6ad15b8bda93188255938d9cc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **289.1 MB (289063576 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a541608b7bdf2e8455d39e762bd0b61bcf72438a12a0f41d8a692e1e513481d6`
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
# Tue, 12 Oct 2021 09:49:13 GMT
RUN set -eux;     ARCH=$(case "$(dpkg --print-architecture)" in amd64) echo "x64";; esac;);     SDK="dartsdk-linux-$ARCH-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.14.3/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "cad36ec238af96c8048bbcec4cff7e69fcb1b895620010ca1762674ca4ade171 *$SDK"     | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK";
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
	-	`sha256:d2d33d8b9592194e7f0147e607d97c522691a0b68850ee994e112126dba7975e`  
		Last Modified: Tue, 12 Oct 2021 09:50:24 GMT  
		Size: 210.0 MB (209982370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:stable-sdk`

```console
$ docker pull dart@sha256:4f321ebb13ee952810c7dab53e8439547dd0e413c827b382a7f2b5b3cd447da3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `dart:stable-sdk` - linux; amd64

```console
$ docker pull dart@sha256:398c325b807d3d0481c7b0b3249d8d0db26263b6ad15b8bda93188255938d9cc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **289.1 MB (289063576 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a541608b7bdf2e8455d39e762bd0b61bcf72438a12a0f41d8a692e1e513481d6`
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
# Tue, 12 Oct 2021 09:49:13 GMT
RUN set -eux;     ARCH=$(case "$(dpkg --print-architecture)" in amd64) echo "x64";; esac;);     SDK="dartsdk-linux-$ARCH-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.14.3/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "cad36ec238af96c8048bbcec4cff7e69fcb1b895620010ca1762674ca4ade171 *$SDK"     | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK";
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
	-	`sha256:d2d33d8b9592194e7f0147e607d97c522691a0b68850ee994e112126dba7975e`  
		Last Modified: Tue, 12 Oct 2021 09:50:24 GMT  
		Size: 210.0 MB (209982370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
