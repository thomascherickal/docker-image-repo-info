## `cirros:latest`

```console
$ docker pull cirros@sha256:be6f5d1ab1e463e7991ecb29f1e71993d633ff1d190188662085ef641bdcf389
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `cirros:latest` - linux; amd64

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

### `cirros:latest` - linux; arm variant v5

```console
$ docker pull cirros@sha256:99f4ab71a597d62de0b564acd772e4a645596cd0c6e1edb21c5f871f5abf334b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.6 MB (5634246 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7d31ee5281129d677d247c14ec880e570a9bf7673b45b366a4d6dabc106205ac`
-	Default Command: `["\/sbin\/init"]`

```dockerfile
# Tue, 21 Jun 2022 06:51:38 GMT
ADD file:d452db6e53e5ba209c771ecfc8acc0e1991f018f8578e48e0d0dce69e46395b9 in / 
# Tue, 21 Jun 2022 06:51:40 GMT
RUN rm /etc/rc3.d/S40-network
# Tue, 21 Jun 2022 06:51:41 GMT
RUN sed -i '/is_lxc && lxc_netdown/d' /etc/init.d/rc.sysinit
# Tue, 21 Jun 2022 06:51:42 GMT
CMD ["/sbin/init"]
```

-	Layers:
	-	`sha256:231303b903e38cc8d918f588a01a3320b9fb4b4c95fa20f9852b95624c251df9`  
		Last Modified: Mon, 08 Mar 2021 21:51:37 GMT  
		Size: 5.6 MB (5632836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28ed6471769f7f3e072934bd34d9866785f200b125732e2859c4ce4f0c48b8f2`  
		Last Modified: Tue, 21 Jun 2022 06:52:16 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:511fcacf758453879c95ef28db5432536d4649198a8ff64de37e07c2e195681b`  
		Last Modified: Tue, 21 Jun 2022 06:52:15 GMT  
		Size: 1.3 KB (1253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `cirros:latest` - linux; arm64 variant v8

```console
$ docker pull cirros@sha256:ab30156e31b5921bc17060725729a67058a27cdf3d65f9432a1d5d9c843a8e26
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.4 MB (5381559 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a296a5a9b16435a4be2f250deda463c75cf9a250fa1a2c4d4a235a69c91a79b4`
-	Default Command: `["\/sbin\/init"]`

```dockerfile
# Sun, 08 May 2022 19:54:27 GMT
ADD file:7f294f3d60585f86a27be204f949a663c79c9187a153fe00b725e8fa062cf493 in / 
# Sun, 08 May 2022 19:54:28 GMT
RUN rm /etc/rc3.d/S40-network
# Sun, 08 May 2022 19:54:29 GMT
RUN sed -i '/is_lxc && lxc_netdown/d' /etc/init.d/rc.sysinit
# Sun, 08 May 2022 19:54:30 GMT
CMD ["/sbin/init"]
```

-	Layers:
	-	`sha256:e6a197a3618a47fbe537101b254c366a779102387d42cf6a37a38f61534ab352`  
		Last Modified: Mon, 08 Mar 2021 21:43:20 GMT  
		Size: 5.4 MB (5380157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ba64309d602fc578d19f836f771c1f346a9823aa59b2d615e8d64618333b0fa`  
		Last Modified: Sun, 08 May 2022 19:55:41 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d98d987dcf6805875debbc870ea35c21d3c980949d403f0f31f57f965437259e`  
		Last Modified: Sun, 08 May 2022 19:55:41 GMT  
		Size: 1.2 KB (1248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `cirros:latest` - linux; 386

```console
$ docker pull cirros@sha256:111dd6cf830531a11fe07cede5845cb0c6f020171e485f2f1b3342714b99bcaa
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.5 MB (5531817 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2fb487fd3a0f68afa6592346edf47ea792e2bfdb0367455103ee21c9e8e3b91f`
-	Default Command: `["\/sbin\/init"]`

```dockerfile
# Mon, 08 Mar 2021 22:01:41 GMT
ADD file:6fe295a0acec8cf81b2eb7b6868ad7e913a4b8d73574bdacba578b3d05d4f2d5 in / 
# Mon, 08 Mar 2021 22:01:42 GMT
RUN rm /etc/rc3.d/S40-network
# Mon, 08 Mar 2021 22:01:43 GMT
RUN sed -i '/is_lxc && lxc_netdown/d' /etc/init.d/rc.sysinit
# Mon, 08 Mar 2021 22:01:43 GMT
CMD ["/sbin/init"]
```

-	Layers:
	-	`sha256:6ec03cf697719ca502eb22d6de2bc3d696c52a6ba02d190332a1f21e542e048d`  
		Last Modified: Mon, 08 Mar 2021 22:02:01 GMT  
		Size: 5.5 MB (5530412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70f1cfcdb21741b197e2bc5bf26ca7b0f5792f154130c3f88b26e44b50e57d07`  
		Last Modified: Mon, 08 Mar 2021 22:02:00 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b14a0418e0a405f9acd1059962a1d26ca670fb5a4b764969ba3995282615d461`  
		Last Modified: Mon, 08 Mar 2021 22:02:00 GMT  
		Size: 1.2 KB (1248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `cirros:latest` - linux; ppc64le

```console
$ docker pull cirros@sha256:d73c78dc6c4a275c6cb1bf46654ede0305b76b430a8cb3e9d114315c1f4d2ad1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 MB (5770839 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93df8c5c52071e4dd5e2ca046f7d33481ea590317b92611c992dc101cf9f9b2c`
-	Default Command: `["\/sbin\/init"]`

```dockerfile
# Mon, 08 Mar 2021 21:33:05 GMT
ADD file:37ce090900e2d750646c4d7da4fbb79559e30b5b817c833396c86613236ba838 in / 
# Mon, 08 Mar 2021 21:33:21 GMT
RUN rm /etc/rc3.d/S40-network
# Mon, 08 Mar 2021 21:33:33 GMT
RUN sed -i '/is_lxc && lxc_netdown/d' /etc/init.d/rc.sysinit
# Mon, 08 Mar 2021 21:33:39 GMT
CMD ["/sbin/init"]
```

-	Layers:
	-	`sha256:587c91809a2ae1af15d948969c3a1adb2aad2dbe2cbb6a2b8982a5cf9d14c7ef`  
		Last Modified: Mon, 08 Mar 2021 21:34:03 GMT  
		Size: 5.8 MB (5769433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01739d1b3e0963fe3d0194afd70a85c6098f0139dff49965d2ce40342d33de96`  
		Last Modified: Mon, 08 Mar 2021 21:34:01 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2169930d58d52208fd25b17049537fa4ec9192f04fc372a1cb57a20d7a8d3fd`  
		Last Modified: Mon, 08 Mar 2021 21:34:01 GMT  
		Size: 1.3 KB (1252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
