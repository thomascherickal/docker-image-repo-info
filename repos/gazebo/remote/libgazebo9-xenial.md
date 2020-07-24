## `gazebo:libgazebo9-xenial`

```console
$ docker pull gazebo@sha256:0a419782150ae56925874117a51f5c197e9172d54630dfe2accdc2228244f50b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `gazebo:libgazebo9-xenial` - linux; amd64

```console
$ docker pull gazebo@sha256:0ce65710641e60b6747a1a719e7b21edff86c5f7b68a41814dafc1fea94214c4
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **493.6 MB (493601923 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4eff2ac2397a7365bca9b5f6330078c847f312f337edf5c9e58f9d95866b149`
-	Entrypoint: `["\/gzserver_entrypoint.sh"]`
-	Default Command: `["gzserver"]`

```dockerfile
# Fri, 24 Jul 2020 14:39:06 GMT
ADD file:513ae777bc4042f8446c0454f8cffc9a94f8429de963651d9a6dab95d4502007 in / 
# Fri, 24 Jul 2020 14:39:07 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 14:39:07 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Jul 2020 14:39:08 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Jul 2020 14:39:08 GMT
CMD ["/bin/bash"]
# Fri, 24 Jul 2020 15:37:33 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     lsb-release     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 15:37:39 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys D2486D2DD83DB69272AFE98867170598AF249743
# Fri, 24 Jul 2020 15:37:40 GMT
RUN . /etc/os-release     && echo "deb http://packages.osrfoundation.org/gazebo/$ID-stable `lsb_release -sc` main" > /etc/apt/sources.list.d/gazebo-latest.list
# Fri, 24 Jul 2020 15:42:35 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     gazebo9=9.13.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 15:42:36 GMT
EXPOSE 11345
# Fri, 24 Jul 2020 15:42:36 GMT
COPY file:b79966dec12c55a0a5c9e673326cc3faf9cbbeee0ea5f172e863df237eb8a601 in / 
# Fri, 24 Jul 2020 15:42:36 GMT
ENTRYPOINT ["/gzserver_entrypoint.sh"]
# Fri, 24 Jul 2020 15:42:36 GMT
CMD ["gzserver"]
# Fri, 24 Jul 2020 15:44:03 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     libgazebo9-dev=9.13.2-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7b378fa0f9085667ced1c76c9919cde8663becf2218e8d20e2df8d0824311531`  
		Last Modified: Tue, 07 Jul 2020 13:19:56 GMT  
		Size: 44.4 MB (44401021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d77b1b29f2e9b6f141b9d8f74b601f40eb998544783f4a0a3cdc384873c1a4e`  
		Last Modified: Fri, 24 Jul 2020 14:39:50 GMT  
		Size: 529.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c793be88baee3f3204444e4d4e49c4e44c1709d40182c131cd5681c94e17227`  
		Last Modified: Fri, 24 Jul 2020 14:39:50 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecc05c8a19c0cf83f2f44263c967c3fe81fffc4b41b592ad088fb1534c206e70`  
		Last Modified: Fri, 24 Jul 2020 14:39:49 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d916041f92a6961d82541630abdb30c1498f924d9977c3b38b91678d1c02a601`  
		Last Modified: Fri, 24 Jul 2020 16:01:59 GMT  
		Size: 16.3 MB (16275937 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27666f170c8634cda060ed942cc86470f03058b3e1544ed9a00a260afe6772ac`  
		Last Modified: Fri, 24 Jul 2020 16:01:55 GMT  
		Size: 14.8 KB (14760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e238795d3354ffbeb7f8a071aadaa9303991d0ac42081be50479bbb688b7c69e`  
		Last Modified: Fri, 24 Jul 2020 16:01:55 GMT  
		Size: 5.5 KB (5525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba09bf0088affd311d90108b84c0a478a3f7f131f996f27358433f647758b669`  
		Last Modified: Fri, 24 Jul 2020 16:03:53 GMT  
		Size: 208.2 MB (208229225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df7f21021ada008f3f0a02f1b4703dc12078c4a954562f101187c37767883f68`  
		Last Modified: Fri, 24 Jul 2020 16:03:24 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:522dcef8c3ea4b77f4b31abd70d0361e487bbf589c2c0838bba94d561c3aa5a9`  
		Last Modified: Fri, 24 Jul 2020 16:05:03 GMT  
		Size: 224.7 MB (224673722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
