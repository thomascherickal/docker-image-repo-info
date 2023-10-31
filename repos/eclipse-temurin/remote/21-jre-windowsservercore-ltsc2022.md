## `eclipse-temurin:21-jre-windowsservercore-ltsc2022`

```console
$ docker pull eclipse-temurin@sha256:7af3a1a579648c896bdd17f5e3678c9c65f96c5a03e1e72464a1b5edcdcbacbb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.2031; amd64

### `eclipse-temurin:21-jre-windowsservercore-ltsc2022` - windows version 10.0.20348.2031; amd64

```console
$ docker pull eclipse-temurin@sha256:4cddbf7eefba5f659cb1cb1bd139b175df282e4c217b27fb4cee842abc313f59
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 GB (1943532788 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:44e561a81cb9cc95b815a88e313cba161fee81a7fb1ec3cbcdbb231de147a2bc`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:55:20 GMT
RUN Apply image 10.0.20348.1787
# Fri, 06 Oct 2023 21:59:31 GMT
RUN Install update 10.0.20348.2031
# Wed, 11 Oct 2023 01:35:10 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 30 Oct 2023 23:33:00 GMT
ENV JAVA_VERSION=jdk-21.0.1+12
# Mon, 30 Oct 2023 23:38:26 GMT
RUN Write-Host ('Downloading https://github.com/adoptium/temurin21-binaries/releases/download/jdk-21.0.1%2B12/OpenJDK21U-jre_x64_windows_hotspot_21.0.1_12.msi ...');     curl.exe -LfsSo openjdk.msi https://github.com/adoptium/temurin21-binaries/releases/download/jdk-21.0.1%2B12/OpenJDK21U-jre_x64_windows_hotspot_21.0.1_12.msi ;     Write-Host ('Verifying sha256 (9bb4db6e70e105e77a2f395ab925d6413ccd2a97d81fe7eab67cfdc373cfbe9e) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne '9bb4db6e70e105e77a2f395ab925d6413ccd2a97d81fe7eab67cfdc373cfbe9e') {         Write-Host 'FAILED!';         exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     $proc = Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome', 'INSTALLDIR=C:\openjdk-21' -Wait -Passthru;     $proc.WaitForExit() ;     if ($proc.ExitCode -ne 0) {         Write-Host 'FAILED installing MSI!' ;         exit 1;     };         Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Mon, 30 Oct 2023 23:38:44 GMT
RUN Write-Host 'Verifying install ...';     Write-Host 'java --version'; java --version;         Write-Host 'Complete.'
```

-	Layers:
	-	`sha256:7c76e5cf7755ce357ffb737715b0da6799a50ea468cc252c094f4d915d426b3f`  
		Last Modified: Tue, 13 Jun 2023 17:55:32 GMT  
		Size: 1.4 GB (1388598786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3d2471a50c8ec3ea61c16dd871f7b9167bf779faad2b6e5a6f72a18b88b846b`  
		Last Modified: Tue, 10 Oct 2023 17:55:23 GMT  
		Size: 471.2 MB (471244358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a73b90f34f44bbbb354af4f3d4cc6cde597d2f5183641e139f7ca8b76ec3bb9`  
		Last Modified: Wed, 11 Oct 2023 02:45:06 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb2342cad8ad6a05bce2e29d23b6ae040b453d90db04b167e1041acd26752953`  
		Last Modified: Mon, 30 Oct 2023 23:52:51 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3c1e7e7823a5183cc6bd844107585d387f72afa39afb3a62a425b364e8cb75f`  
		Last Modified: Mon, 30 Oct 2023 23:54:53 GMT  
		Size: 83.4 MB (83397365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d91369a4172c90e971c1ea558bbd9a049afcc35b66bacc39780b2c4ea0a438a3`  
		Last Modified: Mon, 30 Oct 2023 23:54:42 GMT  
		Size: 289.5 KB (289545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
