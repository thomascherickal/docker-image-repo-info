<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `clearlinux`

-	[`clearlinux:base`](#clearlinuxbase)
-	[`clearlinux:latest`](#clearlinuxlatest)

## `clearlinux:base`

```console
$ docker pull clearlinux@sha256:610c4ade0b7c4fd5986aebf4d95e215e6ec2190206e7b1152bd52e82d9f37c65
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `clearlinux:base` - linux; amd64

```console
$ docker pull clearlinux@sha256:f02ad60787c9ca5b9975ab52bcb14c6a02aea1dd627110fbe41139cabda06eea
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **98.2 MB (98244609 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31a048a8aae330933c5ce816c246d7b1ebbc3eb16fb8c4e21257948a9e708d99`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 09 Mar 2021 00:22:54 GMT
MAINTAINER William Douglas <william.douglas@intel.com>
# Mon, 12 Sep 2022 20:19:50 GMT
ADD file:90924874406d67b09806ed8ac61115f418b03a444e2369a4b2593b0344237dd8 in / 
# Mon, 12 Sep 2022 20:19:51 GMT
RUN cd /etc &&     grep root /usr/share/defaults/etc/passwd > /etc/passwd &&     grep root /usr/share/defaults/etc/group > /etc/group &&     grep root /usr/share/defaults/etc/shadow > /etc/shadow
# Mon, 12 Sep 2022 20:19:51 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:40cc60c056d6290e9dc5a737803bc22268ff1f474fed88722abe1ccd0208c973`  
		Last Modified: Mon, 12 Sep 2022 20:20:16 GMT  
		Size: 98.2 MB (98244391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07110403637bab6b47dbeb4086337841bbd1a703fff4a82437ad12f27b3c403e`  
		Last Modified: Mon, 12 Sep 2022 20:20:03 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `clearlinux:latest`

```console
$ docker pull clearlinux@sha256:610c4ade0b7c4fd5986aebf4d95e215e6ec2190206e7b1152bd52e82d9f37c65
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `clearlinux:latest` - linux; amd64

```console
$ docker pull clearlinux@sha256:f02ad60787c9ca5b9975ab52bcb14c6a02aea1dd627110fbe41139cabda06eea
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **98.2 MB (98244609 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31a048a8aae330933c5ce816c246d7b1ebbc3eb16fb8c4e21257948a9e708d99`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 09 Mar 2021 00:22:54 GMT
MAINTAINER William Douglas <william.douglas@intel.com>
# Mon, 12 Sep 2022 20:19:50 GMT
ADD file:90924874406d67b09806ed8ac61115f418b03a444e2369a4b2593b0344237dd8 in / 
# Mon, 12 Sep 2022 20:19:51 GMT
RUN cd /etc &&     grep root /usr/share/defaults/etc/passwd > /etc/passwd &&     grep root /usr/share/defaults/etc/group > /etc/group &&     grep root /usr/share/defaults/etc/shadow > /etc/shadow
# Mon, 12 Sep 2022 20:19:51 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:40cc60c056d6290e9dc5a737803bc22268ff1f474fed88722abe1ccd0208c973`  
		Last Modified: Mon, 12 Sep 2022 20:20:16 GMT  
		Size: 98.2 MB (98244391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07110403637bab6b47dbeb4086337841bbd1a703fff4a82437ad12f27b3c403e`  
		Last Modified: Mon, 12 Sep 2022 20:20:03 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
