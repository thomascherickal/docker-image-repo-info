## `hylang:python3.7-windowsservercore-ltsc2016`

```console
$ docker pull hylang@sha256:347ce2de06edaac058abf968014dd1e7722130d1fdc34661a7a89712e8a269a0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4046; amd64

### `hylang:python3.7-windowsservercore-ltsc2016` - windows version 10.0.14393.4046; amd64

```console
$ docker pull hylang@sha256:8aa48589a99e19c926cc503c62cdd97aa2f53c0b6c2cbdc23e325e41cae4841c
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 GB (5853669347 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1367164c901811fab1ae91f3008bcb49f6fdac7516bfaa8ddb0d8d01eec93fd9`
-	Default Command: `["hy"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 28 Oct 2020 18:03:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 11 Nov 2020 13:23:11 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Nov 2020 17:09:28 GMT
ENV PYTHONIOENCODING=UTF-8
# Wed, 11 Nov 2020 17:30:07 GMT
ENV PYTHON_VERSION=3.7.9
# Wed, 11 Nov 2020 17:30:08 GMT
ENV PYTHON_RELEASE=3.7.9
# Wed, 11 Nov 2020 17:32:24 GMT
RUN $url = ('https://www.python.org/ftp/python/{0}/python-{1}-amd64.exe' -f $env:PYTHON_RELEASE, $env:PYTHON_VERSION); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'python.exe'; 		Write-Host 'Installing ...'; 	Start-Process python.exe -Wait 		-ArgumentList @( 			'/quiet', 			'InstallAllUsers=1', 			'TargetDir=C:\Python', 			'PrependPath=1', 			'Shortcuts=0', 			'Include_doc=0', 			'Include_pip=0', 			'Include_test=0' 		); 		$env:PATH = [Environment]::GetEnvironmentVariable('PATH', [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  python --version'; python --version; 		Write-Host 'Removing ...'; 	Remove-Item python.exe -Force; 		Write-Host 'Complete.'
# Wed, 02 Dec 2020 01:24:09 GMT
ENV PYTHON_PIP_VERSION=20.3
# Wed, 02 Dec 2020 01:24:09 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/2357a5f805565496648ebf597bcffe9e2d9ce379/get-pip.py
# Wed, 02 Dec 2020 01:24:10 GMT
ENV PYTHON_GET_PIP_SHA256=7f28b41ce236af61a00dfcbd6fd38c52d46488ece91fb4585b95775b076bbc85
# Wed, 02 Dec 2020 01:25:50 GMT
RUN Write-Host ('Downloading get-pip.py ({0}) ...' -f $env:PYTHON_GET_PIP_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:PYTHON_GET_PIP_URL -OutFile 'get-pip.py'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:PYTHON_GET_PIP_SHA256); 	if ((Get-FileHash 'get-pip.py' -Algorithm sha256).Hash -ne $env:PYTHON_GET_PIP_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host ('Installing pip=={0} ...' -f $env:PYTHON_PIP_VERSION); 	python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		('pip=={0}' -f $env:PYTHON_PIP_VERSION) 	; 	Remove-Item get-pip.py -Force; 		Write-Host 'Verifying pip install ...'; 	pip --version; 		Write-Host 'Complete.'
# Wed, 02 Dec 2020 01:25:50 GMT
CMD ["python"]
# Wed, 02 Dec 2020 01:50:09 GMT
ENV HY_VERSION=0.19.0
# Wed, 02 Dec 2020 01:51:35 GMT
RUN pip install --no-cache-dir ('hy == {0}' -f $env:HY_VERSION)
# Wed, 02 Dec 2020 01:51:36 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4830fb08bc2df7ae80548c349b880c263ea87a7b93e13ecbc77c862b6e179558`  
		Size: 1.7 GB (1700572904 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:126d9a92c0cb7b68c56dec2dd5ba118de9dde3ec6368db734c5135fdf1528a33`  
		Last Modified: Wed, 11 Nov 2020 13:34:53 GMT  
		Size: 1.2 KB (1170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f32d36bd6ec3b70ad877771d7f97cafedd40418fb1bba46babfeda374e5ada5b`  
		Last Modified: Wed, 11 Nov 2020 17:37:45 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d2021b0490e902aab422f8843401b5f3abdaa0e93b5da3d9da20531b02056a3`  
		Last Modified: Wed, 11 Nov 2020 17:41:14 GMT  
		Size: 1.2 KB (1176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44172a67924cdacd1daaf1f6074b94db1697a39e56bf8fab5949562988a0666c`  
		Last Modified: Wed, 11 Nov 2020 17:41:14 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e559276d983ffa8a61b66e3f766c4e5347410f196330d29ef6578c3fbd9f43d5`  
		Last Modified: Wed, 11 Nov 2020 17:41:22 GMT  
		Size: 56.6 MB (56636759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb302c5021c3e449343f95400ae3adee26c5ed6e03f66a32997a65fdde430d80`  
		Last Modified: Wed, 02 Dec 2020 01:29:32 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8e9d08422b5cef449ac38be1dcee09bfc565b329cbb2da3748cf627ca42e22f`  
		Last Modified: Wed, 02 Dec 2020 01:29:32 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42d805d38cef1650d05f9847a900b3f14be68f7821fa3ff8618af5fabb4bb174`  
		Last Modified: Wed, 02 Dec 2020 01:29:32 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f28530d391125407d59ff270395b5860438f7472464af56252c5f3e6743a48f9`  
		Last Modified: Wed, 02 Dec 2020 01:29:37 GMT  
		Size: 15.6 MB (15618348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:518853be71728c2d94506227604b05d33de97a9ff73fda5e4da0321953fe8d90`  
		Last Modified: Wed, 02 Dec 2020 01:29:32 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1f24d7b66173698240bbf0d59c573b74cd6cd398426f5387195474906d0474f`  
		Last Modified: Wed, 02 Dec 2020 01:53:52 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e05a7987b6b60e81628d653366e3def96c5d94ba67d55c3330c70345abb20d0`  
		Last Modified: Wed, 02 Dec 2020 01:53:54 GMT  
		Size: 10.8 MB (10844055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:053d7b8414a599d7465015235ca0ed2bd208070c94deb7430b4c8e1c98f6f2bf`  
		Last Modified: Wed, 02 Dec 2020 01:53:53 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
