## `nats:latest`

```console
$ docker pull nats@sha256:4cc6ae97db8f844bcb32288362ff30125146324890be158dc006e0d6bc7d4a65
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.1817; amd64

### `nats:latest` - linux; amd64

```console
$ docker pull nats@sha256:ebea070618f2459bc2f6a200dadc2f1a4c0763212c361372b62e98660433e12b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4185085 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8bd9298a0432fe41651ac7852910e0de92e1bde3bd7497195ffc861b4785d3f0`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 15 Mar 2021 20:38:14 GMT
COPY file:b5d1e003164e33741898b7ec26a4040874906b36efbc359506c187ae6df7c294 in /nats-server 
# Mon, 15 Mar 2021 20:38:14 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Mon, 15 Mar 2021 20:38:15 GMT
EXPOSE 4222 6222 8222
# Mon, 15 Mar 2021 20:38:15 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 15 Mar 2021 20:38:15 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:061215568e0623f6f43c6616f33a9bea7665a183db6a276a6038af3f305833d6`  
		Last Modified: Mon, 15 Mar 2021 20:39:10 GMT  
		Size: 4.2 MB (4184610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05331b79a067343f06d2c17089ee22d3cd8193f712ae7647b0977867e36bc36a`  
		Last Modified: Mon, 15 Mar 2021 20:39:09 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm variant v6

```console
$ docker pull nats@sha256:81a7d3301eb008ada26d22889711a883bbad763673b54f7593f2445d22298acd
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3859233 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b8dc88c3bd1fffabc0615fa001fa033818d9eee65d62c50afed1958c58045ab4`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 15 Mar 2021 21:17:04 GMT
COPY file:d436e7cf1178e7919a5eeaba22715cc73a25f54e3b98dc4c2511f0969af50c7d in /nats-server 
# Mon, 15 Mar 2021 21:17:05 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Mon, 15 Mar 2021 21:17:06 GMT
EXPOSE 4222 6222 8222
# Mon, 15 Mar 2021 21:17:07 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 15 Mar 2021 21:17:08 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:029a8ef0b1c1c9cd107dd578ac757718ad474948fd5e7b25aacc28f3507dca3e`  
		Last Modified: Mon, 15 Mar 2021 21:17:49 GMT  
		Size: 3.9 MB (3858758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3658434d7560f8e07a195f69d5fca2be87c52936bbebb0443bb8d30b36aa0072`  
		Last Modified: Mon, 15 Mar 2021 21:17:48 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm variant v7

```console
$ docker pull nats@sha256:b2e5433b90b1cdd96decdc44183063bffcc7b73e088c1033edccb1afd8a5c17f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3855937 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e2b8659db05958c00c35ed9fbd5356e048d3585f6ab0de6b4ad63250f013741f`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 15 Mar 2021 21:24:57 GMT
COPY file:68bb849e5773af4031f3eed004a40bf4f742c3945319085d56bee16a0a9207d2 in /nats-server 
# Mon, 15 Mar 2021 21:24:58 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Mon, 15 Mar 2021 21:24:59 GMT
EXPOSE 4222 6222 8222
# Mon, 15 Mar 2021 21:25:00 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 15 Mar 2021 21:25:01 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:0e6b2bfbd8fee738af6e2eb535451184e1cfa44d6189259fc78a03247687a7a3`  
		Last Modified: Mon, 15 Mar 2021 21:25:48 GMT  
		Size: 3.9 MB (3855460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc5a766cb9431ee6ca3fa9462f0b1cd15de1270719b74fe5f17e3bbbf75acbc0`  
		Last Modified: Mon, 15 Mar 2021 21:25:47 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:68284dadffb40430476fffec3f3f3175e215e0efbd8ebb3b84d61745afbc8208
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3826067 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9c42fd7b12781200e6e26a21ac0f074a31c2bb3ab913378dbbd126c5e1dc232`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 15 Mar 2021 22:15:07 GMT
COPY file:cc5a975f9a3d3dec9e7c117963cb0f29cccd7a6d9891efe13202d82f16983d97 in /nats-server 
# Mon, 15 Mar 2021 22:15:08 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Mon, 15 Mar 2021 22:15:09 GMT
EXPOSE 4222 6222 8222
# Mon, 15 Mar 2021 22:15:10 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 15 Mar 2021 22:15:10 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6dfc8ec71d6cbeecdf9b73546e133c54fe31a144e705660e1732d4c3fd7cec38`  
		Last Modified: Mon, 15 Mar 2021 22:16:28 GMT  
		Size: 3.8 MB (3825589 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8298fc0383beb85f28b7722738f7772924405727f566aba126c37b60b6fb55d4`  
		Last Modified: Mon, 15 Mar 2021 22:16:27 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - windows version 10.0.17763.1817; amd64

```console
$ docker pull nats@sha256:3621f57fd3c277ec4cbe88e91a364bb90b3a614178b075b262025c69902f6749
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.6 MB (105632823 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80a15211278567816e8c2d0069b2ff094c0b9dcb8cf04e2d51d41006e2004719`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 26 Feb 2021 16:47:31 GMT
RUN Apply image 1809-amd64
# Wed, 10 Mar 2021 16:56:55 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Mon, 15 Mar 2021 20:17:12 GMT
RUN cmd /S /C #(nop) COPY file:ae552f9fffc5cd2f6ed45296e57705c2f61343b2c0e5351c85ccd047adfa7b73 in C:\nats-server.exe 
# Mon, 15 Mar 2021 20:17:13 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Mon, 15 Mar 2021 20:17:14 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Mon, 15 Mar 2021 20:17:15 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Mon, 15 Mar 2021 20:17:16 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a11c4ca8f1ba16b6e1395d4523be2215bd0871c2e3e4695b9f2b87bd7472be52`  
		Size: 101.4 MB (101389964 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f49969195f32b7e40a81e3d189259fec7ebf52ee0ec5dafd5f3f288715354fed`  
		Last Modified: Wed, 10 Mar 2021 17:01:57 GMT  
		Size: 1.0 KB (1047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e8ae67f49930ee74c376428149104959d1ff9583b9fdbb41fdb5aed581931f2`  
		Last Modified: Mon, 15 Mar 2021 20:22:15 GMT  
		Size: 4.2 MB (4236588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7f29b29488ecf17138eea47d55def6573211a3f9a3e68a1fa63e5cd412339d2`  
		Last Modified: Mon, 15 Mar 2021 20:22:14 GMT  
		Size: 1.8 KB (1773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deb3d7ef6e3c578d1823bbe7699b42e32f024d0b5de366ce42cf2cfd46ad2f76`  
		Last Modified: Mon, 15 Mar 2021 20:22:14 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bfa0a814bb44d3fb408de44b16509731ff63e96cea480295bb63dfc15fe5789`  
		Last Modified: Mon, 15 Mar 2021 20:22:14 GMT  
		Size: 1.2 KB (1167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3d3b5144a635921fbead0a95e2d3a141eddba274abd7c281b40fadc3d13e121`  
		Last Modified: Mon, 15 Mar 2021 20:22:14 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
