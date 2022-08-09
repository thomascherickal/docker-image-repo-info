## `openjdk:19-ea-jdk`

```console
$ docker pull openjdk@sha256:e1aa6f330486eccf4163a54ac430fd90eac81119bbd824b3b0a4918424adc50f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	windows version 10.0.20348.825; amd64
	-	windows version 10.0.17763.3165; amd64

### `openjdk:19-ea-jdk` - linux; amd64

```console
$ docker pull openjdk@sha256:177859802a9de531de78542029f8a759843db086edba9fee4e6467f03a8220a4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **248.9 MB (248901718 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9379295221fe6205e1be76e1212423aef85b4a4e90846c253d0a11d7dd8a709c`
-	Default Command: `["jshell"]`

```dockerfile
# Thu, 04 Aug 2022 00:36:37 GMT
ADD file:0a05a213ae66f556b2b320291ac58ec9f2f67554e29338a072f1347f22864a49 in / 
# Thu, 04 Aug 2022 00:36:37 GMT
CMD ["/bin/bash"]
# Thu, 04 Aug 2022 01:35:27 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Thu, 04 Aug 2022 01:35:57 GMT
ENV JAVA_HOME=/usr/java/openjdk-19
# Thu, 04 Aug 2022 01:35:57 GMT
ENV PATH=/usr/java/openjdk-19/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 04 Aug 2022 01:35:57 GMT
ENV LANG=C.UTF-8
# Mon, 08 Aug 2022 22:52:59 GMT
ENV JAVA_VERSION=19-ea+34
# Mon, 08 Aug 2022 22:53:11 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk19/34/GPL/openjdk-19-ea+34_linux-x64_bin.tar.gz'; 			downloadSha256='719889f7aaf988e7ec5c6edd0c3bd03342294f329a36dd6591af2e64f6aefae7'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk19/34/GPL/openjdk-19-ea+34_linux-aarch64_bin.tar.gz'; 			downloadSha256='8d5d5327b1a7d35ae2c16ba69701cb58cb5b5df58f5ace295c08fe77d96a688b'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Mon, 08 Aug 2022 22:53:12 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:32c1bf40aba1f372a057d3280b0b7cdacde9d8500a069004e6f243bc09cde806`  
		Last Modified: Thu, 04 Aug 2022 00:37:33 GMT  
		Size: 39.2 MB (39223952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d72ac1fb23a36f89addf60367990f28d5c0882e4b8f569c77b51c51eb271261`  
		Last Modified: Thu, 04 Aug 2022 01:42:41 GMT  
		Size: 13.5 MB (13506500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:759b12086838c0cadc93bbe08dd3f35cd6565cb1307dbc34b28e7c6fe6bb9b46`  
		Last Modified: Mon, 08 Aug 2022 23:04:09 GMT  
		Size: 196.2 MB (196171266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:19-ea-jdk` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:87b8ff3d086260cf3ed9ddcd0b549a351056553e2a84187d734a7476089fef53
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **247.3 MB (247334316 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:06b288690c01e858cdbcfe18357258664c8fa1803ed1d90f9e444111d7154800`
-	Default Command: `["jshell"]`

```dockerfile
# Thu, 04 Aug 2022 00:40:43 GMT
ADD file:a68d82fa032efe6adc2926f7e745508f0541bba3f906e2702d34252353100747 in / 
# Thu, 04 Aug 2022 00:40:44 GMT
CMD ["/bin/bash"]
# Thu, 04 Aug 2022 01:01:11 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Thu, 04 Aug 2022 01:02:12 GMT
ENV JAVA_HOME=/usr/java/openjdk-19
# Thu, 04 Aug 2022 01:02:12 GMT
ENV PATH=/usr/java/openjdk-19/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 04 Aug 2022 01:02:13 GMT
ENV LANG=C.UTF-8
# Mon, 08 Aug 2022 23:32:16 GMT
ENV JAVA_VERSION=19-ea+34
# Mon, 08 Aug 2022 23:32:38 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk19/34/GPL/openjdk-19-ea+34_linux-x64_bin.tar.gz'; 			downloadSha256='719889f7aaf988e7ec5c6edd0c3bd03342294f329a36dd6591af2e64f6aefae7'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk19/34/GPL/openjdk-19-ea+34_linux-aarch64_bin.tar.gz'; 			downloadSha256='8d5d5327b1a7d35ae2c16ba69701cb58cb5b5df58f5ace295c08fe77d96a688b'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Mon, 08 Aug 2022 23:32:38 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:ecf56004177eb6ca162c88de29e84bc4ba3d2e7efd3703df9ecae51b89003d52`  
		Last Modified: Thu, 04 Aug 2022 00:41:51 GMT  
		Size: 38.0 MB (38023046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e225b6ab834ff85ee0d347a2859ecb14fc169f362360408133589ab8a37d8333`  
		Last Modified: Thu, 04 Aug 2022 01:14:59 GMT  
		Size: 14.3 MB (14278746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d6108e1a6eeb1984a19a306b3f37c0b9676fcfadb5ec712c6b45726cba6a851`  
		Last Modified: Mon, 08 Aug 2022 23:50:26 GMT  
		Size: 195.0 MB (195032524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:19-ea-jdk` - windows version 10.0.20348.825; amd64

```console
$ docker pull openjdk@sha256:82e1dc36405951a160a71048bc909111c765283c8ee477695926b08d783ae9d9
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2493211274 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b58446534e09bda79cb63c0c8403ed519888973881496187f1e3fd0a2afefb0a`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Mon, 04 Jul 2022 17:46:55 GMT
RUN Install update 10.0.20348.825
# Tue, 12 Jul 2022 19:25:40 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Jul 2022 15:47:47 GMT
RUN Write-Host 'Enabling TLS 1.2 (https://githubengineering.com/crypto-removal-notice/) ...'; 	$tls12RegBase = 'HKLM:\\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2'; 	if (Test-Path $tls12RegBase) { throw ('"{0}" already exists!' -f $tls12RegBase) }; 	New-Item -Path ('{0}/Client' -f $tls12RegBase) -Force; 	New-Item -Path ('{0}/Server' -f $tls12RegBase) -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	Write-Host 'Complete.'
# Wed, 13 Jul 2022 15:53:28 GMT
ENV JAVA_HOME=C:\openjdk-19
# Wed, 13 Jul 2022 15:53:49 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath; 	Write-Host 'Complete.'
# Mon, 08 Aug 2022 22:19:25 GMT
ENV JAVA_VERSION=19-ea+34
# Mon, 08 Aug 2022 22:19:26 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk19/34/GPL/openjdk-19-ea+34_windows-x64_bin.zip
# Mon, 08 Aug 2022 22:19:27 GMT
ENV JAVA_SHA256=5d3ac1a89d92a142588bc8546aa737c37d1971bcff17810b5ff947790c97e623
# Mon, 08 Aug 2022 22:20:17 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Mon, 08 Aug 2022 22:20:18 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:97f65a0ec59e643faf84024aa713a9be059322380315fda829756bbbd96d6258`  
		Size: 1.4 GB (1436863614 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e1a27cb9d4615dec325f2cbabac4ca1f65413bdbb8b440cc961df032993a9b81`  
		Size: 863.4 MB (863367943 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:6452cb934201756f0ed9fb5e0cbea54a22a66412cb696ff30a1923d456e28bcf`  
		Last Modified: Tue, 12 Jul 2022 20:20:48 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f6a9bb0f902c90ab99dd7b3c8634f73649b052868aa5272230088be93b0be1f`  
		Last Modified: Mon, 18 Jul 2022 21:21:07 GMT  
		Size: 655.6 KB (655645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcd66eccfd01aee1696d4c33d4a0c1b49827e90518a13fde80169d46f2171f64`  
		Last Modified: Mon, 18 Jul 2022 21:23:16 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92a625d17ec9ae423e7fd6a2cd3d934b06c1a4872336d21f5021622a34e145e1`  
		Last Modified: Mon, 18 Jul 2022 21:23:16 GMT  
		Size: 555.8 KB (555849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e20d23943d06d6d4f96030c8fe307945b2f5db29324dfc902da964cc246c2e0e`  
		Last Modified: Mon, 08 Aug 2022 22:29:36 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0199c6c6a75f80abd2fbb88c1037f27ccf27afa52c9fec98210f7bf60d6c61f2`  
		Last Modified: Mon, 08 Aug 2022 22:29:36 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65403d2317db231b4346a7a45cdd0b63016600803091ea88725482dfc0ea43cf`  
		Last Modified: Mon, 08 Aug 2022 22:29:37 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a8e0fa98d211abc3bf5065058d0809e9c94bbe528764beec74619efdd03f70c`  
		Last Modified: Mon, 08 Aug 2022 22:29:57 GMT  
		Size: 191.8 MB (191759761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:435e3fb327d8e2523699088ca0eeb5d38585bab28f3b2a798bfa19863abada80`  
		Last Modified: Mon, 08 Aug 2022 22:29:36 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:19-ea-jdk` - windows version 10.0.17763.3165; amd64

```console
$ docker pull openjdk@sha256:73d9b156343f2c4adafbc2f58f49bc454bc8cbaf7f4b3c1e36e4fe0432dd4a5c
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 GB (2864273313 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a3cf72be7f0a7917c3d1fcb57599ca7a34a4b9bf3b25eea4081b2df416043f9`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Wed, 06 Jul 2022 22:37:15 GMT
RUN Install update 10.0.17763.3165
# Tue, 12 Jul 2022 19:32:43 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Jul 2022 15:50:04 GMT
RUN Write-Host 'Enabling TLS 1.2 (https://githubengineering.com/crypto-removal-notice/) ...'; 	$tls12RegBase = 'HKLM:\\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2'; 	if (Test-Path $tls12RegBase) { throw ('"{0}" already exists!' -f $tls12RegBase) }; 	New-Item -Path ('{0}/Client' -f $tls12RegBase) -Force; 	New-Item -Path ('{0}/Server' -f $tls12RegBase) -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	Write-Host 'Complete.'
# Wed, 13 Jul 2022 15:55:10 GMT
ENV JAVA_HOME=C:\openjdk-19
# Wed, 13 Jul 2022 15:56:04 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath; 	Write-Host 'Complete.'
# Mon, 08 Aug 2022 22:20:28 GMT
ENV JAVA_VERSION=19-ea+34
# Mon, 08 Aug 2022 22:20:29 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk19/34/GPL/openjdk-19-ea+34_windows-x64_bin.zip
# Mon, 08 Aug 2022 22:20:30 GMT
ENV JAVA_SHA256=5d3ac1a89d92a142588bc8546aa737c37d1971bcff17810b5ff947790c97e623
# Mon, 08 Aug 2022 22:21:56 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Mon, 08 Aug 2022 22:21:57 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7aca8de30754f19fe03ee4c21eed0762efb5e91bf684b0cc36cc92b2af13446d`  
		Size: 794.9 MB (794877652 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:912efe6370f7047e630e1f70d9201e3143571e3ed1fe50a1e61754d2d536ea95`  
		Last Modified: Tue, 12 Jul 2022 20:21:55 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6acf5949ddc551d281d19646d7dbeb4f3772073cf86c194f6d98c8afe422f3b5`  
		Last Modified: Mon, 18 Jul 2022 21:21:50 GMT  
		Size: 353.5 KB (353532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0ef755dcec989c5860b62157e6a71a3161b651df08ebc5d41a441c82db2bda3`  
		Last Modified: Mon, 18 Jul 2022 21:23:59 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0be3865968b6d273d0d991753302d14841ef7355875ec01f046c8f653d019223`  
		Last Modified: Mon, 18 Jul 2022 21:23:59 GMT  
		Size: 311.7 KB (311730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ada3e77ee115d05d9a9899adedac83218670e2975f4f7f84e328cfc9f8b4c622`  
		Last Modified: Mon, 08 Aug 2022 22:30:18 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f2f0ce27c6e3be4355cd0ba7da5234dadcfa3b950d8d7128e1066102cf18714`  
		Last Modified: Mon, 08 Aug 2022 22:30:18 GMT  
		Size: 1.4 KB (1445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20e956b3127157cf40c5e0e9e65697d20701f0de8f7f78a9357499077a605503`  
		Last Modified: Mon, 08 Aug 2022 22:30:18 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3567d27f19e2c439737bfc0987e27b26934646f84f746995db345a95988f5f4f`  
		Last Modified: Mon, 08 Aug 2022 22:30:38 GMT  
		Size: 191.6 MB (191555768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cbce2153197de2622aca1bcc9eff846120d07cd5d2015c0e4e5a227135f69d2`  
		Last Modified: Mon, 08 Aug 2022 22:30:18 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
