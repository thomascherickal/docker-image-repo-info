## `adoptopenjdk:11-jre-hotspot-windowsservercore-1809`

```console
$ docker pull adoptopenjdk@sha256:9fd67bca92dc6e41a6e5e061614b4ac4b68b834e7fc8d6cfb8c67d9148f64a48
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2061; amd64

### `adoptopenjdk:11-jre-hotspot-windowsservercore-1809` - windows version 10.0.17763.2061; amd64

```console
$ docker pull adoptopenjdk@sha256:81b50136060b3efc617e7ede71552ddf32e2e97f220b472eac5375842bc22369
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2758649506 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a8cfb984e3598f562d953cc05d3deaf0f6c4ac602a2947f93836e1530f91ddd1`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 06 Jul 2021 20:34:18 GMT
RUN Install update 1809-amd64
# Wed, 14 Jul 2021 02:41:59 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Jul 2021 15:33:20 GMT
ENV JAVA_VERSION=jdk-11.0.11+9
# Wed, 14 Jul 2021 15:39:33 GMT
RUN Write-Host ('Downloading https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.11%2B9/OpenJDK11U-jre_x64_windows_hotspot_11.0.11_9.msi ...');     curl.exe -LfsSo openjdk.msi https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.11%2B9/OpenJDK11U-jre_x64_windows_hotspot_11.0.11_9.msi ;     Write-Host ('Verifying sha256 (d52262a1ac6d86326cd071b687dcc5bb546bedda6d03c6bd26a046070a013df3) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne 'd52262a1ac6d86326cd071b687dcc5bb546bedda6d03c6bd26a046070a013df3') {             Write-Host 'FAILED!';             exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     $proc = Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome' -Wait -Passthru;     $proc.WaitForExit() ;     if ($proc.ExitCode -ne 0) {             Write-Host 'FAILED installing MSI!' ;             exit 1;     };         Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f143c6fed32d477c35b660b2e108ea62e3593c03e44bd9ced208ce52b26b0841`  
		Size: 967.1 MB (967113907 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:dd3b24b55401566ea01a5005138a23766b6b6408c2276b7ebd097da01de80897`  
		Last Modified: Wed, 14 Jul 2021 03:38:04 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f047fbbd8b17018ca409212e52b95f4daaa10861fcfc86be53d143948858be80`  
		Last Modified: Wed, 14 Jul 2021 16:44:10 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ace0497d67851a574e914c709c417f69ed1c9cbe8e160eb7e64147ae847a5616`  
		Last Modified: Wed, 14 Jul 2021 16:52:39 GMT  
		Size: 73.2 MB (73199866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
