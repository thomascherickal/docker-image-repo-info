## `debian:rc-buggy`

```console
$ docker pull debian@sha256:f293fa56cc727a4162d17ccfa9125aa81805f65a9ae3e08a1c710d86a0415538
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; s390x

### `debian:rc-buggy` - linux; amd64

```console
$ docker pull debian@sha256:1e11153d3b4484a203bc1610744433862c6ba793d072e25b2d7621efa0a0aeb0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.5 MB (49463151 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:34d484f02063b14a93fdcea8b69b6ecff5a3e9d12758c81f7ff60ef4d62c75a4`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 Jul 2023 23:26:24 GMT
ADD file:89538c836015e15bfe955d940c080e251ce5b25e2cfaac73d8ce77f8475cd08f in / 
# Thu, 27 Jul 2023 23:26:25 GMT
CMD ["bash"]
# Thu, 27 Jul 2023 23:28:07 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:9828fc546889681c4c23160b0ee9abb2a08f99ec58b166856cf38d03e0173700`  
		Last Modified: Thu, 27 Jul 2023 23:32:15 GMT  
		Size: 49.5 MB (49462924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9ea8b9e0e4a03e9243f81c206973da2f4c8da590afe79e7409d929dff2386c2`  
		Last Modified: Thu, 27 Jul 2023 23:34:52 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; arm variant v5

```console
$ docker pull debian@sha256:d84cf30ada971a1cddac23cf6ed9b92d4bd89cc4efaeb107fce78317f2aaa29a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.4 MB (47404006 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:94304158ee40407d7606f1650e6375fe54d2f992a42ca2fcaa21bf4ba98da0d2`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Aug 2023 23:49:11 GMT
ADD file:2d486f4790de50d5a173ed5147c22ebcaaade283f5bdf6b62bc072050fc164c1 in / 
# Tue, 15 Aug 2023 23:49:11 GMT
CMD ["bash"]
# Tue, 15 Aug 2023 23:50:23 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:0fb27bc4b8f884dd1bc1129dd87397bcc993ec915005657bd21811eb84745100`  
		Last Modified: Tue, 15 Aug 2023 23:53:08 GMT  
		Size: 47.4 MB (47403781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fadaab52d9ba2255d3467baf5c79a0867bbb0a36dd36fa8906d0f8482aa039b8`  
		Last Modified: Tue, 15 Aug 2023 23:55:49 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; arm variant v7

```console
$ docker pull debian@sha256:6d43c7d3770a1663b32b6699abc70b94fac6a7c8df530b80a892a777f04c045f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.0 MB (45003433 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:20a9a05a44bbb7cbb4bb9a9dfa93671edd03b9eda99b5e7f17fffa804dad4bba`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 Jul 2023 23:59:54 GMT
ADD file:751198e94159fde0051292c0a2bcc0ae0c4b82b34b63913cd6860cbed520b9b6 in / 
# Thu, 27 Jul 2023 23:59:55 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 00:01:46 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:d8947caaed239612a0bd233bb275a710201bd19a169719c1541890b12489b8ff`  
		Last Modified: Fri, 28 Jul 2023 00:06:07 GMT  
		Size: 45.0 MB (45003207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0c0dc76c5426de57e21f90855e7b1b00e13339a9bd7a0a5157871bcb1982692`  
		Last Modified: Fri, 28 Jul 2023 00:08:52 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:72557e4de2cc0e083fff30ca9d73df0c8af932165da5f71e4c3a9378008e0488
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.5 MB (49531955 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c427542b410257ab6d703b5771148d09c1abac348563ca67103b5f9740d3c098`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Aug 2023 23:41:01 GMT
ADD file:8064072457ccf7b4072e08095fa84f96b0fe3387ec8f302afde022186aa3eab5 in / 
# Tue, 15 Aug 2023 23:41:01 GMT
CMD ["bash"]
# Tue, 15 Aug 2023 23:42:07 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:4513653e4d749342b34f60c592adaf0ef4af993e76a913a1c086a4229a0e3afe`  
		Last Modified: Tue, 15 Aug 2023 23:45:54 GMT  
		Size: 49.5 MB (49531730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:faa17cee307bdacaae57f147ba0619032cfffadd04964efbb24024ca12ea8837`  
		Last Modified: Tue, 15 Aug 2023 23:48:22 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; 386

```console
$ docker pull debian@sha256:a6f79caae9ab92f696cea7ebba8472268e1fd5fc7287ce82716a1dcdde1e1d26
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.6 MB (50631580 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:54d4395e55f3f09d62d21748f768187def9b8806b094607456ced6211b7252ee`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Aug 2023 23:40:34 GMT
ADD file:d86f66385d3993c597ac040a976cd8a826b097d014cc4f3b69d8ebfaa5aa6eff in / 
# Tue, 15 Aug 2023 23:40:35 GMT
CMD ["bash"]
# Tue, 15 Aug 2023 23:42:05 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:e41394c7daa90fb4aae0f67d43af5ee9838fb125e249fc0002bfdc3b90bb6c05`  
		Last Modified: Tue, 15 Aug 2023 23:46:33 GMT  
		Size: 50.6 MB (50631355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e323c216a876bebcbf917fb42c503130745bb8533dff5c6243677f5816c2fb8e`  
		Last Modified: Tue, 15 Aug 2023 23:49:31 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; mips64le

```console
$ docker pull debian@sha256:5d62c8bbd30741be4a46ad5aed8cdf6a1e77dc8848ea7600038b18b7f2bdac4e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.3 MB (49334828 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:87eddb86c72e3a428fa758fc6c99264c54ce704fbbe122afca84f5b83cc0edfa`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 Jul 2023 23:14:28 GMT
ADD file:5d5d4b53ad51debb95681500ba4a990279ff7fdd2ff80d4d4333b7dc647c0543 in / 
# Thu, 27 Jul 2023 23:14:34 GMT
CMD ["bash"]
# Thu, 27 Jul 2023 23:20:16 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:9b48d6f46b6cff8bfdf81f7ffbfa05dff828e1d7545e640bf61d5486c1b79892`  
		Last Modified: Thu, 27 Jul 2023 23:25:52 GMT  
		Size: 49.3 MB (49334598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f85a4c3976f20baa4e54ed40f7ae98a0166a9310df179b9c87fe9128f9950665`  
		Last Modified: Thu, 27 Jul 2023 23:31:32 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; ppc64le

```console
$ docker pull debian@sha256:eb66caf34e4f162f1b37cfccbd8a9f9518876c82e4f0957b6176a28769d48284
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.4 MB (53379473 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e183bb0683367269ebb4ef57cf49e36562abf5b21dfd09ccc19af52911e502ce`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 Jul 2023 23:24:36 GMT
ADD file:c9a8e26186be211989debc20aaaea2b9b0a88ef3c95dc67df08fb292c70fd107 in / 
# Thu, 27 Jul 2023 23:24:39 GMT
CMD ["bash"]
# Thu, 27 Jul 2023 23:27:23 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:8a2370b39a2d35f89bb2978a591923ded0652ff040aa00a837d799ffdb028e76`  
		Last Modified: Thu, 27 Jul 2023 23:31:58 GMT  
		Size: 53.4 MB (53379244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ea4efeeef38c228063db4c9b70e8e6584d62e4797993239070f8b17e27b226e`  
		Last Modified: Thu, 27 Jul 2023 23:36:04 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; s390x

```console
$ docker pull debian@sha256:6cc309ca7893ab8b32b72ae06d2826ab2a8c89a38177ef8ffb8966116f1afad7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.6 MB (48594621 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:755590bbeb7ab6bb277eb1794c5a52b2f86c06b4ffd45cee2a3918083c9e42ed`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Aug 2023 23:43:50 GMT
ADD file:a27e7d7c954291d644437a8054f06f492700f1ce13d3a9e2c3bbd71afd0869cf in / 
# Tue, 15 Aug 2023 23:43:56 GMT
CMD ["bash"]
# Tue, 15 Aug 2023 23:46:34 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:db9f34e47daed3854a411cee94f611a7139b82002ae54802c9a44d3faccaaea7`  
		Last Modified: Tue, 15 Aug 2023 23:49:01 GMT  
		Size: 48.6 MB (48594395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c45c97c49f18f8a1b027269794dab7d477ddaac2db4db8112ea7c2bd0e0c6d09`  
		Last Modified: Tue, 15 Aug 2023 23:51:01 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
