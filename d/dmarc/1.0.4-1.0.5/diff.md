# Comparing `tmp/dmarc-1.0.4.tar.gz` & `tmp/dmarc-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dmarc-1.0.4.tar", last modified: Thu Mar  7 21:49:16 2024, max compression
+gzip compressed data, was "dmarc-1.0.5.tar", last modified: Sun Apr  7 16:31:26 2024, max compression
```

## Comparing `dmarc-1.0.4.tar` & `dmarc-1.0.5.tar`

### file list

```diff
@@ -1,13 +1,25 @@
-drwxr-xr-x   0 dusan      (501) staff       (20)        0 2024-03-07 21:49:16.411740 dmarc-1.0.4/
--rw-r--r--   0 dusan      (501) staff       (20)     1091 2023-12-23 04:27:57.000000 dmarc-1.0.4/LICENSE
--rw-r--r--   0 dusan      (501) staff       (20)     1777 2024-03-07 21:49:16.410879 dmarc-1.0.4/PKG-INFO
--rw-r--r--   0 dusan      (501) staff       (20)      946 2024-03-07 20:59:57.000000 dmarc-1.0.4/README.md
-drwxr-xr-x   0 dusan      (501) staff       (20)        0 2024-03-07 21:49:16.405228 dmarc-1.0.4/dmarc/
--rw-r--r--   0 dusan      (501) staff       (20)    18335 2024-03-07 21:14:49.000000 dmarc-1.0.4/dmarc/__init__.py
-drwxr-xr-x   0 dusan      (501) staff       (20)        0 2024-03-07 21:49:16.410108 dmarc-1.0.4/dmarc.egg-info/
--rw-r--r--   0 dusan      (501) staff       (20)     1777 2024-03-07 21:49:16.000000 dmarc-1.0.4/dmarc.egg-info/PKG-INFO
--rw-r--r--   0 dusan      (501) staff       (20)      160 2024-03-07 21:49:16.000000 dmarc-1.0.4/dmarc.egg-info/SOURCES.txt
--rw-r--r--   0 dusan      (501) staff       (20)        1 2024-03-07 21:49:16.000000 dmarc-1.0.4/dmarc.egg-info/dependency_links.txt
--rw-r--r--   0 dusan      (501) staff       (20)        6 2024-03-07 21:49:16.000000 dmarc-1.0.4/dmarc.egg-info/top_level.txt
--rw-r--r--   0 dusan      (501) staff       (20)       38 2024-03-07 21:49:16.411961 dmarc-1.0.4/setup.cfg
--rw-r--r--   0 dusan      (501) staff       (20)     1081 2024-03-07 21:15:08.000000 dmarc-1.0.4/setup.py
+drwxr-xr-x   0 dusan      (501) staff       (20)        0 2024-04-07 16:31:26.864894 dmarc-1.0.5/
+-rw-r--r--   0 dusan      (501) staff       (20)     1091 2023-12-23 04:27:57.000000 dmarc-1.0.5/LICENSE
+-rw-r--r--   0 dusan      (501) staff       (20)     3274 2024-04-07 16:31:26.863559 dmarc-1.0.5/PKG-INFO
+-rw-r--r--   0 dusan      (501) staff       (20)     2250 2024-04-06 17:40:27.000000 dmarc-1.0.5/README.md
+drwxr-xr-x   0 dusan      (501) staff       (20)        0 2024-04-07 16:31:26.842983 dmarc-1.0.5/dmarc/
+-rw-r--r--   0 dusan      (501) staff       (20)    21966 2024-04-07 16:09:53.000000 dmarc-1.0.5/dmarc/__init__.py
+-rw-r--r--   0 dusan      (501) staff       (20)     1306 2024-03-23 19:44:51.000000 dmarc-1.0.5/dmarc/ar.py
+-rw-r--r--   0 dusan      (501) staff       (20)      983 2024-03-22 18:33:19.000000 dmarc-1.0.5/dmarc/asyncresolver.py
+-rw-r--r--   0 dusan      (501) staff       (20)      271 2024-03-23 21:26:06.000000 dmarc-1.0.5/dmarc/psl.py
+-rw-r--r--   0 dusan      (501) staff       (20)     1259 2024-03-21 21:48:07.000000 dmarc-1.0.5/dmarc/resolver.py
+drwxr-xr-x   0 dusan      (501) staff       (20)        0 2024-04-07 16:31:26.856776 dmarc-1.0.5/dmarc/tests/
+-rw-r--r--   0 dusan      (501) staff       (20)        0 2024-04-04 14:53:57.000000 dmarc-1.0.5/dmarc/tests/__init__.py
+-rw-r--r--   0 dusan      (501) staff       (20)     1045 2024-04-04 16:02:36.000000 dmarc-1.0.5/dmarc/tests/test_ar.py
+-rw-r--r--   0 dusan      (501) staff       (20)      516 2024-04-04 15:56:02.000000 dmarc-1.0.5/dmarc/tests/test_asyncresolver.py
+-rw-r--r--   0 dusan      (501) staff       (20)     7317 2024-04-07 15:39:42.000000 dmarc-1.0.5/dmarc/tests/test_dmarc.py
+-rw-r--r--   0 dusan      (501) staff       (20)      441 2024-04-04 18:59:04.000000 dmarc-1.0.5/dmarc/tests/test_psl.py
+-rw-r--r--   0 dusan      (501) staff       (20)      472 2024-04-04 15:59:24.000000 dmarc-1.0.5/dmarc/tests/test_resolver.py
+drwxr-xr-x   0 dusan      (501) staff       (20)        0 2024-04-07 16:31:26.860629 dmarc-1.0.5/dmarc.egg-info/
+-rw-r--r--   0 dusan      (501) staff       (20)     3274 2024-04-07 16:31:26.000000 dmarc-1.0.5/dmarc.egg-info/PKG-INFO
+-rw-r--r--   0 dusan      (501) staff       (20)      414 2024-04-07 16:31:26.000000 dmarc-1.0.5/dmarc.egg-info/SOURCES.txt
+-rw-r--r--   0 dusan      (501) staff       (20)        1 2024-04-07 16:31:26.000000 dmarc-1.0.5/dmarc.egg-info/dependency_links.txt
+-rw-r--r--   0 dusan      (501) staff       (20)       57 2024-04-07 16:31:26.000000 dmarc-1.0.5/dmarc.egg-info/requires.txt
+-rw-r--r--   0 dusan      (501) staff       (20)        6 2024-04-07 16:31:26.000000 dmarc-1.0.5/dmarc.egg-info/top_level.txt
+-rw-r--r--   0 dusan      (501) staff       (20)       38 2024-04-07 16:31:26.865174 dmarc-1.0.5/setup.cfg
+-rw-r--r--   0 dusan      (501) staff       (20)     1205 2024-04-07 16:00:27.000000 dmarc-1.0.5/setup.py
```

### Comparing `dmarc-1.0.4/LICENSE` & `dmarc-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dmarc-1.0.4/README.md` & `dmarc-1.0.5/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -11,27 +11,53 @@
 ```
 
 ## Usage
 
 ```python
 >>> import dmarc
 >>>
