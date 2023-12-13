## `eclipse-temurin:11-jre-windowsservercore-ltsc2022`

```console
$ docker pull eclipse-temurin@sha256:fe3c38c69b5986d3e9250a17bfe1a4cd0fbcda15f061f3b644485aea8187f9cb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.2159; amd64

### `eclipse-temurin:11-jre-windowsservercore-ltsc2022` - windows version 10.0.20348.2159; amd64

```console
$ docker pull eclipse-temurin@sha256:495d7bcc60187babf0a80aa9c8ec2c3309db247ac98073d33e4d357e28356dca
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (1964283762 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:37ef28dd503887f016e612d61860e771a1638ab818bea4fce7f594e8c0a7953f`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:55:20 GMT
RUN Apply image 10.0.20348.1787
# Sat, 02 Dec 2023 12:42:56 GMT
RUN Install update 10.0.20348.2159
# Tue, 12 Dec 2023 23:35:07 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Dec 2023 00:19:32 GMT
ENV JAVA_VERSION=jdk-11.0.21+9
# Wed, 13 Dec 2023 00:25:37 GMT
RUN Write-Host ('Downloading https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_x64_windows_hotspot_11.0.21_9.msi ...');     curl.exe -LfsSo openjdk.msi https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_x64_windows_hotspot_11.0.21_9.msi ;     Write-Host ('Verifying sha256 (9b0ea6ebe77e70c7ac229074028d64399d72a7fda499aad114ef0ba4c375b1a8) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne '9b0ea6ebe77e70c7ac229074028d64399d72a7fda499aad114ef0ba4c375b1a8') {         Write-Host 'FAILED!';         exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     $proc = Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome', 'INSTALLDIR=C:\openjdk-11' -Wait -Passthru;     $proc.WaitForExit() ;     if ($proc.ExitCode -ne 0) {         Write-Host 'FAILED installing MSI!' ;         exit 1;     };         Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Wed, 13 Dec 2023 00:26:00 GMT
RUN Write-Host 'Verifying install ...';     Write-Host 'java --version'; java --version;         Write-Host 'Complete.'
```

-	Layers:
	-	`sha256:7c76e5cf7755ce357ffb737715b0da6799a50ea468cc252c094f4d915d426b3f`  
		Last Modified: Tue, 13 Jun 2023 17:55:32 GMT  
		Size: 1.4 GB (1388598786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7839fc47f6e056f9e09a214230f8b7115e69419dbc74acbbb1ad6bc0caa28862`  
		Last Modified: Tue, 12 Dec 2023 18:27:40 GMT  
		Size: 500.7 MB (500674814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95d0c853ded9068434b9128a8016b3ae5e18f748f62801c7bb6e6092495300ec`  
		Last Modified: Wed, 13 Dec 2023 00:02:39 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:455780d2f42600efb2a3a20116e117f6d5c0f47e123f17be7a83db9c2c69bf42`  
		Last Modified: Wed, 13 Dec 2023 06:36:14 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ee464e22d5ff8101fae6692bb893de984398a1490dbde4e7c7cdec5b3c8201c`  
		Last Modified: Wed, 13 Dec 2023 06:38:07 GMT  
		Size: 74.7 MB (74714733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4420b81b25f5ba0806ff655a91fbce307ee4219b373a2e7aeed0c793ab5061e3`  
		Last Modified: Wed, 13 Dec 2023 06:37:57 GMT  
		Size: 292.7 KB (292716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
