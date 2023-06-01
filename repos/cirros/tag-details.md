<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `cirros`

-	[`cirros:0`](#cirros0)
-	[`cirros:0.5`](#cirros05)
-	[`cirros:0.5.3`](#cirros053)
-	[`cirros:0.6`](#cirros06)
-	[`cirros:0.6.0`](#cirros060)
-	[`cirros:0.6.1`](#cirros061)
-	[`cirros:0.6.2`](#cirros062)
-	[`cirros:latest`](#cirroslatest)

## `cirros:0`

```console
$ docker pull cirros@sha256:f0bc1c8d5421cd424bf8cee3340885dc9ad99fe089e8f1ed485c7a7a82c74307
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `cirros:0` - linux; amd64

```console
$ docker pull cirros@sha256:04469d1f7155e892eaa5cc0d774b4c8f499dd9f1d2df92c91505775b8b975abc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.4 MB (7415253 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cdb40efc43d69d1840118638fd91da72607c3125101fb428d4ac30e0a3bc5b1b`
-	Default Command: `["\/sbin\/init"]`

```dockerfile
# Tue, 22 Nov 2022 22:24:57 GMT
ADD file:12aef9d2ac43f48be6b03ab418cb5312e4e7f397d71d610afedfbcd1c2c73650 in / 
# Tue, 22 Nov 2022 22:24:57 GMT
RUN rm /etc/rc3.d/S40-network
# Tue, 22 Nov 2022 22:24:58 GMT
RUN sed -i '/is_lxc && lxc_netdown/d' /etc/init.d/rc.sysinit
# Tue, 22 Nov 2022 22:24:58 GMT
CMD ["/sbin/init"]
```

-	Layers:
	-	`sha256:d3ba20487232c21211201e5e9726d4bc5ac60d2db08ca089112733699c52a601`  
		Last Modified: Tue, 22 Nov 2022 22:25:09 GMT  
		Size: 7.4 MB (7413828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8c3cce1196c79818d788e9ce4c53d60d3129ed4e16923aa1184121b903c1a38`  
		Last Modified: Tue, 22 Nov 2022 22:25:08 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:899be78ec08abb367d05c9296da5f3d5701d8c5bd3653eafab2298ae9d53e067`  
		Last Modified: Tue, 22 Nov 2022 22:25:08 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `cirros:0` - linux; arm variant v7

```console
$ docker pull cirros@sha256:989d58cc2417ceb3997af1d5eec45942bfb96d179de42258ef26feee90d492a3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.9 MB (6917710 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:589a1ac713ab5d2e4ebe435a19733e169d3c3b0b41dc8ba9e5152e9077d69ff7`
-	Default Command: `["\/sbin\/init"]`

```dockerfile
# Thu, 01 Jun 2023 17:45:40 GMT
ADD file:5eedfffbb6342e38402ce33ec22c8e56d5fedf4bbe54378386e677f347a36e3c in / 
# Thu, 01 Jun 2023 17:45:41 GMT
RUN rm /etc/rc3.d/S40-network
# Thu, 01 Jun 2023 17:45:41 GMT
RUN sed -i '/is_lxc && lxc_netdown/d' /etc/init.d/rc.sysinit
# Thu, 01 Jun 2023 17:45:41 GMT
CMD ["/sbin/init"]
```

-	Layers:
	-	`sha256:f80362f561c125292ff108e8158fb93cff22d6c31e7254ff0934beb9d0aedd30`  
		Last Modified: Thu, 01 Jun 2023 17:46:05 GMT  
		Size: 6.9 MB (6916286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc766dd3aab55abadcc8e04db8c6eb70a4ac34059850310d5dcb7194f7d310fb`  
		Last Modified: Thu, 01 Jun 2023 17:46:04 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0abdd24eb7958ba4437dc204083be4fa5bab38f70969d9f1a696b42f0fb9995`  
		Last Modified: Thu, 01 Jun 2023 17:46:04 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `cirros:0` - linux; arm64 variant v8

```console
$ docker pull cirros@sha256:cdb1caacd17effe39a0f7de10ad063ffe48213936c6878ec47f9fd6ac0d4eeaa
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.5 MB (7512951 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c08510651948f20e927663a4e51033d4ed0272eacdb7f2eb22ca02f12de8008b`
-	Default Command: `["\/sbin\/init"]`

```dockerfile
# Thu, 01 Jun 2023 17:47:42 GMT
ADD file:b631ea2eba505c45d900fefe6abe60bf0fd55081d73b533b675497b4ac6fc7e9 in / 
# Thu, 01 Jun 2023 17:47:42 GMT
RUN rm /etc/rc3.d/S40-network
# Thu, 01 Jun 2023 17:47:43 GMT
RUN sed -i '/is_lxc && lxc_netdown/d' /etc/init.d/rc.sysinit
# Thu, 01 Jun 2023 17:47:43 GMT
CMD ["/sbin/init"]
```

-	Layers:
	-	`sha256:9f6485d64479ba46aaa6a5a1ceac7a29a0150c98eeed49ba17c0afe4eb2f7fff`  
		Last Modified: Thu, 01 Jun 2023 17:48:11 GMT  
		Size: 7.5 MB (7511527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be6fd5e2e591cbc25e4761475e2a118e730e79198465438b66eb3a1c993999c7`  
		Last Modified: Thu, 01 Jun 2023 17:48:10 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12503d8dede453a111c6f27f4d55ef0600dbc5b36706fe6d134d3c6f99620be6`  
		Last Modified: Thu, 01 Jun 2023 17:48:10 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `cirros:0` - linux; ppc64le

```console
$ docker pull cirros@sha256:752d80a265707f0757f06e543fe5bec4893f867be2cb0c65846ae0fc9e06a79d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.9 MB (7893829 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:75f332a1c396c946394238438e7a562e1bbe08e0fe70e267336bdbf3b45a0eed`
-	Default Command: `["\/sbin\/init"]`

```dockerfile
# Thu, 01 Jun 2023 17:47:02 GMT
ADD file:a96c96efad4fc7338db684c36b45a65c81d03475dbb97215d1928b899de72dbf in / 
# Thu, 01 Jun 2023 17:47:06 GMT
RUN rm /etc/rc3.d/S40-network
# Thu, 01 Jun 2023 17:47:08 GMT
RUN sed -i '/is_lxc && lxc_netdown/d' /etc/init.d/rc.sysinit
# Thu, 01 Jun 2023 17:47:09 GMT
CMD ["/sbin/init"]
```

-	Layers:
	-	`sha256:63052c0afd46b074efef54663e7dc1b63492c6d36d602f7bc5b14e9ffeac3f23`  
		Last Modified: Thu, 01 Jun 2023 17:48:10 GMT  
		Size: 7.9 MB (7892397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a0a340c0258d53ee3573a7b2bae98cf43ced4e6cba1b21e35a6cd7bb962ae55`  
		Last Modified: Thu, 01 Jun 2023 17:48:07 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b64dfb5dc29e3f4dbfcd1d631565b9931f7c168341874432f2bca100c31f4a4`  
		Last Modified: Thu, 01 Jun 2023 17:48:07 GMT  
		Size: 1.3 KB (1274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `cirros:0.5`

```console
$ docker pull cirros@sha256:75605258b2b2592ea514050d516accd8a7756e5f884c0b7f4871e3364eb602cd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `cirros:0.5` - linux; amd64

```console
$ docker pull cirros@sha256:483f15ac97d03dc3d4dcf79cf71ded2e099cf76c340f3fdd0b3670a40a198a22
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 MB (5953672 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9cae1daf5f682cb6403a766b3e6afd73a102296910f27ea1ec392b54dc0c188`
-	Default Command: `["\/sbin\/init"]`

```dockerfile
# Mon, 08 Mar 2021 21:36:43 GMT
ADD file:bf4d7c23fe6b77a5c46f4c3ece606130b86aa04af3fbb2a320fb4a4d412c4603 in / 
# Mon, 08 Mar 2021 21:36:44 GMT
RUN rm /etc/rc3.d/S40-network
# Mon, 08 Mar 2021 21:36:45 GMT
RUN sed -i '/is_lxc && lxc_netdown/d' /etc/init.d/rc.sysinit
# Mon, 08 Mar 2021 21:36:45 GMT
CMD ["/sbin/init"]
```

-	Layers:
	-	`sha256:d0b405be7a3253cffc2d4b8425dd78c06d4196846dfe4d8fe45935f8d30fa351`  
		Last Modified: Mon, 08 Mar 2021 21:36:59 GMT  
		Size: 6.0 MB (5952271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd054094a03766a7be2860c487e0752bd99b1a636e189a2f9f2a29af58f2814e`  
		Last Modified: Mon, 08 Mar 2021 21:36:59 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6a00de1ec8ac5311a5d4166e3433bb59659057b5be4de6465234975bec50742`  
		Last Modified: Mon, 08 Mar 2021 21:36:56 GMT  
		Size: 1.2 KB (1247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `cirros:0.5` - linux; arm variant v5

```console
$ docker pull cirros@sha256:a3f86bf18b65a590fab7d5617b18f1dade32d775927976b1283bf86af55cc3d2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.6 MB (5641934 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0bb20bb109168d8888a73db3087ff30f6eab6e354d58912f8a40330d00f25572`
-	Default Command: `["\/sbin\/init"]`

```dockerfile
# Thu, 01 Jun 2023 17:45:31 GMT
ADD file:bf385ba21e024b8fa774ca2b95f19dec63586786a2c97a5163e00188e43d9543 in / 
# Thu, 01 Jun 2023 17:45:32 GMT
RUN rm /etc/rc3.d/S40-network
# Thu, 01 Jun 2023 17:45:32 GMT
RUN sed -i '/is_lxc && lxc_netdown/d' /etc/init.d/rc.sysinit
# Thu, 01 Jun 2023 17:45:32 GMT
CMD ["/sbin/init"]
```

-	Layers:
	-	`sha256:819bef02c3fe5830c3e4bc706e4d0c0c105cde329dc595488acf1a57edbb5ed6`  
		Last Modified: Thu, 01 Jun 2023 17:45:40 GMT  
		Size: 5.6 MB (5640532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5c050fc343b75f9770587dcc662e56b0cf514db635d3b0eceb29a100f048362`  
		Last Modified: Thu, 01 Jun 2023 17:45:39 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e998d2f7f7669247b2794c89738f6bfb649af9534ee69c2533de88fcf336005`  
		Last Modified: Thu, 01 Jun 2023 17:45:40 GMT  
		Size: 1.2 KB (1248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `cirros:0.5` - linux; arm64 variant v8

```console
$ docker pull cirros@sha256:93c54f8af2c550bd6a487bfd942767501ccf10706535a2d11e7b0b460d560900
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.4 MB (5392028 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:734b3665d29281d49078baa3c60b9e5272aa24001d48a2536e0bcf45efa392d4`
-	Default Command: `["\/sbin\/init"]`

```dockerfile
# Thu, 01 Jun 2023 17:47:59 GMT
ADD file:26037a1f961c5fc52d85131f9ccf3f142d2d4c20671bd5cf8f3878c1892ab344 in / 
# Thu, 01 Jun 2023 17:47:59 GMT
RUN rm /etc/rc3.d/S40-network
# Thu, 01 Jun 2023 17:48:00 GMT
RUN sed -i '/is_lxc && lxc_netdown/d' /etc/init.d/rc.sysinit
# Thu, 01 Jun 2023 17:48:00 GMT
CMD ["/sbin/init"]
```

-	Layers:
	-	`sha256:f7f09ef34c82c562e400e47d217f3e4bb947c8368f2a80f6a6bb0a7511e8fc6f`  
		Last Modified: Thu, 01 Jun 2023 17:48:31 GMT  
		Size: 5.4 MB (5390622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04e365931f6c8283628f13f3c0b389893445131dd87bf03240426110eb41ed5f`  
		Last Modified: Thu, 01 Jun 2023 17:48:30 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b189719c6c804ac56805ce4405886dc97489c4d2e1f440b3571946c72c7b4701`  
		Last Modified: Thu, 01 Jun 2023 17:48:30 GMT  
		Size: 1.3 KB (1252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `cirros:0.5` - linux; 386

```console
$ docker pull cirros@sha256:4b1bb6b67517af641a8cbceda13d0c90c4ace544d60321e02e6d44cbf85ee887
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.5 MB (5535384 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5faefcd187329dcd768cb9dc410ac5ccee72519854dcf87575ffb534f496944c`
-	Default Command: `["\/sbin\/init"]`

```dockerfile
# Thu, 01 Jun 2023 17:45:52 GMT
ADD file:7bd750ce8f56337eaed882eb743acae802072db86d0b398f1da5e272a8129e1c in / 
# Thu, 01 Jun 2023 17:45:53 GMT
RUN rm /etc/rc3.d/S40-network
# Thu, 01 Jun 2023 17:45:53 GMT
RUN sed -i '/is_lxc && lxc_netdown/d' /etc/init.d/rc.sysinit
# Thu, 01 Jun 2023 17:45:53 GMT
CMD ["/sbin/init"]
```

-	Layers:
	-	`sha256:32402c253eb2ceae60dd1bee991be9679a785eee02f1760dec07aa0d752324ca`  
		Last Modified: Thu, 01 Jun 2023 17:46:02 GMT  
		Size: 5.5 MB (5533980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ea9a0bcc5b6ec5dceeb5bce92bb889e749d349ccd1e986145f13b2453b895fc`  
		Last Modified: Thu, 01 Jun 2023 17:46:01 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58a9fba927dbf72c1339bc1a34de47d6f65707d6af5faee7685bb5689ac487d7`  
		Last Modified: Thu, 01 Jun 2023 17:46:01 GMT  
		Size: 1.2 KB (1247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `cirros:0.5` - linux; ppc64le

```console
$ docker pull cirros@sha256:a58a2e732775fbadb0095abeb37b76630e1939b43a23d60a1a84ca774c9a9d9c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 MB (5771764 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1aff4e7d85a54d72bc9f21c926441b4c07353a087a01242129b82b6d09c97cb6`
-	Default Command: `["\/sbin\/init"]`

```dockerfile
# Thu, 01 Jun 2023 17:47:47 GMT
ADD file:1b1f13ccf93e0821eebb8d4cb823f694074c26ebad6a6b783e10486c3665f146 in / 
# Thu, 01 Jun 2023 17:47:49 GMT
RUN rm /etc/rc3.d/S40-network
# Thu, 01 Jun 2023 17:47:50 GMT
RUN sed -i '/is_lxc && lxc_netdown/d' /etc/init.d/rc.sysinit
# Thu, 01 Jun 2023 17:47:51 GMT
CMD ["/sbin/init"]
```

-	Layers:
	-	`sha256:f85f7bbf72d281f812455db98a71c3d0a8f7bd1cd7c943227304d5e30eef38db`  
		Last Modified: Thu, 01 Jun 2023 17:48:32 GMT  
		Size: 5.8 MB (5770356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15fbe7207990c509701036cbd821b7353c2ae698ad7ceef928878dfc11ab59ab`  
		Last Modified: Thu, 01 Jun 2023 17:48:31 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d9979dd462606b77d4574a38169bbc4bbadbe75d73310ec00db716d4ed72d2e`  
		Last Modified: Thu, 01 Jun 2023 17:48:31 GMT  
		Size: 1.3 KB (1251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `cirros:0.5.3`

```console
$ docker pull cirros@sha256:20856349982924e2691ed98e66bbb2ff45e95f5f6f33a254cd1baf52c7620dcb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; arm variant v5
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `cirros:0.5.3` - linux; arm variant v5

```console
$ docker pull cirros@sha256:a3f86bf18b65a590fab7d5617b18f1dade32d775927976b1283bf86af55cc3d2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.6 MB (5641934 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0bb20bb109168d8888a73db3087ff30f6eab6e354d58912f8a40330d00f25572`
-	Default Command: `["\/sbin\/init"]`

```dockerfile
# Thu, 01 Jun 2023 17:45:31 GMT
ADD file:bf385ba21e024b8fa774ca2b95f19dec63586786a2c97a5163e00188e43d9543 in / 
# Thu, 01 Jun 2023 17:45:32 GMT
RUN rm /etc/rc3.d/S40-network
# Thu, 01 Jun 2023 17:45:32 GMT
RUN sed -i '/is_lxc && lxc_netdown/d' /etc/init.d/rc.sysinit
# Thu, 01 Jun 2023 17:45:32 GMT
CMD ["/sbin/init"]
```

-	Layers:
	-	`sha256:819bef02c3fe5830c3e4bc706e4d0c0c105cde329dc595488acf1a57edbb5ed6`  
		Last Modified: Thu, 01 Jun 2023 17:45:40 GMT  
		Size: 5.6 MB (5640532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5c050fc343b75f9770587dcc662e56b0cf514db635d3b0eceb29a100f048362`  
		Last Modified: Thu, 01 Jun 2023 17:45:39 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e998d2f7f7669247b2794c89738f6bfb649af9534ee69c2533de88fcf336005`  
		Last Modified: Thu, 01 Jun 2023 17:45:40 GMT  
		Size: 1.2 KB (1248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `cirros:0.5.3` - linux; arm64 variant v8

```console
$ docker pull cirros@sha256:93c54f8af2c550bd6a487bfd942767501ccf10706535a2d11e7b0b460d560900
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.4 MB (5392028 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:734b3665d29281d49078baa3c60b9e5272aa24001d48a2536e0bcf45efa392d4`
-	Default Command: `["\/sbin\/init"]`

```dockerfile
# Thu, 01 Jun 2023 17:47:59 GMT
ADD file:26037a1f961c5fc52d85131f9ccf3f142d2d4c20671bd5cf8f3878c1892ab344 in / 
# Thu, 01 Jun 2023 17:47:59 GMT
RUN rm /etc/rc3.d/S40-network
# Thu, 01 Jun 2023 17:48:00 GMT
RUN sed -i '/is_lxc && lxc_netdown/d' /etc/init.d/rc.sysinit
# Thu, 01 Jun 2023 17:48:00 GMT
CMD ["/sbin/init"]
```

-	Layers:
	-	`sha256:f7f09ef34c82c562e400e47d217f3e4bb947c8368f2a80f6a6bb0a7511e8fc6f`  
		Last Modified: Thu, 01 Jun 2023 17:48:31 GMT  
		Size: 5.4 MB (5390622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04e365931f6c8283628f13f3c0b389893445131dd87bf03240426110eb41ed5f`  
		Last Modified: Thu, 01 Jun 2023 17:48:30 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b189719c6c804ac56805ce4405886dc97489c4d2e1f440b3571946c72c7b4701`  
		Last Modified: Thu, 01 Jun 2023 17:48:30 GMT  
		Size: 1.3 KB (1252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `cirros:0.5.3` - linux; 386

```console
$ docker pull cirros@sha256:4b1bb6b67517af641a8cbceda13d0c90c4ace544d60321e02e6d44cbf85ee887
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.5 MB (5535384 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5faefcd187329dcd768cb9dc410ac5ccee72519854dcf87575ffb534f496944c`
-	Default Command: `["\/sbin\/init"]`

```dockerfile
# Thu, 01 Jun 2023 17:45:52 GMT
ADD file:7bd750ce8f56337eaed882eb743acae802072db86d0b398f1da5e272a8129e1c in / 
# Thu, 01 Jun 2023 17:45:53 GMT
RUN rm /etc/rc3.d/S40-network
# Thu, 01 Jun 2023 17:45:53 GMT
RUN sed -i '/is_lxc && lxc_netdown/d' /etc/init.d/rc.sysinit
# Thu, 01 Jun 2023 17:45:53 GMT
CMD ["/sbin/init"]
```

-	Layers:
	-	`sha256:32402c253eb2ceae60dd1bee991be9679a785eee02f1760dec07aa0d752324ca`  
		Last Modified: Thu, 01 Jun 2023 17:46:02 GMT  
		Size: 5.5 MB (5533980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ea9a0bcc5b6ec5dceeb5bce92bb889e749d349ccd1e986145f13b2453b895fc`  
		Last Modified: Thu, 01 Jun 2023 17:46:01 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58a9fba927dbf72c1339bc1a34de47d6f65707d6af5faee7685bb5689ac487d7`  
		Last Modified: Thu, 01 Jun 2023 17:46:01 GMT  
		Size: 1.2 KB (1247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `cirros:0.5.3` - linux; ppc64le

```console
$ docker pull cirros@sha256:a58a2e732775fbadb0095abeb37b76630e1939b43a23d60a1a84ca774c9a9d9c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 MB (5771764 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1aff4e7d85a54d72bc9f21c926441b4c07353a087a01242129b82b6d09c97cb6`
-	Default Command: `["\/sbin\/init"]`

```dockerfile
# Thu, 01 Jun 2023 17:47:47 GMT
ADD file:1b1f13ccf93e0821eebb8d4cb823f694074c26ebad6a6b783e10486c3665f146 in / 
# Thu, 01 Jun 2023 17:47:49 GMT
RUN rm /etc/rc3.d/S40-network
# Thu, 01 Jun 2023 17:47:50 GMT
RUN sed -i '/is_lxc && lxc_netdown/d' /etc/init.d/rc.sysinit
# Thu, 01 Jun 2023 17:47:51 GMT
CMD ["/sbin/init"]
```

-	Layers:
	-	`sha256:f85f7bbf72d281f812455db98a71c3d0a8f7bd1cd7c943227304d5e30eef38db`  
		Last Modified: Thu, 01 Jun 2023 17:48:32 GMT  
		Size: 5.8 MB (5770356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15fbe7207990c509701036cbd821b7353c2ae698ad7ceef928878dfc11ab59ab`  
		Last Modified: Thu, 01 Jun 2023 17:48:31 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d9979dd462606b77d4574a38169bbc4bbadbe75d73310ec00db716d4ed72d2e`  
		Last Modified: Thu, 01 Jun 2023 17:48:31 GMT  
		Size: 1.3 KB (1251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `cirros:0.6`

```console
$ docker pull cirros@sha256:f0bc1c8d5421cd424bf8cee3340885dc9ad99fe089e8f1ed485c7a7a82c74307
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `cirros:0.6` - linux; amd64

```console
$ docker pull cirros@sha256:04469d1f7155e892eaa5cc0d774b4c8f499dd9f1d2df92c91505775b8b975abc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.4 MB (7415253 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cdb40efc43d69d1840118638fd91da72607c3125101fb428d4ac30e0a3bc5b1b`
-	Default Command: `["\/sbin\/init"]`

```dockerfile
# Tue, 22 Nov 2022 22:24:57 GMT
ADD file:12aef9d2ac43f48be6b03ab418cb5312e4e7f397d71d610afedfbcd1c2c73650 in / 
# Tue, 22 Nov 2022 22:24:57 GMT
RUN rm /etc/rc3.d/S40-network
# Tue, 22 Nov 2022 22:24:58 GMT
RUN sed -i '/is_lxc && lxc_netdown/d' /etc/init.d/rc.sysinit
# Tue, 22 Nov 2022 22:24:58 GMT
CMD ["/sbin/init"]
```

-	Layers:
	-	`sha256:d3ba20487232c21211201e5e9726d4bc5ac60d2db08ca089112733699c52a601`  
		Last Modified: Tue, 22 Nov 2022 22:25:09 GMT  
		Size: 7.4 MB (7413828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8c3cce1196c79818d788e9ce4c53d60d3129ed4e16923aa1184121b903c1a38`  
		Last Modified: Tue, 22 Nov 2022 22:25:08 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:899be78ec08abb367d05c9296da5f3d5701d8c5bd3653eafab2298ae9d53e067`  
		Last Modified: Tue, 22 Nov 2022 22:25:08 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `cirros:0.6` - linux; arm variant v7

```console
$ docker pull cirros@sha256:989d58cc2417ceb3997af1d5eec45942bfb96d179de42258ef26feee90d492a3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.9 MB (6917710 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:589a1ac713ab5d2e4ebe435a19733e169d3c3b0b41dc8ba9e5152e9077d69ff7`
-	Default Command: `["\/sbin\/init"]`

```dockerfile
# Thu, 01 Jun 2023 17:45:40 GMT
ADD file:5eedfffbb6342e38402ce33ec22c8e56d5fedf4bbe54378386e677f347a36e3c in / 
# Thu, 01 Jun 2023 17:45:41 GMT
RUN rm /etc/rc3.d/S40-network
# Thu, 01 Jun 2023 17:45:41 GMT
RUN sed -i '/is_lxc && lxc_netdown/d' /etc/init.d/rc.sysinit
# Thu, 01 Jun 2023 17:45:41 GMT
CMD ["/sbin/init"]
```

-	Layers:
	-	`sha256:f80362f561c125292ff108e8158fb93cff22d6c31e7254ff0934beb9d0aedd30`  
		Last Modified: Thu, 01 Jun 2023 17:46:05 GMT  
		Size: 6.9 MB (6916286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc766dd3aab55abadcc8e04db8c6eb70a4ac34059850310d5dcb7194f7d310fb`  
		Last Modified: Thu, 01 Jun 2023 17:46:04 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0abdd24eb7958ba4437dc204083be4fa5bab38f70969d9f1a696b42f0fb9995`  
		Last Modified: Thu, 01 Jun 2023 17:46:04 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `cirros:0.6` - linux; arm64 variant v8

```console
$ docker pull cirros@sha256:cdb1caacd17effe39a0f7de10ad063ffe48213936c6878ec47f9fd6ac0d4eeaa
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.5 MB (7512951 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c08510651948f20e927663a4e51033d4ed0272eacdb7f2eb22ca02f12de8008b`
-	Default Command: `["\/sbin\/init"]`

```dockerfile
# Thu, 01 Jun 2023 17:47:42 GMT
ADD file:b631ea2eba505c45d900fefe6abe60bf0fd55081d73b533b675497b4ac6fc7e9 in / 
# Thu, 01 Jun 2023 17:47:42 GMT
RUN rm /etc/rc3.d/S40-network
# Thu, 01 Jun 2023 17:47:43 GMT
RUN sed -i '/is_lxc && lxc_netdown/d' /etc/init.d/rc.sysinit
# Thu, 01 Jun 2023 17:47:43 GMT
CMD ["/sbin/init"]
```

-	Layers:
	-	`sha256:9f6485d64479ba46aaa6a5a1ceac7a29a0150c98eeed49ba17c0afe4eb2f7fff`  
		Last Modified: Thu, 01 Jun 2023 17:48:11 GMT  
		Size: 7.5 MB (7511527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be6fd5e2e591cbc25e4761475e2a118e730e79198465438b66eb3a1c993999c7`  
		Last Modified: Thu, 01 Jun 2023 17:48:10 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12503d8dede453a111c6f27f4d55ef0600dbc5b36706fe6d134d3c6f99620be6`  
		Last Modified: Thu, 01 Jun 2023 17:48:10 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `cirros:0.6` - linux; ppc64le

```console
$ docker pull cirros@sha256:752d80a265707f0757f06e543fe5bec4893f867be2cb0c65846ae0fc9e06a79d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.9 MB (7893829 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:75f332a1c396c946394238438e7a562e1bbe08e0fe70e267336bdbf3b45a0eed`
-	Default Command: `["\/sbin\/init"]`

```dockerfile
# Thu, 01 Jun 2023 17:47:02 GMT
ADD file:a96c96efad4fc7338db684c36b45a65c81d03475dbb97215d1928b899de72dbf in / 
# Thu, 01 Jun 2023 17:47:06 GMT
RUN rm /etc/rc3.d/S40-network
# Thu, 01 Jun 2023 17:47:08 GMT
RUN sed -i '/is_lxc && lxc_netdown/d' /etc/init.d/rc.sysinit
# Thu, 01 Jun 2023 17:47:09 GMT
CMD ["/sbin/init"]
```

-	Layers:
	-	`sha256:63052c0afd46b074efef54663e7dc1b63492c6d36d602f7bc5b14e9ffeac3f23`  
		Last Modified: Thu, 01 Jun 2023 17:48:10 GMT  
		Size: 7.9 MB (7892397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a0a340c0258d53ee3573a7b2bae98cf43ced4e6cba1b21e35a6cd7bb962ae55`  
		Last Modified: Thu, 01 Jun 2023 17:48:07 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b64dfb5dc29e3f4dbfcd1d631565b9931f7c168341874432f2bca100c31f4a4`  
		Last Modified: Thu, 01 Jun 2023 17:48:07 GMT  
		Size: 1.3 KB (1274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `cirros:0.6.0`

```console
$ docker pull cirros@sha256:1c44d65d6bca98c4319345eac5d93e32fa1e2578951bf0dfcd501d96bd0c1f29
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `cirros:0.6.0` - linux; amd64

```console
$ docker pull cirros@sha256:b091f9f8a8afb0c7dbaf739527a28f0cc36e6a272a67f2a355228bc0251e8f03
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.4 MB (7396061 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fb8645b3e96cb8fa8f6b0ea7f3a513aecda704242e8c061ba79ba86bfad07b22`
-	Default Command: `["\/sbin\/init"]`

```dockerfile
# Wed, 28 Sep 2022 22:19:35 GMT
ADD file:b8d91b562c53a12cb13826cb11a65c4ac06a77fa38cc3ecd9c42560e9a982c82 in / 
# Wed, 28 Sep 2022 22:19:36 GMT
RUN rm /etc/rc3.d/S40-network
# Wed, 28 Sep 2022 22:19:37 GMT
RUN sed -i '/is_lxc && lxc_netdown/d' /etc/init.d/rc.sysinit
# Wed, 28 Sep 2022 22:19:37 GMT
CMD ["/sbin/init"]
```

-	Layers:
	-	`sha256:be7f771b7ce61d7b35d254415470a28cdc9a5513c4e188cf623ff36bcb95208e`  
		Last Modified: Wed, 28 Sep 2022 22:19:49 GMT  
		Size: 7.4 MB (7394660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:978a5518d53f7def25bf6e2fef250b43f81d88caaa03f48de7ac9ea8e5b52ab0`  
		Last Modified: Wed, 28 Sep 2022 22:19:47 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cdd27c98889cb990c870d7a614e9cd7abdc71ecfce9378726411ff5bbb21fb0`  
		Last Modified: Wed, 28 Sep 2022 22:19:47 GMT  
		Size: 1.2 KB (1244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `cirros:0.6.0` - linux; arm variant v7

```console
$ docker pull cirros@sha256:e92c472db412a3ca5a88f0dadd9d75fbf762c580d06e1f6fdab9b76f7f37e867
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.9 MB (6896134 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ae62985911ae71c702034321b794a6c1763a1ee6741b45a71ce6a7f9fd49e61d`
-	Default Command: `["\/sbin\/init"]`

```dockerfile
# Thu, 01 Jun 2023 17:45:53 GMT
ADD file:da9fcd1025acb12e39f02d61c9db96e5643e1b171bd7c70fc5904caca4444cbd in / 
# Thu, 01 Jun 2023 17:45:53 GMT
RUN rm /etc/rc3.d/S40-network
# Thu, 01 Jun 2023 17:45:54 GMT
RUN sed -i '/is_lxc && lxc_netdown/d' /etc/init.d/rc.sysinit
# Thu, 01 Jun 2023 17:45:54 GMT
CMD ["/sbin/init"]
```

-	Layers:
	-	`sha256:9ea391a19b65fb9cb506d6cba741637fa497f8dbe3b7aa5b8da499f89986036f`  
		Last Modified: Wed, 28 Sep 2022 21:48:38 GMT  
		Size: 6.9 MB (6894731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67ebe99f353688f4664cc84341d076902da7dcc1cc7f5bb18c5204aa34e9b079`  
		Last Modified: Thu, 01 Jun 2023 17:46:24 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29a72d561bbe268cb7c8f3336ddf02b54179b8546074ceacd5b0994c3cfbc61c`  
		Last Modified: Thu, 01 Jun 2023 17:46:24 GMT  
		Size: 1.2 KB (1249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `cirros:0.6.0` - linux; arm64 variant v8

```console
$ docker pull cirros@sha256:6ec7275b3813aa674028eedb791fa9e45089d48d1ff661c877ed60bec23ff5e3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.5 MB (7493751 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d294fe7eb01a9f64db135d7b7e933ce890d5e92894856adba05cc00380a73868`
-	Default Command: `["\/sbin\/init"]`

```dockerfile
# Thu, 01 Jun 2023 17:47:52 GMT
ADD file:e4ad7e8f8ff0a06a00a1187410abf6f9a7b103307857239e8b23bdf786d18ed1 in / 
# Thu, 01 Jun 2023 17:47:53 GMT
RUN rm /etc/rc3.d/S40-network
# Thu, 01 Jun 2023 17:47:53 GMT
RUN sed -i '/is_lxc && lxc_netdown/d' /etc/init.d/rc.sysinit
# Thu, 01 Jun 2023 17:47:54 GMT
CMD ["/sbin/init"]
```

-	Layers:
	-	`sha256:46314231ec9fd8a50fac23daae253555d0556a7533d908a3b93a4602e68ec7bf`  
		Last Modified: Wed, 28 Sep 2022 21:41:17 GMT  
		Size: 7.5 MB (7492347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96964917a635fc6496c93e82d4962f0eb139ea2dc94329e1c5ecd0cf70d84a30`  
		Last Modified: Thu, 01 Jun 2023 17:48:23 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d06bd3f35d9e0b0e2f526cdd4b7372f6d384e2b1ba8d6c9bf4dae7d9e1b3b17c`  
		Last Modified: Thu, 01 Jun 2023 17:48:23 GMT  
		Size: 1.2 KB (1247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `cirros:0.6.0` - linux; ppc64le

```console
$ docker pull cirros@sha256:d59778a09b21318157fbc812e9e1e4d3c283a02e3b4debe89144d52c5308e139
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.9 MB (7860615 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a7dc15c16adbc6935cb70ece2fa1c08a1784e22721188abdbd3fcc7afeab56be`
-	Default Command: `["\/sbin\/init"]`

```dockerfile
# Thu, 01 Jun 2023 17:47:33 GMT
ADD file:a7ec69c97fafba6a384e64a1ed985fcb6739b8fbea97fd39760fe3e306834d1d in / 
# Thu, 01 Jun 2023 17:47:34 GMT
RUN rm /etc/rc3.d/S40-network
# Thu, 01 Jun 2023 17:47:37 GMT
RUN sed -i '/is_lxc && lxc_netdown/d' /etc/init.d/rc.sysinit
# Thu, 01 Jun 2023 17:47:37 GMT
CMD ["/sbin/init"]
```

-	Layers:
	-	`sha256:61b998b3cc8178647a684107dbfe618f042e8646d0bfb92b3903a8510bf8099a`  
		Last Modified: Wed, 28 Sep 2022 22:16:59 GMT  
		Size: 7.9 MB (7859207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:920d1fb428335f781eceb0597a14d145831844606f3ce6ccbe77a87fa279c56e`  
		Last Modified: Thu, 01 Jun 2023 17:48:24 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:844580c51f9921965e81fc44137d42c3584925a779ad992114159f35f2969f9c`  
		Last Modified: Thu, 01 Jun 2023 17:48:24 GMT  
		Size: 1.3 KB (1252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `cirros:0.6.1`

```console
$ docker pull cirros@sha256:3a97e369d366961993b0227311cffd3930b07a18bdda5ad7bfd2d36b15e7d7d2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `cirros:0.6.1` - linux; amd64

```console
$ docker pull cirros@sha256:04469d1f7155e892eaa5cc0d774b4c8f499dd9f1d2df92c91505775b8b975abc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.4 MB (7415253 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cdb40efc43d69d1840118638fd91da72607c3125101fb428d4ac30e0a3bc5b1b`
-	Default Command: `["\/sbin\/init"]`

```dockerfile
# Tue, 22 Nov 2022 22:24:57 GMT
ADD file:12aef9d2ac43f48be6b03ab418cb5312e4e7f397d71d610afedfbcd1c2c73650 in / 
# Tue, 22 Nov 2022 22:24:57 GMT
RUN rm /etc/rc3.d/S40-network
# Tue, 22 Nov 2022 22:24:58 GMT
RUN sed -i '/is_lxc && lxc_netdown/d' /etc/init.d/rc.sysinit
# Tue, 22 Nov 2022 22:24:58 GMT
CMD ["/sbin/init"]
```

-	Layers:
	-	`sha256:d3ba20487232c21211201e5e9726d4bc5ac60d2db08ca089112733699c52a601`  
		Last Modified: Tue, 22 Nov 2022 22:25:09 GMT  
		Size: 7.4 MB (7413828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8c3cce1196c79818d788e9ce4c53d60d3129ed4e16923aa1184121b903c1a38`  
		Last Modified: Tue, 22 Nov 2022 22:25:08 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:899be78ec08abb367d05c9296da5f3d5701d8c5bd3653eafab2298ae9d53e067`  
		Last Modified: Tue, 22 Nov 2022 22:25:08 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `cirros:0.6.1` - linux; arm variant v7

```console
$ docker pull cirros@sha256:67f6fc514f386c81156778787809fc82e9924a80264824ddbd3616773eb99d21
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.9 MB (6917657 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c9a231fe5f5e84fcd4a3f188dd59bda62a474c2e0bb1a47d1031c4158c60cfb`
-	Default Command: `["\/sbin\/init"]`

```dockerfile
# Thu, 01 Jun 2023 17:45:47 GMT
ADD file:a7007b63f19798cbc22966ecedc9e89242374a10b1afb98d0a6d3a2c65f1f144 in / 
# Thu, 01 Jun 2023 17:45:48 GMT
RUN rm /etc/rc3.d/S40-network
# Thu, 01 Jun 2023 17:45:48 GMT
RUN sed -i '/is_lxc && lxc_netdown/d' /etc/init.d/rc.sysinit
# Thu, 01 Jun 2023 17:45:49 GMT
CMD ["/sbin/init"]
```

-	Layers:
	-	`sha256:1b9fe69ed5aa8f1fc5e892a6797855a8e2b287bdeca83678c4baa5ef680ff902`  
		Last Modified: Tue, 22 Nov 2022 22:48:46 GMT  
		Size: 6.9 MB (6916230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e7c4f94f6e84312f35d4c837221a0a6f09ca51fd015f33992f1437a4ac5f573`  
		Last Modified: Thu, 01 Jun 2023 17:46:17 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35dbfe37b771d7c90cd52757da0331cbf4c9832ed536f95a7e89092c66b53fb9`  
		Last Modified: Thu, 01 Jun 2023 17:46:18 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `cirros:0.6.1` - linux; arm64 variant v8

```console
$ docker pull cirros@sha256:30db2666166be7fa735adfe4acacc993155fe42d7cb10c71466d041087a1656d
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.5 MB (7512652 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6de97c6c15f18adf0026a11296814e3d3e8831def6c83ed8d3bdcfcb9b7e74b1`
-	Default Command: `["\/sbin\/init"]`

```dockerfile
# Tue, 22 Nov 2022 22:44:49 GMT
ADD file:c514c5032cd91c1fb91255042fe76fa4ceff872c26b8e0736dc53a404a00ac39 in / 
# Tue, 22 Nov 2022 22:44:50 GMT
RUN rm /etc/rc3.d/S40-network
# Tue, 22 Nov 2022 22:44:50 GMT
RUN sed -i '/is_lxc && lxc_netdown/d' /etc/init.d/rc.sysinit
# Tue, 22 Nov 2022 22:44:50 GMT
CMD ["/sbin/init"]
```

-	Layers:
	-	`sha256:c8707b44c02a6ce4855dfbf586d6ced951085be6fa4d08f07a7ee2edf4da3ace`  
		Last Modified: Tue, 22 Nov 2022 22:45:00 GMT  
		Size: 7.5 MB (7511226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea1d71011505eddfbcdaee10a64041d078488e86d245ff3682e284d7df5aa6c9`  
		Last Modified: Tue, 22 Nov 2022 22:44:59 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a55391f8c263fc986ed0bb96c40ee7365b364e515a22c4411706348d64aa929d`  
		Last Modified: Tue, 22 Nov 2022 22:44:59 GMT  
		Size: 1.3 KB (1272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `cirros:0.6.1` - linux; ppc64le

```console
$ docker pull cirros@sha256:bf0de90a3e2b1ea0fdf252cf76a6310556f89e00fa22f15d361ad0695a70ab35
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.9 MB (7893520 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1a29a37940a400355fccefeb6424b3157ae269ea3cfb780b3c66889f29aa5027`
-	Default Command: `["\/sbin\/init"]`

```dockerfile
# Tue, 22 Nov 2022 22:24:26 GMT
ADD file:e7ac3506307e02ffe6fe2dc4aae3c3c2b4670caf39f27d546b7aafa56804d15d in / 
# Tue, 22 Nov 2022 22:24:28 GMT
RUN rm /etc/rc3.d/S40-network
# Tue, 22 Nov 2022 22:24:30 GMT
RUN sed -i '/is_lxc && lxc_netdown/d' /etc/init.d/rc.sysinit
# Tue, 22 Nov 2022 22:24:30 GMT
CMD ["/sbin/init"]
```

-	Layers:
	-	`sha256:8ff514ef264d54b0769c5c9d8694bf3b3205f7ebc8dab4684c4c01b065317360`  
		Last Modified: Tue, 22 Nov 2022 22:24:50 GMT  
		Size: 7.9 MB (7892088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:211d8e8a50a26a9eb56f1a25726b335406277d20936cfb4f70d395d526ee4a4e`  
		Last Modified: Tue, 22 Nov 2022 22:24:48 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b20cf7ce7547c1821bda40130026988eeb9e996599b347a0f91335c72194ff52`  
		Last Modified: Tue, 22 Nov 2022 22:24:48 GMT  
		Size: 1.3 KB (1275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `cirros:0.6.2`

```console
$ docker pull cirros@sha256:4ddc00d15810606575fa12be5ef8ff52177c31c47eb6bdaab3956c34a9dc5ccb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `cirros:0.6.2` - linux; arm variant v7

```console
$ docker pull cirros@sha256:989d58cc2417ceb3997af1d5eec45942bfb96d179de42258ef26feee90d492a3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.9 MB (6917710 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:589a1ac713ab5d2e4ebe435a19733e169d3c3b0b41dc8ba9e5152e9077d69ff7`
-	Default Command: `["\/sbin\/init"]`

```dockerfile
# Thu, 01 Jun 2023 17:45:40 GMT
ADD file:5eedfffbb6342e38402ce33ec22c8e56d5fedf4bbe54378386e677f347a36e3c in / 
# Thu, 01 Jun 2023 17:45:41 GMT
RUN rm /etc/rc3.d/S40-network
# Thu, 01 Jun 2023 17:45:41 GMT
RUN sed -i '/is_lxc && lxc_netdown/d' /etc/init.d/rc.sysinit
# Thu, 01 Jun 2023 17:45:41 GMT
CMD ["/sbin/init"]
```

-	Layers:
	-	`sha256:f80362f561c125292ff108e8158fb93cff22d6c31e7254ff0934beb9d0aedd30`  
		Last Modified: Thu, 01 Jun 2023 17:46:05 GMT  
		Size: 6.9 MB (6916286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc766dd3aab55abadcc8e04db8c6eb70a4ac34059850310d5dcb7194f7d310fb`  
		Last Modified: Thu, 01 Jun 2023 17:46:04 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0abdd24eb7958ba4437dc204083be4fa5bab38f70969d9f1a696b42f0fb9995`  
		Last Modified: Thu, 01 Jun 2023 17:46:04 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `cirros:0.6.2` - linux; arm64 variant v8

```console
$ docker pull cirros@sha256:cdb1caacd17effe39a0f7de10ad063ffe48213936c6878ec47f9fd6ac0d4eeaa
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.5 MB (7512951 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c08510651948f20e927663a4e51033d4ed0272eacdb7f2eb22ca02f12de8008b`
-	Default Command: `["\/sbin\/init"]`

```dockerfile
# Thu, 01 Jun 2023 17:47:42 GMT
ADD file:b631ea2eba505c45d900fefe6abe60bf0fd55081d73b533b675497b4ac6fc7e9 in / 
# Thu, 01 Jun 2023 17:47:42 GMT
RUN rm /etc/rc3.d/S40-network
# Thu, 01 Jun 2023 17:47:43 GMT
RUN sed -i '/is_lxc && lxc_netdown/d' /etc/init.d/rc.sysinit
# Thu, 01 Jun 2023 17:47:43 GMT
CMD ["/sbin/init"]
```

-	Layers:
	-	`sha256:9f6485d64479ba46aaa6a5a1ceac7a29a0150c98eeed49ba17c0afe4eb2f7fff`  
		Last Modified: Thu, 01 Jun 2023 17:48:11 GMT  
		Size: 7.5 MB (7511527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be6fd5e2e591cbc25e4761475e2a118e730e79198465438b66eb3a1c993999c7`  
		Last Modified: Thu, 01 Jun 2023 17:48:10 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12503d8dede453a111c6f27f4d55ef0600dbc5b36706fe6d134d3c6f99620be6`  
		Last Modified: Thu, 01 Jun 2023 17:48:10 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `cirros:0.6.2` - linux; ppc64le

```console
$ docker pull cirros@sha256:752d80a265707f0757f06e543fe5bec4893f867be2cb0c65846ae0fc9e06a79d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.9 MB (7893829 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:75f332a1c396c946394238438e7a562e1bbe08e0fe70e267336bdbf3b45a0eed`
-	Default Command: `["\/sbin\/init"]`

```dockerfile
# Thu, 01 Jun 2023 17:47:02 GMT
ADD file:a96c96efad4fc7338db684c36b45a65c81d03475dbb97215d1928b899de72dbf in / 
# Thu, 01 Jun 2023 17:47:06 GMT
RUN rm /etc/rc3.d/S40-network
# Thu, 01 Jun 2023 17:47:08 GMT
RUN sed -i '/is_lxc && lxc_netdown/d' /etc/init.d/rc.sysinit
# Thu, 01 Jun 2023 17:47:09 GMT
CMD ["/sbin/init"]
```

-	Layers:
	-	`sha256:63052c0afd46b074efef54663e7dc1b63492c6d36d602f7bc5b14e9ffeac3f23`  
		Last Modified: Thu, 01 Jun 2023 17:48:10 GMT  
		Size: 7.9 MB (7892397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a0a340c0258d53ee3573a7b2bae98cf43ced4e6cba1b21e35a6cd7bb962ae55`  
		Last Modified: Thu, 01 Jun 2023 17:48:07 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b64dfb5dc29e3f4dbfcd1d631565b9931f7c168341874432f2bca100c31f4a4`  
		Last Modified: Thu, 01 Jun 2023 17:48:07 GMT  
		Size: 1.3 KB (1274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `cirros:latest`

```console
$ docker pull cirros@sha256:f0bc1c8d5421cd424bf8cee3340885dc9ad99fe089e8f1ed485c7a7a82c74307
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `cirros:latest` - linux; amd64

```console
$ docker pull cirros@sha256:04469d1f7155e892eaa5cc0d774b4c8f499dd9f1d2df92c91505775b8b975abc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.4 MB (7415253 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cdb40efc43d69d1840118638fd91da72607c3125101fb428d4ac30e0a3bc5b1b`
-	Default Command: `["\/sbin\/init"]`

```dockerfile
# Tue, 22 Nov 2022 22:24:57 GMT
ADD file:12aef9d2ac43f48be6b03ab418cb5312e4e7f397d71d610afedfbcd1c2c73650 in / 
# Tue, 22 Nov 2022 22:24:57 GMT
RUN rm /etc/rc3.d/S40-network
# Tue, 22 Nov 2022 22:24:58 GMT
RUN sed -i '/is_lxc && lxc_netdown/d' /etc/init.d/rc.sysinit
# Tue, 22 Nov 2022 22:24:58 GMT
CMD ["/sbin/init"]
```

-	Layers:
	-	`sha256:d3ba20487232c21211201e5e9726d4bc5ac60d2db08ca089112733699c52a601`  
		Last Modified: Tue, 22 Nov 2022 22:25:09 GMT  
		Size: 7.4 MB (7413828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8c3cce1196c79818d788e9ce4c53d60d3129ed4e16923aa1184121b903c1a38`  
		Last Modified: Tue, 22 Nov 2022 22:25:08 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:899be78ec08abb367d05c9296da5f3d5701d8c5bd3653eafab2298ae9d53e067`  
		Last Modified: Tue, 22 Nov 2022 22:25:08 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `cirros:latest` - linux; arm variant v7

```console
$ docker pull cirros@sha256:989d58cc2417ceb3997af1d5eec45942bfb96d179de42258ef26feee90d492a3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.9 MB (6917710 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:589a1ac713ab5d2e4ebe435a19733e169d3c3b0b41dc8ba9e5152e9077d69ff7`
-	Default Command: `["\/sbin\/init"]`

```dockerfile
# Thu, 01 Jun 2023 17:45:40 GMT
ADD file:5eedfffbb6342e38402ce33ec22c8e56d5fedf4bbe54378386e677f347a36e3c in / 
# Thu, 01 Jun 2023 17:45:41 GMT
RUN rm /etc/rc3.d/S40-network
# Thu, 01 Jun 2023 17:45:41 GMT
RUN sed -i '/is_lxc && lxc_netdown/d' /etc/init.d/rc.sysinit
# Thu, 01 Jun 2023 17:45:41 GMT
CMD ["/sbin/init"]
```

-	Layers:
	-	`sha256:f80362f561c125292ff108e8158fb93cff22d6c31e7254ff0934beb9d0aedd30`  
		Last Modified: Thu, 01 Jun 2023 17:46:05 GMT  
		Size: 6.9 MB (6916286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc766dd3aab55abadcc8e04db8c6eb70a4ac34059850310d5dcb7194f7d310fb`  
		Last Modified: Thu, 01 Jun 2023 17:46:04 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0abdd24eb7958ba4437dc204083be4fa5bab38f70969d9f1a696b42f0fb9995`  
		Last Modified: Thu, 01 Jun 2023 17:46:04 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `cirros:latest` - linux; arm64 variant v8

```console
$ docker pull cirros@sha256:cdb1caacd17effe39a0f7de10ad063ffe48213936c6878ec47f9fd6ac0d4eeaa
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.5 MB (7512951 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c08510651948f20e927663a4e51033d4ed0272eacdb7f2eb22ca02f12de8008b`
-	Default Command: `["\/sbin\/init"]`

```dockerfile
# Thu, 01 Jun 2023 17:47:42 GMT
ADD file:b631ea2eba505c45d900fefe6abe60bf0fd55081d73b533b675497b4ac6fc7e9 in / 
# Thu, 01 Jun 2023 17:47:42 GMT
RUN rm /etc/rc3.d/S40-network
# Thu, 01 Jun 2023 17:47:43 GMT
RUN sed -i '/is_lxc && lxc_netdown/d' /etc/init.d/rc.sysinit
# Thu, 01 Jun 2023 17:47:43 GMT
CMD ["/sbin/init"]
```

-	Layers:
	-	`sha256:9f6485d64479ba46aaa6a5a1ceac7a29a0150c98eeed49ba17c0afe4eb2f7fff`  
		Last Modified: Thu, 01 Jun 2023 17:48:11 GMT  
		Size: 7.5 MB (7511527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be6fd5e2e591cbc25e4761475e2a118e730e79198465438b66eb3a1c993999c7`  
		Last Modified: Thu, 01 Jun 2023 17:48:10 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12503d8dede453a111c6f27f4d55ef0600dbc5b36706fe6d134d3c6f99620be6`  
		Last Modified: Thu, 01 Jun 2023 17:48:10 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `cirros:latest` - linux; ppc64le

```console
$ docker pull cirros@sha256:752d80a265707f0757f06e543fe5bec4893f867be2cb0c65846ae0fc9e06a79d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.9 MB (7893829 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:75f332a1c396c946394238438e7a562e1bbe08e0fe70e267336bdbf3b45a0eed`
-	Default Command: `["\/sbin\/init"]`

```dockerfile
# Thu, 01 Jun 2023 17:47:02 GMT
ADD file:a96c96efad4fc7338db684c36b45a65c81d03475dbb97215d1928b899de72dbf in / 
# Thu, 01 Jun 2023 17:47:06 GMT
RUN rm /etc/rc3.d/S40-network
# Thu, 01 Jun 2023 17:47:08 GMT
RUN sed -i '/is_lxc && lxc_netdown/d' /etc/init.d/rc.sysinit
# Thu, 01 Jun 2023 17:47:09 GMT
CMD ["/sbin/init"]
```

-	Layers:
	-	`sha256:63052c0afd46b074efef54663e7dc1b63492c6d36d602f7bc5b14e9ffeac3f23`  
		Last Modified: Thu, 01 Jun 2023 17:48:10 GMT  
		Size: 7.9 MB (7892397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a0a340c0258d53ee3573a7b2bae98cf43ced4e6cba1b21e35a6cd7bb962ae55`  
		Last Modified: Thu, 01 Jun 2023 17:48:07 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b64dfb5dc29e3f4dbfcd1d631565b9931f7c168341874432f2bca100c31f4a4`  
		Last Modified: Thu, 01 Jun 2023 17:48:07 GMT  
		Size: 1.3 KB (1274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
