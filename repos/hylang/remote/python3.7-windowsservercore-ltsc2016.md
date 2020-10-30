## `hylang:python3.7-windowsservercore-ltsc2016`

```console
$ docker pull hylang@sha256:ee39565ae3ae0518f8a0eddc8d51729b751b8049f96798612184b60a93e54bca
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3986; amd64

### `hylang:python3.7-windowsservercore-ltsc2016` - windows version 10.0.14393.3986; amd64

```console
$ docker pull hylang@sha256:e2ecd63f409ebf36a85660e689308abd0ecb39c32e5d4229e06e13cd595be41e
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5823919672 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:53cf4294f2deba7b6c0c9488b612a4b77f2f0c99c3c8cf59161e309a34276967`
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
# Fri, 30 Oct 2020 00:36:25 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/8283828b8fd6f1783daf55a765384e6d8d2c5014/get-pip.py
# Fri, 30 Oct 2020 00:36:26 GMT
ENV PYTHON_GET_PIP_SHA256=2250ab0a7e70f6fd22b955493f7f5cf1ea53e70b584a84a32573644a045b4bfb
# Fri, 30 Oct 2020 00:38:02 GMT
RUN Write-Host ('Downloading get-pip.py ({0}) ...' -f $env:PYTHON_GET_PIP_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:PYTHON_GET_PIP_URL -OutFile 'get-pip.py'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:PYTHON_GET_PIP_SHA256); 	if ((Get-FileHash 'get-pip.py' -Algorithm sha256).Hash -ne $env:PYTHON_GET_PIP_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host ('Installing pip=={0} ...' -f $env:PYTHON_PIP_VERSION); 	python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		('pip=={0}' -f $env:PYTHON_PIP_VERSION) 	; 	Remove-Item get-pip.py -Force; 		Write-Host 'Verifying pip install ...'; 	pip --version; 		Write-Host 'Complete.'
# Fri, 30 Oct 2020 00:38:04 GMT
CMD ["python"]
# Fri, 30 Oct 2020 01:12:08 GMT
ENV HY_VERSION=0.19.0
# Fri, 30 Oct 2020 01:13:35 GMT
RUN pip install --no-cache-dir ('hy == {0}' -f $env:HY_VERSION)
# Fri, 30 Oct 2020 01:13:36 GMT
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
	-	`sha256:9b599675cf6ac496f5549439d7657632aa8c5be1eaaffb34056c604efbeabd83`  
		Last Modified: Fri, 30 Oct 2020 00:49:41 GMT  
		Size: 1.1 KB (1143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c488dc0b7408276010313c248503f3f907a77512ed3b428484873feb036ed8f4`  
		Last Modified: Fri, 30 Oct 2020 00:49:41 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c202a24e7296426b37eab51d65f45a4b427c080192489ddd5e7854c49926d7b`  
		Last Modified: Fri, 30 Oct 2020 00:50:01 GMT  
		Size: 15.4 MB (15407307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:228ff6dbb21dffbc0fdd511a7ffc09d0125d85d163bd168ac5f326dd0409a345`  
		Last Modified: Fri, 30 Oct 2020 00:49:42 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f75786a7dd326bf96f2009952efe68e3c1bc967922ab8b81f30b39d6e464b8f`  
		Last Modified: Fri, 30 Oct 2020 01:15:57 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7344e741a0532d52564fa5c967678b29d093e818eda9a6645262db8d151571f7`  
		Last Modified: Fri, 30 Oct 2020 01:16:08 GMT  
		Size: 10.7 MB (10678230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26bd07c6e4d5028ff5b54e80312eef4bd03f3b17ff7b50fc9c50e657a4836ebb`  
		Last Modified: Fri, 30 Oct 2020 01:15:57 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