->>> # represent verified SPF and DKIM status
+>>> # Represent verified SPF and DKIM status
 >>> aspf = dmarc.SPF(domain='news.example.com', result=dmarc.SPF_PASS)
+>>> #aspf = dmarc.SPF.from_authres(SPFAuthenticationResult(result='pass', smtp_mailfrom='email@news.example.com'))
+>>> 
 >>> adkim = dmarc.DKIM(domain='example.com', result=dmarc.DKIM_PASS)
+>>> #adkim = dmarc.DKIM.from_authres(DKIMAuthenticationResult(result='pass', header_d='example.com'))
+>>>
 >>> try:
 ...     admarc = dmarc.DMARCPolicy(record='v=DMARC1; p=reject;', domain='example.com')
 ...     admarc.verify(spf=aspf, dkim=adkim)
+...     #admarc.verify(auth_results=[aspf, adkim, dmarc.DKIM('news.example.com', dmarc.DKIM_FAIL)])
 ...     adict = admarc.result.as_dict() # dict repr
 ... except dmarc.PolicyNoneError:
 ...     pass
 ... except dmarc.PolicyQuarantineError:
 ...     raise
 ... except dmarc.PolicyRejectError:
 ...     raise
 ... except dmarc.RecordSyntaxError:
 ...     raise
 ...
