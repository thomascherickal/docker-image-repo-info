## `hylang:0-python3.7-windowsservercore-ltsc2016`

```console
$ docker pull hylang@sha256:39e74cef2ca1ab65678b2d1a0b4be4bcac0e93bdd063ef22d9537a643a6698a4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3986; amd64

### `hylang:0-python3.7-windowsservercore-ltsc2016` - windows version 10.0.14393.3986; amd64

```console
$ docker pull hylang@sha256:908536aabdd0d1ba66bd4341017b9cdd341c934f5cee24074252bbeb4f10f0c4
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5823921349 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6824dbe1e72d7d85e15024cdab302885d1dd5bff724a9183dd476d0be2e25c1a`
-	Default Command: `["hy"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Fri, 02 Oct 2020 17:07:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 14 Oct 2020 12:31:45 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 30 Oct 2020 00:14:08 GMT
ENV PYTHONIOENCODING=UTF-8
# Fri, 30 Oct 2020 00:34:07 GMT
ENV PYTHON_VERSION=3.7.9
# Fri, 30 Oct 2020 00:34:08 GMT
ENV PYTHON_RELEASE=3.7.9
# Fri, 30 Oct 2020 00:36:22 GMT
RUN $url = ('https://www.python.org/ftp/python/{0}/python-{1}-amd64.exe' -f $env:PYTHON_RELEASE, $env:PYTHON_VERSION); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'python.exe'; 		Write-Host 'Installing ...'; 	Start-Process python.exe -Wait 		-ArgumentList @( 			'/quiet', 			'InstallAllUsers=1', 			'TargetDir=C:\Python', 			'PrependPath=1', 			'Shortcuts=0', 			'Include_doc=0', 			'Include_pip=0', 			'Include_test=0' 		); 		$env:PATH = [Environment]::GetEnvironmentVariable('PATH', [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  python --version'; python --version; 		Write-Host 'Removing ...'; 	Remove-Item python.exe -Force; 		Write-Host 'Complete.'
# Fri, 30 Oct 2020 00:36:24 GMT
ENV PYTHON_PIP_VERSION=20.2.4
# Tue, 03 Nov 2020 21:23:39 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/fa7dc83944936bf09a0e4cb5d5ec852c0d256599/get-pip.py
# Tue, 03 Nov 2020 21:23:39 GMT
ENV PYTHON_GET_PIP_SHA256=6e0bb0a2c2533361d7f297ed547237caf1b7507f197835974c0dd7eba998c53c
# Tue, 03 Nov 2020 21:25:22 GMT
RUN Write-Host ('Downloading get-pip.py ({0}) ...' -f $env:PYTHON_GET_PIP_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:PYTHON_GET_PIP_URL -OutFile 'get-pip.py'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:PYTHON_GET_PIP_SHA256); 	if ((Get-FileHash 'get-pip.py' -Algorithm sha256).Hash -ne $env:PYTHON_GET_PIP_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host ('Installing pip=={0} ...' -f $env:PYTHON_PIP_VERSION); 	python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		('pip=={0}' -f $env:PYTHON_PIP_VERSION) 	; 	Remove-Item get-pip.py -Force; 		Write-Host 'Verifying pip install ...'; 	pip --version; 		Write-Host 'Complete.'
# Tue, 03 Nov 2020 21:25:22 GMT
CMD ["python"]
# Tue, 03 Nov 2020 21:51:10 GMT
ENV HY_VERSION=0.19.0
# Tue, 03 Nov 2020 21:52:36 GMT
RUN pip install --no-cache-dir ('hy == {0}' -f $env:HY_VERSION)
# Tue, 03 Nov 2020 21:52:37 GMT
CMD ["hy"]
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
	-	`sha256:97dc0237500b170e70f7bea25e66289624b0f31aaaa023dcbd4e88ae406fe558`  
		Last Modified: Fri, 30 Oct 2020 00:41:49 GMT  
		Size: 1.1 KB (1138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:448052cd3f5e3a52af8a874815a44a05522de5a31c38172559e060e0f520f24a`  
		Last Modified: Fri, 30 Oct 2020 00:49:46 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c38e97f5923ebc3a17ffe3f06baff5b066931be3a529d6df0cb9b36d520182ff`  
		Last Modified: Fri, 30 Oct 2020 00:49:45 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4318d66d89c3788fb6f53f7260b46b7feab94ef65a3e3c0fc3c71a491bfab8e`  
		Last Modified: Fri, 30 Oct 2020 00:50:49 GMT  
		Size: 56.5 MB (56471084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f4a730b9f786925c6a28579207b28178f75a3daa99fd7c6a6680d1fbf0288d2`  
		Last Modified: Fri, 30 Oct 2020 00:49:42 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:366d1b9ebe31536e368dfbc18b8b8e04bc9d60f4b44665f774dc4b148a9bacf5`  
		Last Modified: Tue, 03 Nov 2020 21:30:06 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:516f99475d8fe97cd6e317174436c4cfdc98f0cb595a049b925afa384f141ed9`  
		Last Modified: Tue, 03 Nov 2020 21:30:07 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abd28addc95dab814c5c3ee6518b5afda23d4923a73b862106b49f5b34877612`  
		Last Modified: Tue, 03 Nov 2020 21:30:11 GMT  
		Size: 15.4 MB (15410167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f7025d4f45a071504cde7cedf7876ed1201b7f3857fd961ec2a156a7182f317`  
		Last Modified: Tue, 03 Nov 2020 21:30:06 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5173ba3d3b3905369686ad0c609dd54f026dd423e913777f1a2aff1b99c60c5`  
		Last Modified: Tue, 03 Nov 2020 21:57:25 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52bcd8cac3efb7281cdf513fdcf2807ce1c92da4428c4525dba9bd8eb1504f5f`  
		Last Modified: Tue, 03 Nov 2020 21:57:27 GMT  
		Size: 10.7 MB (10677064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00f32311a8764fcc3eb9396fd31842f2fa1951d711cb14e131d7d82db151f9cc`  
		Last Modified: Tue, 03 Nov 2020 21:57:24 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
