## `openjdk:20-ea-2-jdk`

```console
$ docker pull openjdk@sha256:b4d1d0d1adcdff135f844b09d03c55669b5f4085e3ccca53acc1fb60a1ad9d0a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	windows version 10.0.20348.768; amd64
	-	windows version 10.0.17763.3046; amd64

### `openjdk:20-ea-2-jdk` - linux; amd64

```console
$ docker pull openjdk@sha256:44ea48e5c2b6757cf7e34d8ff09724ca7ecf5c31e1d554953692431ee3c868a4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **249.9 MB (249870311 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ada797b06bdc879d5500cf9996d4aa84feacbcfa2deb8d6a937a50678cd4a0e8`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 14 Jun 2022 18:23:26 GMT
ADD file:837f6c6e7e20067b92edb72e78a8399e6cbbd72dab23db7b5b5a301c58d2a0de in / 
# Tue, 14 Jun 2022 18:23:26 GMT
CMD ["/bin/bash"]
# Tue, 14 Jun 2022 18:42:55 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Thu, 16 Jun 2022 01:21:37 GMT
ENV JAVA_HOME=/usr/java/openjdk-20
# Thu, 16 Jun 2022 01:21:37 GMT
ENV PATH=/usr/java/openjdk-20/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 16 Jun 2022 01:21:37 GMT
ENV LANG=C.UTF-8
# Wed, 22 Jun 2022 01:19:43 GMT
ENV JAVA_VERSION=20-ea+2
# Wed, 22 Jun 2022 01:20:10 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/2/GPL/openjdk-20-ea+2_linux-x64_bin.tar.gz'; 			downloadSha256='21ff68a0fba20bd62c33f66b6215e4dbb6a4ccc40ee4c63aefd5a69ded443812'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/2/GPL/openjdk-20-ea+2_linux-aarch64_bin.tar.gz'; 			downloadSha256='23ec06e04606ac8ccd9f304bc06527f78c6a196b796b8b7581de2153a3097bff'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 22 Jun 2022 01:20:11 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:5f160c0f6cac587a73883b48a8857f5cce0930112792cef25c62510e256e93dc`  
		Last Modified: Tue, 14 Jun 2022 18:24:18 GMT  
		Size: 39.2 MB (39219730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb499df0377a2bd9163e9a611ce46b5379196826787392defef98dbf215a8aa4`  
		Last Modified: Tue, 14 Jun 2022 18:49:29 GMT  
		Size: 13.5 MB (13502563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8806eb980f4a525fff5a8ba2d3703410d26bf8a51d5bdebe61d3fe728323c450`  
		Last Modified: Wed, 22 Jun 2022 01:29:35 GMT  
		Size: 197.1 MB (197148018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:20-ea-2-jdk` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:4f79ebf57992e09bd68066a7117b654699297dd859bc600ce52f4ef2d4d24a36
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **248.3 MB (248260798 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:24d354c48b727e293a39885f556e517d5748c337682e3324142ded8d15941b8c`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 14 Jun 2022 18:41:36 GMT
ADD file:4a6ee90ad73353bfb87b2f121e06bddaed6104536e485baa83fadbe7facc774c in / 
# Tue, 14 Jun 2022 18:41:37 GMT
CMD ["/bin/bash"]
# Tue, 14 Jun 2022 18:58:47 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Thu, 16 Jun 2022 00:49:01 GMT
ENV JAVA_HOME=/usr/java/openjdk-20
# Thu, 16 Jun 2022 00:49:02 GMT
ENV PATH=/usr/java/openjdk-20/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 16 Jun 2022 00:49:03 GMT
ENV LANG=C.UTF-8
# Wed, 22 Jun 2022 02:12:55 GMT
ENV JAVA_VERSION=20-ea+2
# Wed, 22 Jun 2022 02:13:09 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/2/GPL/openjdk-20-ea+2_linux-x64_bin.tar.gz'; 			downloadSha256='21ff68a0fba20bd62c33f66b6215e4dbb6a4ccc40ee4c63aefd5a69ded443812'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/2/GPL/openjdk-20-ea+2_linux-aarch64_bin.tar.gz'; 			downloadSha256='23ec06e04606ac8ccd9f304bc06527f78c6a196b796b8b7581de2153a3097bff'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 22 Jun 2022 02:13:09 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:2bbc1bf883bd601c0da5735b538963308bcc17f90d36525ecc93456ffad79064`  
		Last Modified: Tue, 14 Jun 2022 18:42:39 GMT  
		Size: 38.0 MB (38012371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bde7855ef536fce06527372a019087e1972db9d092b2ec88091b6017cfc5a16`  
		Last Modified: Tue, 14 Jun 2022 19:10:59 GMT  
		Size: 14.3 MB (14260872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:975e3aa3f26f08acd1baf2a2870b6e14ea24bf656c3aab2e88c29e15dc756be3`  
		Last Modified: Wed, 22 Jun 2022 02:29:23 GMT  
		Size: 196.0 MB (195987555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:20-ea-2-jdk` - windows version 10.0.20348.768; amd64

```console
$ docker pull openjdk@sha256:8fc38cd3880bcb448cb8f2b2b24ef533797727b80d0c02b0c72de8495625002f
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2472447604 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7adbb28b1e51f4b7e7cb19a56ae454cc670c788b7e146461dbe154ea3536ae71`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Thu, 09 Jun 2022 04:32:50 GMT
RUN Install update 10.0.20348.768
# Wed, 15 Jun 2022 12:13:32 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Jun 2022 19:30:14 GMT
RUN Write-Host 'Enabling TLS 1.2 (https://githubengineering.com/crypto-removal-notice/) ...'; 	$tls12RegBase = 'HKLM:\\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2'; 	if (Test-Path $tls12RegBase) { throw ('"{0}" already exists!' -f $tls12RegBase) }; 	New-Item -Path ('{0}/Client' -f $tls12RegBase) -Force; 	New-Item -Path ('{0}/Server' -f $tls12RegBase) -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	Write-Host 'Complete.'
# Thu, 16 Jun 2022 01:14:39 GMT
ENV JAVA_HOME=C:\openjdk-20
# Thu, 16 Jun 2022 01:15:08 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath; 	Write-Host 'Complete.'
# Wed, 22 Jun 2022 00:43:45 GMT
ENV JAVA_VERSION=20-ea+2
# Wed, 22 Jun 2022 00:43:46 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk20/2/GPL/openjdk-20-ea+2_windows-x64_bin.zip
# Wed, 22 Jun 2022 00:43:47 GMT
ENV JAVA_SHA256=8dc5a274cd002d32ae4c8f6561afb4b620763ac5c05a3fdf77ea1b5ad58fbe3a
# Wed, 22 Jun 2022 00:44:44 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Wed, 22 Jun 2022 00:44:45 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:97f65a0ec59e643faf84024aa713a9be059322380315fda829756bbbd96d6258`  
		Size: 1.4 GB (1436863614 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:6c71967ff41928927e4c407171e4ffbac3c9ab4221eb64f5ca5a34ff4c230567`  
		Size: 841.6 MB (841600427 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:dec0338feaf01f35eb916b7fd9ecc08b719354163254885d5215e513c1a3eb2e`  
		Last Modified: Wed, 15 Jun 2022 12:49:26 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8b6e059d50cccbff94037bf242f1b94acf1cc939d701dff58c07f4fcfdc9767`  
		Last Modified: Wed, 15 Jun 2022 20:02:04 GMT  
		Size: 632.3 KB (632288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5e4ff554b66055922423d154f7282c8144066ebe31d1393200cf475fb56555f`  
		Last Modified: Thu, 16 Jun 2022 01:26:02 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a207dedd7fa079f899254dd9a6ea4b20cbb4e77f9880ed19716901e210c1e42f`  
		Last Modified: Thu, 16 Jun 2022 01:26:02 GMT  
		Size: 564.2 KB (564202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b410becae28da98cf3dfbe89961fdce7d06d4e812eb2754adbf8ac5090962fe1`  
		Last Modified: Wed, 22 Jun 2022 02:21:01 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f56547dc781f34bf6b9287fffa681df757f3b6e937f2811c39b7a99f2e316ed`  
		Last Modified: Wed, 22 Jun 2022 02:21:01 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c7f521e26920b4cbbee7d688f2af6d24a6b12287fd13729549d71844d181902`  
		Last Modified: Wed, 22 Jun 2022 02:21:01 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c59fc63ab696ebb1e274427cc28de05c3092d1c87f39ef3613b9f7a61c2d2c42`  
		Last Modified: Wed, 22 Jun 2022 02:24:31 GMT  
		Size: 192.8 MB (192778565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67f31263e29428da3a257cdae2ba85cf98403b88c97552bc06ed1aab791d2b0a`  
		Last Modified: Wed, 22 Jun 2022 02:21:01 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:20-ea-2-jdk` - windows version 10.0.17763.3046; amd64

```console
$ docker pull openjdk@sha256:31ef4b0e5e2d74692190368bfde0bd3481d2c228e81d7a66a6887cacf547071c
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 GB (2856495708 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:225dd3ba6e1bdd06ee63bd0a67763c99bfdea6dbe678e5809ea43d6731a9c609`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Thu, 09 Jun 2022 19:41:03 GMT
RUN Install update 10.0.17763.3046
# Wed, 15 Jun 2022 12:18:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Jun 2022 19:33:08 GMT
RUN Write-Host 'Enabling TLS 1.2 (https://githubengineering.com/crypto-removal-notice/) ...'; 	$tls12RegBase = 'HKLM:\\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2'; 	if (Test-Path $tls12RegBase) { throw ('"{0}" already exists!' -f $tls12RegBase) }; 	New-Item -Path ('{0}/Client' -f $tls12RegBase) -Force; 	New-Item -Path ('{0}/Server' -f $tls12RegBase) -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	Write-Host 'Complete.'
# Thu, 16 Jun 2022 01:16:22 GMT
ENV JAVA_HOME=C:\openjdk-20
# Thu, 16 Jun 2022 01:17:35 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath; 	Write-Host 'Complete.'
# Wed, 22 Jun 2022 00:45:03 GMT
ENV JAVA_VERSION=20-ea+2
# Wed, 22 Jun 2022 00:45:04 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk20/2/GPL/openjdk-20-ea+2_windows-x64_bin.zip
# Wed, 22 Jun 2022 00:45:05 GMT
ENV JAVA_SHA256=8dc5a274cd002d32ae4c8f6561afb4b620763ac5c05a3fdf77ea1b5ad58fbe3a
# Wed, 22 Jun 2022 00:46:52 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Wed, 22 Jun 2022 00:46:53 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:fc6ae6c5aa2b4920ae68469c5e7e7c3a3c85e5eaafc24660e7b3adb21d6fce77`  
		Size: 786.1 MB (786113785 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4ed911f97ae3a2a6279c70738e5692b14369ac11871a2bbd2f6ad301419527ad`  
		Last Modified: Wed, 15 Jun 2022 12:50:13 GMT  
		Size: 1.3 KB (1314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75415e053743ebceabbf30d0a8101d97dd712c88fc012c45f1df824cbac48e21`  
		Last Modified: Wed, 15 Jun 2022 20:05:58 GMT  
		Size: 354.4 KB (354400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52024d1a50366ffd4635321735cd38ce0ecab43a1ba938284d4286b6020140ef`  
		Last Modified: Thu, 16 Jun 2022 01:29:40 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4732abfe811150ac2b9a2ccb0f838bf2f402b7f56952056d2f28ba681fc8b120`  
		Last Modified: Thu, 16 Jun 2022 01:29:40 GMT  
		Size: 312.4 KB (312396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b424ef6bf361dc694b75aafe2f3eaa695fa11e4fba0bbdf2b941b7483a11bab`  
		Last Modified: Wed, 22 Jun 2022 02:24:52 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2ede2556a664b15c0cef8a75604b73e8fb578b36f61b3fb43da1642ce98202c`  
		Last Modified: Wed, 22 Jun 2022 02:24:51 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af19c85b4f898b8502a48295502da644610bdf94283ffbde478b4f01e6771c5a`  
		Last Modified: Wed, 22 Jun 2022 02:24:52 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f921f8c87da9c5303348563fd479c99fa87f45c9be9ea5e40ee4f86e977f66b`  
		Last Modified: Wed, 22 Jun 2022 02:28:24 GMT  
		Size: 192.5 MB (192540612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e58c00fc9ecebbd50398b5268ff465ec4f068bd8cd40d99733b2cdd81e8e832`  
		Last Modified: Wed, 22 Jun 2022 02:24:52 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