+>>> # dmarc rr resolver example
+>>> from dmarc.resolver import resolve, RecordNotFoundError, RecordMultiFoundError, RecordResolverError
+>>> from dmarc.psl import get_public_suffix
+>>> domain = 'example.com'
+>>> try:
+...     record = resolve(domain)
+... except RecordNotFoundError:
+...     org_domain = get_public_suffix(domain)
+...     if org_domain != domain:
+...             record = resolve(org_domain)
+... except RecordMultiFoundError:
+...     raise # permerror
+... except RecordResolverError:
+...     raise # temperror
+... 
+>>> # dmarc authres header example
+>>> from dmarc.ar import authres, AuthenticationResultsHeader
+>>> dares = authres(admarc.result) #DMARCAuthenticationResult factory
+>>> header = AuthenticationResultsHeader(authserv_id='myhostname', results=[dares])
+>>> str(header)
+'Authentication-Results: myhostname; dmarc=pass (domain=example.com adkim=r aspf=r p=reject pct=100) header.from=example.com policy.dmarc=none (disposition=none dkim=pass spf=pass)'
 ```
 
 ## License
 [MIT](https://choosealicense.com/licenses/mit/)
```

### Comparing `dmarc-1.0.4/dmarc/__init__.py` & `dmarc-1.0.5/dmarc/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,41 +1,49 @@
 """DMARC (Domain-based Message Authentication, Reporting & Conformance)
 
 Typical Usage:
 
     >>> import dmarc
     >>>
-    >>> # represent verified SPF and DKIM status
+    >>> # Represent verified SPF and DKIM status
     >>> aspf = dmarc.SPF(domain='news.example.com', result=dmarc.SPF_PASS)
+    >>> #aspf = dmarc.SPF.from_authres(SPFAuthenticationResult(result='pass', smtp_mailfrom='email@news.example.com'))
+    >>> 
     >>> adkim = dmarc.DKIM(domain='example.com', result=dmarc.DKIM_PASS)
+    >>> #adkim = dmarc.DKIM.from_authres(DKIMAuthenticationResult(result='pass', header_d='example.com'))
+    >>>
     >>> try:
     ...     admarc = dmarc.DMARCPolicy(record='v=DMARC1; p=reject;', domain='example.com')
     ...     admarc.verify(spf=aspf, dkim=adkim)
+    ...     #admarc.verify(auth_results=[aspf, adkim, dmarc.DKIM('news.example.com', dmarc.DKIM_FAIL)])
     ...     adict = admarc.result.as_dict() # dict repr
     ... except dmarc.PolicyNoneError:
     ...     pass
     ... except dmarc.PolicyQuarantineError:
     ...     raise
     ... except dmarc.PolicyRejectError:
     ...     raise
     ... except dmarc.RecordSyntaxError:
     ...     raise
     ...
 """
 
-__version__ = '1.0.4'
+__author__ = 'Dusan Obradovic <dusan@euracks.net>'
+__version__ = '1.0.5'
 
 import re
 
 SPF_PASS = 0
 SPF_NEUTRAL = 1
 SPF_FAIL = 2
 SPF_TEMPFAIL = 3
 SPF_PERMFAIL = 4
 SPF_SOFTFAIL = 5
+SPF_SCOPE_MFROM = 0
+SPF_SCOPE_HELO = 1
 
 DKIM_PASS = 0
 DKIM_FAIL = 1
 DKIM_TEMPFAIL = 2
 DKIM_PERMFAIL = 3
 DKIM_NEUTRAL = 4
 
