## `openjdk:16-jdk`

```console
$ docker pull openjdk@sha256:712204b08b876abcca939c87d8b2b53aa9d1e652fdb3437b22623fc8275cdc2a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.1518; amd64
	-	windows version 10.0.14393.3986; amd64

### `openjdk:16-jdk` - linux; amd64

```console
$ docker pull openjdk@sha256:5a694c0e085f06ec915f841ebc9d52ecf3fb9665b9be83ae3c35bbeac0dfc7c1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **264.3 MB (264319025 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:829f2807d9cc9829e53775a5c75c6cc923f5642a7d95a4fb216eaae1bad31c59`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 15 Sep 2020 21:22:07 GMT
LABEL org.opencontainers.image.authors=Oracle Linux Product Team <ol-ovm-info_ww@oracle.com> org.opencontainers.image.url=https://github.com/oracle/container-images org.opencontainers.image.source=https://github.com/oracle/container-images/tree/dist-amd64/8-slim org.opencontainers.image.vendor=Oracle America, Inc org.opencontainers.image.title=Oracle Linux 8 (slim) org.opencontainers.image.description=Oracle Linux is an open-source       operating system available under the GNU General Public License (GPLv2) and       is suitable for both general purpose or Oracle workloads.
# Thu, 22 Oct 2020 02:16:12 GMT
ADD file:dab686af43f04bdaabbdbe7703e0c2dc85868a5dbb38942747055a44e038f37f in / 
# Thu, 22 Oct 2020 02:16:12 GMT
CMD ["/bin/bash"]
# Thu, 22 Oct 2020 02:34:47 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Thu, 22 Oct 2020 02:34:47 GMT
ENV LANG=C.UTF-8
# Thu, 22 Oct 2020 02:34:48 GMT
ENV JAVA_HOME=/usr/java/openjdk-16
# Thu, 22 Oct 2020 02:34:48 GMT
ENV PATH=/usr/java/openjdk-16/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Oct 2020 02:34:48 GMT
ENV JAVA_VERSION=16-ea+20
# Thu, 22 Oct 2020 02:35:32 GMT
RUN set -eux; 		objdump="$(command -v objdump)"; 	arch="$(objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		arm64 | aarch64) 			downloadUrl=https://download.java.net/java/early_access/jdk16/20/GPL/openjdk-16-ea+20_linux-aarch64_bin.tar.gz; 			downloadSha256=5226280cbdaec7e5327d77282717f6a5f716f9437194dd3d464059fbdcfbd8be; 			;; 		amd64 | i386:x86-64) 			downloadUrl=https://download.java.net/java/early_access/jdk16/20/GPL/openjdk-16-ea+20_linux-x64_bin.tar.gz; 			downloadSha256=98b09726ff551251f988fdd812123a0e33effc5ec3ca45d58ab200f911397fff; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Thu, 22 Oct 2020 02:35:33 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:fd3d5e431db632e40b1f1d5ed9a34a906447d43146906e56da1f14f07998bc28`  
		Last Modified: Thu, 22 Oct 2020 02:18:09 GMT  
		Size: 54.2 MB (54161024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1004722dc5e0b01dbfaadfde989754299882cd0cd89e7da3f08996ffde63d55e`  
		Last Modified: Thu, 22 Oct 2020 02:44:53 GMT  
		Size: 13.5 MB (13493854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f1f643e88ad25e2aae7856fcb9ed525ece7d6e7ffde6f832f17d4f3d176d683`  
		Last Modified: Thu, 22 Oct 2020 02:45:12 GMT  
		Size: 196.7 MB (196664147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:16-jdk` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:7cddd6cb45d29469389ee967c54366507e9f8d23bf997c4d984a2e55e0a6a3d2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **246.2 MB (246201830 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1437530785f1eec92d657a5f4d454b082af0fc9c3c3b2582136cf77effa96e9a`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 15 Sep 2020 20:40:54 GMT
LABEL org.opencontainers.image.authors=Oracle Linux Product Team <ol-ovm-info_ww@oracle.com> org.opencontainers.image.url=https://github.com/oracle/container-images org.opencontainers.image.source=https://github.com/oracle/container-images/tree/dist-arm64v8/8-slim org.opencontainers.image.vendor=Oracle America, Inc org.opencontainers.image.title=Oracle Linux 8 (slim) org.opencontainers.image.description=Oracle Linux is an open-source       operating system available under the GNU General Public License (GPLv2) and       is suitable for both general purpose or Oracle workloads.
# Thu, 22 Oct 2020 02:02:57 GMT
ADD file:91f94052d144e7fac61501c6d72e663eda67c40303d29f0b62fda4abe0e5a284 in / 
# Thu, 22 Oct 2020 02:03:00 GMT
CMD ["/bin/bash"]
# Thu, 22 Oct 2020 09:16:39 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Thu, 22 Oct 2020 09:16:41 GMT
ENV LANG=C.UTF-8
# Thu, 22 Oct 2020 09:16:41 GMT
ENV JAVA_HOME=/usr/java/openjdk-16
# Thu, 22 Oct 2020 09:16:42 GMT
ENV PATH=/usr/java/openjdk-16/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Oct 2020 22:45:37 GMT
ENV JAVA_VERSION=16-ea+21
# Thu, 22 Oct 2020 22:46:34 GMT
RUN set -eux; 		objdump="$(command -v objdump)"; 	arch="$(objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		arm64 | aarch64) 			downloadUrl=https://download.java.net/java/early_access/jdk16/21/GPL/openjdk-16-ea+21_linux-aarch64_bin.tar.gz; 			downloadSha256=bee09458526a8c10a40f3d4e5bf6c384b1bbc6f9002997d2f4c0d8c090cca1f8; 			;; 		amd64 | i386:x86-64) 			downloadUrl=https://download.java.net/java/early_access/jdk16/21/GPL/openjdk-16-ea+21_linux-x64_bin.tar.gz; 			downloadSha256=3294d805c6125a6dd55a387f82f74df0c9fc0bce06934061fb3ff2dd42075b33; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Thu, 22 Oct 2020 22:46:36 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:428aa11a26cf7698a25c3ec8f290dd1667191a70a5797b7232fa597f1e52ec1b`  
		Last Modified: Thu, 22 Oct 2020 02:04:59 GMT  
		Size: 54.3 MB (54285957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e761c4ae4b3b9dbb16537c08ceb4e5ad0d91323e105a8b241ae8c7538fa70b1f`  
		Last Modified: Thu, 22 Oct 2020 09:24:38 GMT  
		Size: 14.4 MB (14381453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:179bc4e532061314a92eae26ee461a1638f9c817713e3e649451d0028402ea6f`  
		Last Modified: Thu, 22 Oct 2020 22:55:31 GMT  
		Size: 177.5 MB (177534420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:16-jdk` - windows version 10.0.17763.1518; amd64

```console
$ docker pull openjdk@sha256:c083054b5162f71109158a523607d6e7fa9eaef1390652840a2e3c41ee0bfd27
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2580689420 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa497f9e0bab1cdbf3a111e19329c9560484fed13ea9dd1e052233d01cc3fbba`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 01 Oct 2020 02:26:38 GMT
RUN Install update 1809-amd64
# Wed, 14 Oct 2020 12:27:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Oct 2020 17:38:17 GMT
RUN Write-Host 'Enabling TLS 1.2 (https://githubengineering.com/crypto-removal-notice/) ...'; 	$tls12RegBase = 'HKLM:\\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2'; 	if (Test-Path $tls12RegBase) { throw ('"{0}" already exists!' -f $tls12RegBase) }; 	New-Item -Path ('{0}/Client' -f $tls12RegBase) -Force; 	New-Item -Path ('{0}/Server' -f $tls12RegBase) -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force
# Wed, 14 Oct 2020 17:38:18 GMT
ENV JAVA_HOME=C:\openjdk-16
# Wed, 14 Oct 2020 17:38:40 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath
# Fri, 16 Oct 2020 20:15:22 GMT
ENV JAVA_VERSION=16-ea+20
# Fri, 16 Oct 2020 20:15:23 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk16/20/GPL/openjdk-16-ea+20_windows-x64_bin.zip
# Fri, 16 Oct 2020 20:15:24 GMT
ENV JAVA_SHA256=839776e00748de020446146c67c6bfc9b3ed23df27647fddb9240ab64e24a1fb
# Fri, 16 Oct 2020 20:17:08 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Fri, 16 Oct 2020 20:17:09 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:406ffb8432a757e84f7594e85c676620dec6955e0475ac271aa4dd5c0531190d`  
		Size: 655.8 MB (655757265 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5e61fff845eda39f31bdf5d797254fdf656ee79d8c294c1713007864bc4c2535`  
		Last Modified: Wed, 14 Oct 2020 12:50:32 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b5f8e5825cfa7b4f8c5a50657da7a44c0547d90306b4fa11bbf82021b684262`  
		Last Modified: Wed, 14 Oct 2020 18:26:50 GMT  
		Size: 9.2 MB (9230486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01e034563561e5379df3a00fd4da250e977243aacd8623dc768db3ef40497b87`  
		Last Modified: Wed, 14 Oct 2020 18:26:42 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24997a5d1f99495d60fc79a47ec6d7bcf172f637b322078eccbc230cebf01c74`  
		Last Modified: Wed, 14 Oct 2020 18:26:42 GMT  
		Size: 307.8 KB (307821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b01ca4720822e5941f65252dfcbeac392bf539be2037c58f24b938c277ef2a3`  
		Last Modified: Fri, 16 Oct 2020 20:29:39 GMT  
		Size: 1.2 KB (1161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8284d001b5080d15c32d985b915285fdada0f0db5f71677ebdf677c8ac480287`  
		Last Modified: Fri, 16 Oct 2020 20:29:40 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2dee5fbef6f4b5139a26e4e36128b7563ef735525d5b84d8388878295171359`  
		Last Modified: Fri, 16 Oct 2020 20:29:39 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18dc165b4559d0fdce28cd2f1d6c8f54f26a7cb075a751a7643121c56996c80d`  
		Last Modified: Fri, 16 Oct 2020 20:30:00 GMT  
		Size: 197.1 MB (197054125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:977d3eac884b1a4d19188987d3d522e8a92190a352c51e2a5933f710fd1bf9ee`  
		Last Modified: Fri, 16 Oct 2020 20:29:39 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:16-jdk` - windows version 10.0.14393.3986; amd64

```console
$ docker pull openjdk@sha256:324da5eab2ac09d9a2c7ed0b1940bf7f3f6e375aa5e93297ddd2dffd00677285
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (5958856266 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4add2a68a6c62bbd8e055b963df69e7aed073747e94766141086d6c6cb035e93`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Fri, 02 Oct 2020 17:07:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 14 Oct 2020 12:31:45 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Oct 2020 17:42:04 GMT
RUN Write-Host 'Enabling TLS 1.2 (https://githubengineering.com/crypto-removal-notice/) ...'; 	$tls12RegBase = 'HKLM:\\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2'; 	if (Test-Path $tls12RegBase) { throw ('"{0}" already exists!' -f $tls12RegBase) }; 	New-Item -Path ('{0}/Client' -f $tls12RegBase) -Force; 	New-Item -Path ('{0}/Server' -f $tls12RegBase) -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force
# Wed, 14 Oct 2020 17:42:05 GMT
ENV JAVA_HOME=C:\openjdk-16
# Wed, 14 Oct 2020 17:43:23 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath
# Fri, 16 Oct 2020 20:17:19 GMT
ENV JAVA_VERSION=16-ea+20
# Fri, 16 Oct 2020 20:17:20 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk16/20/GPL/openjdk-16-ea+20_windows-x64_bin.zip
# Fri, 16 Oct 2020 20:17:20 GMT
ENV JAVA_SHA256=839776e00748de020446146c67c6bfc9b3ed23df27647fddb9240ab64e24a1fb
# Fri, 16 Oct 2020 20:20:01 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Fri, 16 Oct 2020 20:20:02 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:17a32268498b2feefa5457f0423ac15473596d514e48c694ef54d740a9a5067d`  
		Size: 1.7 GB (1671365753 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e300a13db0fbbf48a676ace9db3b0de292c825dfa01e6d82979d96ebc23d3675`  
		Last Modified: Wed, 14 Oct 2020 12:51:34 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e48f75bae068c25f8a226647b58c0be2010ed0c8cd6921bdc70e67addcbf5a03`  
		Last Modified: Wed, 14 Oct 2020 18:30:55 GMT  
		Size: 9.9 MB (9914428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:380be8c20c0be6ed94b2345de72a72dc8fa948cfb66f819ea06dbad3715e9431`  
		Last Modified: Wed, 14 Oct 2020 18:30:50 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2abbe75cd492fbd42e73733a282a661cb8caf898389b66479838c9d6a12bf93`  
		Last Modified: Wed, 14 Oct 2020 18:30:53 GMT  
		Size: 5.4 MB (5376495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54c94d9d841e9ad09db4d956de957ddc529f82eb7a317a766e7ccec444303329`  
		Last Modified: Fri, 16 Oct 2020 20:30:29 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:739c111999a323e4bdffbaa9802f8775e70d4ae591fc8ca9af5a9550ecfc59d5`  
		Last Modified: Fri, 16 Oct 2020 20:30:29 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39974e2f48514b6f43a54533790da257d1adbcd778d60863b5e8e350f235e07b`  
		Last Modified: Fri, 16 Oct 2020 20:30:29 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d86232e798a7811f236ba6513dd76e71294628cd24b0847874f6fe61abf2ff5c`  
		Last Modified: Fri, 16 Oct 2020 20:30:52 GMT  
		Size: 202.2 MB (202206871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:217d44a61755c479180692094518709c4394300501adbd837c9c45091ec33b1b`  
		Last Modified: Fri, 16 Oct 2020 20:30:29 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
