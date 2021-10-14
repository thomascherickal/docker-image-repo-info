## `nats:2-scratch`

```console
$ docker pull nats@sha256:dbc00e4f9bdaab8be3605f27f407244a1e60a0e05079076010439f1fbe4d35d1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-scratch` - linux; amd64

```console
$ docker pull nats@sha256:92e7f9daede2d9f0bf0fb19ee9edbda0bb6f3d67d51fcaf7a0ea3a753f2a550c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4565653 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7e4065a82a64422de8554705cef94cee44d57d142a8faeac26a705c22a167cb`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 13 Oct 2021 16:13:46 GMT
COPY file:077f50be0de271ffda1008ecf0034a9197edf920d88c8b7acb4705e440055c58 in /nats-server 
# Wed, 13 Oct 2021 16:13:46 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Wed, 13 Oct 2021 16:13:46 GMT
EXPOSE 4222 6222 8222
# Wed, 13 Oct 2021 16:13:47 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 13 Oct 2021 16:13:47 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c78225a573bcf3c390263b8c87be5c2e84312bb59c28d935337b10784b2f26b6`  
		Last Modified: Wed, 13 Oct 2021 16:14:42 GMT  
		Size: 4.6 MB (4565176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccb63e48ce7d1ea5803409d74f576817497e48d850a274d4aa8f8bf3abb8060e`  
		Last Modified: Wed, 13 Oct 2021 16:14:41 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:93693c23ea5644f401a72bf6929214e9dfd2720b1b4c373025e689c1495de5a4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4228700 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a1d37c768b08a19ab2b56aff52bc2bd23a18c665a38568b80d03d43b91ebe1d`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 12 Oct 2021 23:50:02 GMT
COPY file:87c492688776372ccf80f66cfc3e90fd8fab44035811506c7aaa232e547e000b in /nats-server 
# Tue, 12 Oct 2021 23:50:03 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Tue, 12 Oct 2021 23:50:03 GMT
EXPOSE 4222 6222 8222
# Tue, 12 Oct 2021 23:50:04 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 12 Oct 2021 23:50:04 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3cd12bdf7a9a23f7457d02e8fc11f170382a386c0eeca79fe881fb322825f1a9`  
		Last Modified: Tue, 12 Oct 2021 23:52:26 GMT  
		Size: 4.2 MB (4228225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4d6a7556bfb5d88c2ff5e698fcd012e06a282a35550cc4944de84fe772a4481`  
		Last Modified: Tue, 12 Oct 2021 23:52:23 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:d2e70b8a1a863ae0f789502434cef995627ed0f46f551f291f2f7a0ff7017642
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4213288 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3787a15077edfb6d8fa1646ed439c24cc005849fcf8311a629d20c8679d8b139`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 30 Sep 2021 19:47:57 GMT
COPY file:6d69eef0d821da908da152f3dfe853b07d173db35f1c40a85e545d8218aaeb7e in /nats-server 
# Thu, 30 Sep 2021 19:47:57 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 30 Sep 2021 19:47:58 GMT
EXPOSE 4222 6222 8222
# Thu, 30 Sep 2021 19:47:58 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 30 Sep 2021 19:47:58 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c67bb3b32b6353245cbd27e1ee30c47b5cf8b7c76346ca37875fa7cc7086cf7e`  
		Last Modified: Thu, 30 Sep 2021 19:50:22 GMT  
		Size: 4.2 MB (4212814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:065d109fdaff0adc51732a8f449fee6ffda396a8e2a53cda9273482aa1fb36f0`  
		Last Modified: Thu, 30 Sep 2021 19:50:19 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:786b1d0fd6909fc41b7bd1bf8c44dd2820f8f9541b50fe208b51c505c578d76b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4176251 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:743df55fc15bcdcb14c7494057f1b36c76489d1ac4d8ee07b896d035a5ed0873`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 14 Oct 2021 01:43:21 GMT
COPY file:2d9fd0e07ac02bc374798c164451d7d2711d8ea053b033d74e5cfead339c6a9e in /nats-server 
# Thu, 14 Oct 2021 01:43:22 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 14 Oct 2021 01:43:22 GMT
EXPOSE 4222 6222 8222
# Thu, 14 Oct 2021 01:43:23 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 14 Oct 2021 01:43:24 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:e53ac6baa011c5ae6a6820d36c15d94ac5195d2cedd08c4820acedd234cf2a01`  
		Last Modified: Thu, 14 Oct 2021 01:44:36 GMT  
		Size: 4.2 MB (4175775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39601ce797abecc22d21af5567d4d3edd6263fdfc4fef144c8517ab00434a8e8`  
		Last Modified: Thu, 14 Oct 2021 01:44:36 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