@@ -70,49 +78,102 @@
 
 class Error(Exception):
     pass
 
 class RecordSyntaxError(Error):
     pass
 
+class RecordValueError(RecordSyntaxError):
+    pass
+
 class PolicyError(Error):
     pass
 
 class PolicyNoneError(PolicyError):
     pass
 
 class PolicyRejectError(PolicyError):
     pass
 
 class PolicyQuarantineError(PolicyError):
     pass
 
 class SPF(object):
-    def __init__(self, domain, result):
+    AR = {
+        'pass': SPF_PASS,
+        'neutral': SPF_NEUTRAL,
+        'fail': SPF_FAIL,
+        'temperror': SPF_TEMPFAIL,
+        'permerror': SPF_PERMFAIL,
+        'softfail': SPF_SOFTFAIL
+    }
+    
+    def __init__(self, domain, result, scope=None):
         """Represent a single domain SPF verification status
         
         Args:
             domain: Domain part of RFC5321.MailFrom
             result: one of SPF_PASS, SPF_FAIL, SPF_SOFTFAIL, SPF_NEUTRAL, SPF_TEMPFAIL, SPF_PERMFAIL
+            scope: one of SPF_SCOPE_MFROM, SPF_SCOPE_HELO
         """
         self.domain = domain
         self.result = result
+        self.scope = scope
+    
+    @classmethod
+    def from_authres(cls, ar):
+        """
+        Args:
+            ar: SPFAuthenticationResult object
+        
+        Returns:
+            SPF object
+        """
+        
+        if ar.smtp_mailfrom:
+            domain = ar.smtp_mailfrom.split('@')[-1]
+            scope = SPF_SCOPE_MFROM
+        else:
+            domain = ar.smtp_helo
+            scope = SPF_SCOPE_HELO
+        
+        return cls(domain, cls.AR.get(ar.result), scope)
 
 class DKIM(object):
+    AR = {
+        'pass': DKIM_PASS,
+        'fail': DKIM_FAIL,
+        'temperror': DKIM_TEMPFAIL,
+        'permerror': DKIM_PERMFAIL,
+        'neutral': DKIM_NEUTRAL
+    }
+    
     def __init__(self, domain, result, selector=None):
         """Represent a single domain DKIM verification status
         
         Args:
             domain: Domain value of the signature header d= tag
             result: one of DKIM_PASS, DKIM_FAIL, DKIM_NEUTRAL, DKIM_TEMPFAIL, DKIM_PERMFAIL
             selector: Selector value of the signature header s= tag
         """
         self.domain = domain
         self.result = result
         self.selector = selector
+    
+    @classmethod
+    def from_authres(cls, ar):
+        """
+        Args:
+            ar: DKIMAuthenticationResult object
+        
+        Returns:
+            DKIM object
+        """
+        
+        return cls(ar.header_d, cls.AR.get(ar.result), ar.header_s)
 
 class Policy(object):
     """Policy object:
     
     v: Protocol version
     p: Policy for organizational domain
     sp: Policy for subdomains of the OD
@@ -152,113 +213,113 @@
         """
         
         # The record must start with "v=DMARC1"
         # and the string "DMARC" is the only portion that is case-sensitive...
         pr = re.compile(r'^\s*([^=\s]+)\s*=(.*)$')
         parts = record.split(';')
         if len(parts) < 2:
-            raise RecordSyntaxError
+            raise RecordSyntaxError('Record must specify at least 2 tags')
         
         part = parts[0].strip()
         if not part:
-            raise RecordSyntaxError
+            raise RecordSyntaxError('Record no tag specified')
         
         res = pr.match(part)
         try:
             tag = res.group(1).strip().lower()
             value = res.group(2).strip()
         except AttributeError:
-            raise RecordSyntaxError
+            raise RecordSyntaxError(part)
         
         if tag != 'v' or value != self.v:
