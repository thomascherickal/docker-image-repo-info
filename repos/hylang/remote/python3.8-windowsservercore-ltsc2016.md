## `hylang:python3.8-windowsservercore-ltsc2016`

```console
$ docker pull hylang@sha256:946f74c6352ac8ff840fbea720043093f03ccce0209720572a1c0bc54a019d08
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3930; amd64

### `hylang:python3.8-windowsservercore-ltsc2016` - windows version 10.0.14393.3930; amd64

```console
$ docker pull hylang@sha256:388d86bd8729a118e5c5522139ba0944e7e3bdd94fb3204c918a0e7e7999c75d
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5823261528 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bae1f6d994706c49c3fcac2714a24c30b44493b4e14df7f397cc524f19769be1`
-	Default Command: `["hy"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 01 Sep 2020 19:14:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 08 Sep 2020 19:31:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 08 Sep 2020 19:39:28 GMT
ENV PYTHON_VERSION=3.8.5
# Tue, 08 Sep 2020 19:39:28 GMT
ENV PYTHON_RELEASE=3.8.5
# Tue, 08 Sep 2020 19:41:47 GMT
RUN $url = ('https://www.python.org/ftp/python/{0}/python-{1}-amd64.exe' -f $env:PYTHON_RELEASE, $env:PYTHON_VERSION); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'python.exe'; 		Write-Host 'Installing ...'; 	Start-Process python.exe -Wait 		-ArgumentList @( 			'/quiet', 			'InstallAllUsers=1', 			'TargetDir=C:\Python', 			'PrependPath=1', 			'Shortcuts=0', 			'Include_doc=0', 			'Include_pip=0', 			'Include_test=0' 		); 		$env:PATH = [Environment]::GetEnvironmentVariable('PATH', [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  python --version'; python --version; 		Write-Host 'Removing ...'; 	Remove-Item python.exe -Force; 		Write-Host 'Complete.'
# Tue, 08 Sep 2020 19:41:48 GMT
ENV PYTHON_PIP_VERSION=20.2.3
# Tue, 08 Sep 2020 19:41:49 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/fa7dc83944936bf09a0e4cb5d5ec852c0d256599/get-pip.py
# Tue, 08 Sep 2020 19:41:51 GMT
ENV PYTHON_GET_PIP_SHA256=6e0bb0a2c2533361d7f297ed547237caf1b7507f197835974c0dd7eba998c53c
# Tue, 08 Sep 2020 19:43:34 GMT
RUN Write-Host ('Downloading get-pip.py ({0}) ...' -f $env:PYTHON_GET_PIP_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:PYTHON_GET_PIP_URL -OutFile 'get-pip.py'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:PYTHON_GET_PIP_SHA256); 	if ((Get-FileHash 'get-pip.py' -Algorithm sha256).Hash -ne $env:PYTHON_GET_PIP_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host ('Installing pip=={0} ...' -f $env:PYTHON_PIP_VERSION); 	python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		('pip=={0}' -f $env:PYTHON_PIP_VERSION) 	; 	Remove-Item get-pip.py -Force; 		Write-Host 'Verifying pip install ...'; 	pip --version; 		Write-Host 'Complete.'
# Tue, 08 Sep 2020 19:43:36 GMT
CMD ["python"]
# Tue, 08 Sep 2020 22:48:52 GMT
ENV HY_VERSION=0.19.0
# Tue, 08 Sep 2020 22:50:35 GMT
RUN pip install --no-cache-dir ('hy == {0}' -f $env:HY_VERSION)
# Tue, 08 Sep 2020 22:50:36 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bc202b498d589027cc702b23cf959b8842907508b3465b9d6ff739c9668e5134`  
		Size: 1.7 GB (1669268544 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8f6f82df7cca9113965bd35d2921a651250266aa7a3a9df6a0a42e8c005f1333`  
		Last Modified: Tue, 08 Sep 2020 19:53:55 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:947813843d7199c45a80ff835022a92bc3559da91cf0ad427ce0554383b1e11a`  
		Last Modified: Tue, 08 Sep 2020 19:54:42 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:748e02a7b127f58784c54f322d8dc67af0f91bc24cd338a23a53b14422d5d0cb`  
		Last Modified: Tue, 08 Sep 2020 19:54:42 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66a3f62f40c259d5ff8e8451c46b65829a0f5b5e3a913a18fe8a96a8aa6d3241`  
		Last Modified: Tue, 08 Sep 2020 19:54:52 GMT  
		Size: 57.9 MB (57901053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2a356c0ef5cff755b2126bce586bef9b4108859432657d00b7396151e22f58a`  
		Last Modified: Tue, 08 Sep 2020 19:54:40 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2fcddb2e03bf31e2b734743cd75a91357ae0edfd709fbfcb4b9d0431f59c66d`  
		Last Modified: Tue, 08 Sep 2020 19:54:40 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c00dba1504124d6dd0793c8393017e4b3c55bf5255f74b3f601369d383e473b`  
		Last Modified: Tue, 08 Sep 2020 19:54:40 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b700ad87d0ab628858f56a1fce2ab53461cba34d2cd944bd228aa30f50d450d6`  
		Last Modified: Tue, 08 Sep 2020 19:54:43 GMT  
		Size: 15.4 MB (15428663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74ff3d7bc46fe04c2d82c767f2915613b09b2583c0b5684b98a987d57001bdf4`  
		Last Modified: Tue, 08 Sep 2020 19:54:40 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04bed820e925876e84c14c9b3c3757eff78205af8af904cf81889af4ff57010f`  
		Last Modified: Tue, 08 Sep 2020 22:54:44 GMT  
		Size: 1.2 KB (1184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd82a9c499871db7fa3b4a157555347f5ff16faff5ca52099aea680485fdc995`  
		Last Modified: Tue, 08 Sep 2020 22:54:47 GMT  
		Size: 10.7 MB (10667105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38b5a55cca3f054c217abfd908d363c18ba7b93fc28761e803a209c99ac50fa2`  
		Last Modified: Tue, 08 Sep 2020 22:54:44 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