-            raise RecordSyntaxError
+            raise RecordSyntaxError('Record must start with v=DMARC1')
         
         for part in parts:
             part = part.strip()
             if not part:
                 continue
             
             res = pr.match(part)
             try:
                 tag = res.group(1).strip().lower()
                 value = res.group(2).strip().lower()
             except AttributeError:
-                raise RecordSyntaxError
+                raise RecordSyntaxError(part)
             
             if tag == 'p':
                 if 'none'.startswith(value):
                     self.p = RECORD_P_NONE
                     
                 elif 'reject'.startswith(value):
                     self.p = RECORD_P_REJECT
                     
                 elif 'quarantine'.startswith(value):
                     self.p = RECORD_P_QUARANTINE
                     
                 else:
-                    raise RecordSyntaxError
+                    raise RecordValueError(part)
                 
             elif tag == 'sp':
                 if 'none'.startswith(value):
                     self.sp = RECORD_P_NONE
                     
                 elif 'reject'.startswith(value):
                     self.sp = RECORD_P_REJECT
                     
                 elif 'quarantine'.startswith(value):
                     self.sp = RECORD_P_QUARANTINE
                     
                 else:
-                    raise RecordSyntaxError
+                    raise RecordValueError(part)
             
             elif tag == 'adkim':
                 if 'relaxed'.startswith(value):
                     self.adkim = RECORD_A_RELAXED
                 
                 elif 'strict'.startswith(value):
                     self.adkim = RECORD_A_STRICT
                 
                 else:
-                    raise RecordSyntaxError
+                    raise RecordValueError(part)
             
             elif tag == 'aspf':
                 if 'relaxed'.startswith(value):
                     self.aspf = RECORD_A_RELAXED
                 
                 elif 'strict'.startswith(value):
                     self.aspf = RECORD_A_STRICT
                 
                 else:
-                    raise RecordSyntaxError
+                    raise RecordValueError(part)
             
             elif tag == 'pct':
                 try:
                     self.pct = int(value)
                 except ValueError:
-                    raise RecordSyntaxError
+                    raise RecordValueError(part)
                 
                 if self.pct < 0 or self.pct > 100:
-                    raise RecordSyntaxError
+                    raise RecordValueError(part)
             
             elif tag == 'ri':
                 try:
                     self.ri = int(value)
                 except ValueError:
-                    raise RecordSyntaxError
+                    raise RecordValueError(part)
             
             elif tag == 'rf':
                 for x in value.split(','):
                     if 'afrf'.startswith(x):
                         self.rf |= RECORD_RF_AFRF
                     
                     elif 'iodef'.startswith(x):
                         self.rf |= RECORD_RF_IODEF
                     
                     else:
-                        raise RecordSyntaxError
+                        raise RecordValueError(part)
             
             elif tag == 'rua':
                 self.rua = value.split(',')
             
             elif tag == 'ruf':
                 self.ruf = value.split(',')
             
@@ -273,19 +334,19 @@
                     elif x == 'd':
                         self.fo |= RECORD_FO_D
                     
                     elif x == 's':
                         self.fo |= RECORD_FO_S
                     
                     else:
-                        raise RecordSyntaxError
+                        raise RecordValueError(part)
         
         
         if self.p == RECORD_P_UNSPECIFIED:
-            raise RecordSyntaxError
+            raise RecordValueError('Record required tag p unspecified')
         
         if self.adkim == RECORD_A_UNSPECIFIED:
             self.adkim = RECORD_A_RELAXED
         
         if self.aspf == RECORD_A_UNSPECIFIED:
             self.aspf = RECORD_A_RELAXED
         
@@ -362,15 +423,15 @@
         policy_evaluated = {}
         row = {}
         identifiers = {}
         auth_results = {}
         dkim = {}
         spf = {}
         
-        policy_published['domain'] = self.policy.domain
+        policy_published['domain'] = self.policy.org_domain or self.policy.domain
         policy_published['adkim'] = self.policy.adkim
         policy_published['aspf'] = self.policy.aspf
         if self.policy.p == RECORD_P_NONE:
             policy_published['p'] = 'none'
         elif self.policy.p == RECORD_P_QUARANTINE:
             policy_published['p'] = 'quarantine'
         elif self.policy.p == RECORD_P_REJECT:
@@ -428,14 +489,19 @@
             if self.adkim.selector:
                 dkim['selector'] = self.adkim.selector
             
             auth_results['dkim'] = dkim
         
         if self.aspf:
             spf['domain'] = self.aspf.domain
+            if self.aspf.scope == SPF_SCOPE_HELO:
+                spf['scope'] = 'helo'
+            elif self.aspf.scope == SPF_SCOPE_MFROM:
+                spf['scope'] = 'mfrom'
+            
             if self.aspf.result == SPF_FAIL:
                 spf['result'] = 'fail'
             elif self.aspf.result == SPF_NEUTRAL:
                 spf['result'] = 'neutral'
             elif self.aspf.result == SPF_PASS:
                 spf['result'] = 'pass'
             elif self.aspf.result == SPF_PERMFAIL:
@@ -566,10 +632,49 @@
         publicsuffix: PublicSuffixList object
     """
     def __init__(self, record, domain, org_domain=None, ip_addr=None, publicsuffix=None):
         self.dmarc = DMARC(publicsuffix)
         self.policy = self.dmarc.parse_record(record, domain, org_domain, ip_addr)
         self.result = None
     
-    def verify(self, spf=None, dkim=None):
+    def verify(self, spf=None, dkim=None, auth_results=[]):
+        """Policy disposition verification
+        
+        Args:
+            spf: SPF object
+            dkim: DKIM object
+            auth_results: Iterable (of authentication results)
+        
+        Returns:
+            None
+        
+        Raises:
+            PolicyNoneError: if POLICY_FAIL and POLICY_DIS_NONE
+            PolicyQuarantineError: if POLICY_FAIL and POLICY_DIS_QUARANTINE
+            PolicyRejectError: if POLICY_FAIL and POLICY_DIS_REJECT
+            PolicyError: if POLICY_FAIL and unknown disposition error
+        """
+        for ar in auth_results:
+            # The aligned authentication result is chosen over any result
+            if isinstance(ar, SPF):
+                spf = ar if self.isaligned(ar) else spf or ar
+            elif isinstance(ar, DKIM):
+                dkim = ar if self.isaligned(ar) else dkim or ar
+        
         self.result = self.dmarc.get_result(self.policy, spf, dkim)
         self.result.verify()
+    
+    def isaligned(self, ar):
+        if isinstance(ar, SPF):
+            return (
+                ar.result == SPF_PASS and 
+                self.dmarc.check_alignment(
+                        self.policy.domain, ar.domain, self.policy.aspf, self.dmarc.publicsuffix)
+            )
+        elif isinstance(ar, DKIM):
+            return (
+                ar.result == DKIM_PASS and 
+                self.dmarc.check_alignment(
+                        self.policy.domain, ar.domain, self.policy.adkim, self.dmarc.publicsuffix)
+            )
+        else:
+            raise ValueError("invalid authentication result '{0}'".format(ar))
```

### Comparing `dmarc-1.0.4/setup.py` & `dmarc-1.0.5/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="dmarc",
-    version="1.0.4",
+    version="1.0.5",
     author="Dusan Obradovic",
     author_email="dusan@euracks.net",
     description="Parse and evaluate DMARC email authentication policy",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license='MIT',
     url="https://gitlab.com/duobradovic/pydmarc",
@@ -22,8 +22,13 @@
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Topic :: Communications :: Email :: Mail Transport Agents",
         "Topic :: Communications :: Email :: Filters",
         "Topic :: Software Development :: Libraries :: Python Modules",
     ],
     python_requires='>=2.7',
+    extras_require={
+        "resolver": ['dnspython'],
+        "ar": ['authres'],
+        "psl": ['publicsuffix2'],
+    },
 )
```

