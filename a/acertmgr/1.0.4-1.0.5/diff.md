# Comparing `tmp/acertmgr-1.0.4.tar.gz` & `tmp/acertmgr-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/acertmgr-1.0.4.tar", last modified: Fri May 21 20:55:46 2021, max compression
+gzip compressed data, was "acertmgr-1.0.5.tar", last modified: Thu Jul 13 13:38:55 2023, max compression
```

## Comparing `acertmgr-1.0.4.tar` & `acertmgr-1.0.5.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-05-21 20:55:46.000000 acertmgr-1.0.4/
--rw-r--r--   0 runner    (1001) docker     (116)     3230 2021-05-21 20:55:46.000000 acertmgr-1.0.4/setup.py
--rw-r--r--   0 runner    (1001) docker     (116)       38 2021-05-21 20:55:46.000000 acertmgr-1.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)      755 2021-05-21 20:55:22.000000 acertmgr-1.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)    16953 2021-05-21 20:55:22.000000 acertmgr-1.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (116)    18667 2021-05-21 20:55:46.000000 acertmgr-1.0.4/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-05-21 20:55:46.000000 acertmgr-1.0.4/acertmgr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)      615 2021-05-21 20:55:46.000000 acertmgr-1.0.4/acertmgr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        9 2021-05-21 20:55:46.000000 acertmgr-1.0.4/acertmgr.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2021-05-21 20:55:46.000000 acertmgr-1.0.4/acertmgr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)      167 2021-05-21 20:55:46.000000 acertmgr-1.0.4/acertmgr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)    18667 2021-05-21 20:55:46.000000 acertmgr-1.0.4/acertmgr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)       44 2021-05-21 20:55:46.000000 acertmgr-1.0.4/acertmgr.egg-info/entry_points.txt
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-05-21 20:55:46.000000 acertmgr-1.0.4/acertmgr/
--rw-r--r--   0 runner    (1001) docker     (116)    18859 2021-05-21 20:55:22.000000 acertmgr-1.0.4/acertmgr/tools.py
--rw-r--r--   0 runner    (1001) docker     (116)      245 2021-05-21 20:55:22.000000 acertmgr-1.0.4/acertmgr/__main__.py
--rwxr-xr-x   0 runner    (1001) docker     (116)    10872 2021-05-21 20:55:22.000000 acertmgr-1.0.4/acertmgr/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-05-21 20:55:46.000000 acertmgr-1.0.4/acertmgr/modes/
--rw-r--r--   0 runner    (1001) docker     (116)      834 2021-05-21 20:55:22.000000 acertmgr-1.0.4/acertmgr/modes/abstract.py
--rw-r--r--   0 runner    (1001) docker     (116)     3016 2021-05-21 20:55:22.000000 acertmgr-1.0.4/acertmgr/modes/standalone.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-05-21 20:55:46.000000 acertmgr-1.0.4/acertmgr/modes/dns/
--rw-r--r--   0 runner    (1001) docker     (116)    10273 2021-05-21 20:55:22.000000 acertmgr-1.0.4/acertmgr/modes/dns/abstract.py
--rw-r--r--   0 runner    (1001) docker     (116)        0 2021-05-21 20:55:22.000000 acertmgr-1.0.4/acertmgr/modes/dns/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     4449 2021-05-21 20:55:22.000000 acertmgr-1.0.4/acertmgr/modes/dns/nsupdate.py
--rw-r--r--   0 runner    (1001) docker     (116)      906 2021-05-21 20:55:22.000000 acertmgr-1.0.4/acertmgr/modes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     2205 2021-05-21 20:55:22.000000 acertmgr-1.0.4/acertmgr/modes/webdir.py
--rw-r--r--   0 runner    (1001) docker     (116)    11528 2021-05-21 20:55:22.000000 acertmgr-1.0.4/acertmgr/configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-05-21 20:55:46.000000 acertmgr-1.0.4/acertmgr/authority/
--rw-r--r--   0 runner    (1001) docker     (116)     1264 2021-05-21 20:55:22.000000 acertmgr-1.0.4/acertmgr/authority/acme.py
--rw-r--r--   0 runner    (1001) docker     (116)     1280 2021-05-21 20:55:22.000000 acertmgr-1.0.4/acertmgr/authority/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    14086 2021-05-21 20:55:22.000000 acertmgr-1.0.4/acertmgr/authority/v2.py
--rw-r--r--   0 runner    (1001) docker     (116)     8863 2021-05-21 20:55:22.000000 acertmgr-1.0.4/acertmgr/authority/v1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:38:55.265661 acertmgr-1.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-07-13 13:38:06.000000 acertmgr-1.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17631 2023-07-13 13:38:55.265661 acertmgr-1.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16910 2023-07-13 13:38:06.000000 acertmgr-1.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:38:55.261661 acertmgr-1.0.5/acertmgr/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11164 2023-07-13 13:38:06.000000 acertmgr-1.0.5/acertmgr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-07-13 13:38:06.000000 acertmgr-1.0.5/acertmgr/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:38:55.265661 acertmgr-1.0.5/acertmgr/authority/
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-07-13 13:38:06.000000 acertmgr-1.0.5/acertmgr/authority/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-07-13 13:38:06.000000 acertmgr-1.0.5/acertmgr/authority/acme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8863 2023-07-13 13:38:06.000000 acertmgr-1.0.5/acertmgr/authority/v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14086 2023-07-13 13:38:06.000000 acertmgr-1.0.5/acertmgr/authority/v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12602 2023-07-13 13:38:06.000000 acertmgr-1.0.5/acertmgr/configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:38:55.265661 acertmgr-1.0.5/acertmgr/modes/
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-07-13 13:38:06.000000 acertmgr-1.0.5/acertmgr/modes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-07-13 13:38:06.000000 acertmgr-1.0.5/acertmgr/modes/abstract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:38:55.265661 acertmgr-1.0.5/acertmgr/modes/dns/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 13:38:06.000000 acertmgr-1.0.5/acertmgr/modes/dns/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10273 2023-07-13 13:38:06.000000 acertmgr-1.0.5/acertmgr/modes/dns/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4449 2023-07-13 13:38:06.000000 acertmgr-1.0.5/acertmgr/modes/dns/nsupdate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-07-13 13:38:06.000000 acertmgr-1.0.5/acertmgr/modes/standalone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-07-13 13:38:06.000000 acertmgr-1.0.5/acertmgr/modes/webdir.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18500 2023-07-13 13:38:06.000000 acertmgr-1.0.5/acertmgr/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:38:55.265661 acertmgr-1.0.5/acertmgr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17631 2023-07-13 13:38:55.000000 acertmgr-1.0.5/acertmgr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-07-13 13:38:55.000000 acertmgr-1.0.5/acertmgr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 13:38:55.000000 acertmgr-1.0.5/acertmgr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-13 13:38:55.000000 acertmgr-1.0.5/acertmgr.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-07-13 13:38:55.000000 acertmgr-1.0.5/acertmgr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-13 13:38:55.000000 acertmgr-1.0.5/acertmgr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 13:38:55.265661 acertmgr-1.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-07-13 13:38:54.000000 acertmgr-1.0.5/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `acertmgr-1.0.4/setup.py` & `acertmgr-1.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,15 @@
     "ocsp-validation": ["cryptography>=2.4"],
     "ed25519": ["cryptography>=2.6"],
 }
 
 if __name__ == "__main__":
     setup(
         name="acertmgr",
-        version='1.0.4',
+        version='1.0.5',
         author="Markus Hauschild",
         author_email="moepman@binary-kitchen.de",
         description="An automated certificate manager using ACME/letsencrypt",
         license="ISC",
         keywords="acme letsencrypt",
         url="https://github.com/moepman/acertmgr",
         packages=find_packages(),
```

### Comparing `acertmgr-1.0.4/LICENSE` & `acertmgr-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `acertmgr-1.0.4/README.md` & `acertmgr-1.0.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 The main file acertmgr.py is intended to be run regularly (e.g. as daily cron job / systemd timer) as root or user with enough privileges.
 
 Requirements
 ------------
 
   * Python (2.7+ and 3.5+ should work)
-  * cryptography>=0.6 (usually includes the optional idna module)
+  * cryptography>=0.6
 
 Optional requirements (to use specified features)
 ------------------------------------------------------
 
   * PyYAML: to parse YAML-formatted configuration files
   * dnspython: used by dns.* challenge handlers
   * idna: to allow automatic conversion of unicode domain names to their IDNA2008 counterparts
@@ -52,33 +52,33 @@
 Unless specified with a commandline parameter (see acertmgr.py --help) the optional global configuration is read from `/etc/acertmgr/acertmgr.conf`.
 Domains for which certificates should be obtained/renewed are be configured in `/etc/acertmgr/*.conf` (the global configuration is always excluded if it is in the same directory).
 By default the directory (work_dir) containing the working data (csr,certificate,key and ca files) is located at `/etc/acertmgr/`.
 
 4 configuration contexts are known (*domainconfig (d) > globalconfig (g) > commandline (c) > built-in defaults*) with the following directives (subject to change, usual usage context written bold):
 
 | Directive               | Context           | Description                                                                                                                                  | Built-in Default                     |
-| ---                     | ---               | ---                                                                                                                                          | ---                                  |
+| ---                     | ---               |----------------------------------------------------------------------------------------------------------------------------------------------| ---                                  |
 | -c/--config-file        | **c**             | global configuration file (optional)                                                                                                         | /etc/acertmgr/acertmgr.conf          |
 | -d/--config-dir         | **c**             | directory containing domain configuration files (ending with .conf, globalconfig will be excluded automatically if in same directory)        | /etc/acertmgr/*.conf                 |
 | -w/--work-dir           | **c**             | working directory containing csr/certificates/keys/ca files                                                                                  | /etc/acertmgr                        |
 | --force-renew           | **c**             | (or --renew-now) Immediately renew all certificates containing the given domain(s)                                                           |                                      |
 | --revoke                | **c**             | Revoke the certificate at the given path                                                                                                     |                                      |
 | --revoke-reason         | **c**             | Provide a reason code for the revocation (see https://tools.ietf.org/html/rfc5280#section-5.3.1 for valid values)                            |                                      |
 | domain (san-domain...): | **d**             | (domainconfig section start) Domains to use in the cert request. This value will be MD5-hashed as cert_id.                                   |                                      |
 | api                     | d,**g**           | Determines the API version used                                                                                                              | v2                                   |
-| authority               | d,**g**           | URL to the certificate authorities API                                                                                                       | https://acme-v02.api.letsencrypt.org |
+| authority               | d,**g**           | URL to the certificate authorities ACME API root (without trailing /directory or similar)                                                    | https://acme-v02.api.letsencrypt.org |
 | authority_tos_agreement | d,**g**,c         | Indicates agreement to the ToS of the certificate authority (--authority-tos-agreement on command line)                                      |                                      |
 | authority_contact_email | d,**g**           | (v2 API only) Contact e-mail to be registered with your account key                                                                          |                                      |
 | account_key             | d,**g**           | Path to the account key                                                                                                                      | {work_dir}/account.key               |
 | account_key_algorithm   | d,**g**           | Key-algorithm for newly generated account keys (RSA, EC, ED25519, ED448)                                                                     | RSA                                  |
 | account_key_length      | d,**g**           | Key-length for newly generated RSA account keys (in bits) or EC curve (256=P-256, 384=P-384, 521=P-521)                                      | depends on account_key_algorithm     |
 | ttl_days                | d,**g**           | Renew certificate if it has less than this value validity left                                                                               | 30                                   |
 | validate_ocsp           | d,**g**           | Renew certificate if it's OCSP status is REVOKED. Allowed values for this key are: false, sha1, sha224, sha256, sha384, sha512               | sha1 (as mandated by RFC5019)        |
 | cert_dir                | d,**g**           | Directory containing all certificate related data (crt,key,csr)                                                                              | {work_dir}                           |
-| key_algorithm           | d,**g**           | Key-algorithm for newly generated private keys (RSA, EC, ED25519, ED448)                                                                     | RSA                                  |
+| key_algorithm           | d,**g**           | Key-algorithm for newly generated private keys (RSA, ECC, ED25519, ED448)                                                                    | RSA                                  |
 | key_length              | d,**g**           | Key-length for newly generated RSA private keys (in bits) or EC curve (256=P-256, 384=P-384, 521=P-521)                                      | depends on key_algorithm             |
 | csr_static              | **d**,g           | Whether to re-use a static CSR or generate a new dynamic CSR                                                                                 | false                                |
 | csr_file                | **d**,g           | Path to store (and load) the certificate CSR file                                                                                            | {cert_dir}/{cert_id}.csr             |
 | ca_static               | **d**,g           | Whether to re-use a static CA or download a CA file                                                                                          | false                                |
 | ca_file                 | **d**,g           | Path to store (and load) the certificate authority file                                                                                      | {cert_dir}/{cert_id}.ca              |
 | cert_file               | **d**             | Path to store (and load) the certificate file                                                                                                | {cert_dir}/{cert_id}.crt             |
 | cert_revoke_superseded  | **d**,g           | Revoke the previous certificate with reason "superseded" after successful deployment                                                         | false                                |
@@ -117,8 +117,8 @@
 
   * DO read the source code, since it (usually) will be run as root
   * Make sure that your configuration files are NOT writable by other users - arbitrary commands can be executed after updating certificates
   * Try to run this program non-privileged if possible. This requires you to:
      * Create a dedicated user for acertmgr (e.g. acertmgr)
      * Run a acertmgr as that user (add acertmgr to that users cron!)
      * Access rights to read/write all files configured with the created user
-     * Run any programs/scripts defined on cert update as the created user (might need work-arounds with sudo or wrapper scripts)
+     * Run any programs/scripts defined on cert update as the created user (might need work-arounds with sudo or wrapper scripts)
```

### Comparing `acertmgr-1.0.4/PKG-INFO` & `acertmgr-1.0.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,146 +1,147 @@
 Metadata-Version: 2.1
 Name: acertmgr
-Version: 1.0.4
+Version: 1.0.5
 Summary: An automated certificate manager using ACME/letsencrypt
 Home-page: https://github.com/moepman/acertmgr
 Author: Markus Hauschild
 Author-email: moepman@binary-kitchen.de
 License: ISC
-Description: ACERTMGR
-        ========
-        
-        This is an automated certificate manager using ACME/letsencrypt with minimal dependencies.
-        
-        Running ACERTMGR
-        ----------------
-        
-        The main file acertmgr.py is intended to be run regularly (e.g. as daily cron job / systemd timer) as root or user with enough privileges.
-        
-        Requirements
-        ------------
-        
-          * Python (2.7+ and 3.5+ should work)
-          * cryptography>=0.6 (usually includes the optional idna module)
-        
-        Optional requirements (to use specified features)
-        ------------------------------------------------------
-        
-          * PyYAML: to parse YAML-formatted configuration files
-          * dnspython: used by dns.* challenge handlers
-          * idna: to allow automatic conversion of unicode domain names to their IDNA2008 counterparts
-          * cryptography>=2.1: for creating certificates with the OCSP must-staple flag (cert_must_staple)
-          * cryptography>=2.6: for usage of Ed25519/Ed448 keys
-        
-        Setup
-        -----
-        
-        You should decide which challenge mode you want to use with acertmgr:
-          * webdir: In this mode, responses to challenges are put into a directory, to be served by an existing webserver
-          * standalone: In this mode, challenges are completed by acertmgr directly. This starts a webserver to solve the challenges, which can be used standalone or together with an existing webserver that forwards request to a specified local port/address.
-          * dns.*: This mode puts the challenge into a TXT record for the domain (usually _acme-challenge.<domain>) where it will be parsed from by the authority
-          * dns.* (Alias mode): Can be used similar to the above but allows redirection of _acme-challenge.<domain> to any other (updatable domain) defined in dns_updatedomain via CNAME (e.g. _acme-challenge.example.net IN CNAME bla.foo.bar with dns_updatedomain="bla.foo.bar" in domainconfig)
-          * dns.nsupdate: Updates the TXT record using RFC2136
-        
-        You can optionally provide the private key files to be used with the ACME protocol (if you do not they will be automatically created):
-          * The account private key is (by default) expected at `/etc/acertmgr/account.key` (used to register an account with the authorities server)
-          * The domain private keys are (by default) expected at `/etc/acertmgr/{cert_id}.key`
-          * If you are missing these keys, they will be created for you (using RSA with the configured key_length) or you can create them using e.g. `openssl genrsa 4096 > /etc/acertmgr/account.key`
-          * Do not forget to set proper permissions of the keys using `chmod 0400 /etc/acertmgr/*.key` if you created those manually
-        
-        Finally, you need to setup the configuration files, as shown in the next section.
-        While testing, you can use the acme-staging authority instead, in order to avoid issuing too many certificates.
-        
-        Authorities (e.g. our default Let's Encrypt) will require you to accept their Terms of Service. This can be done either in the optional global config file and/or via a commandline parameter (see acertmgr.py --help).
-        
-        Configuration
-        -------------
-        
-        Configuration examples are included in the `docs/` directory. All configuration files can use yaml (requires PyYAML) or json syntax. (Note: The JSON examples may be incomplete due to inability to express comments in JSON)
-        
-        Unless specified with a commandline parameter (see acertmgr.py --help) the optional global configuration is read from `/etc/acertmgr/acertmgr.conf`.
-        Domains for which certificates should be obtained/renewed are be configured in `/etc/acertmgr/*.conf` (the global configuration is always excluded if it is in the same directory).
-        By default the directory (work_dir) containing the working data (csr,certificate,key and ca files) is located at `/etc/acertmgr/`.
-        
-        4 configuration contexts are known (*domainconfig (d) > globalconfig (g) > commandline (c) > built-in defaults*) with the following directives (subject to change, usual usage context written bold):
-        
-        | Directive               | Context           | Description                                                                                                                                  | Built-in Default                     |
-        | ---                     | ---               | ---                                                                                                                                          | ---                                  |
-        | -c/--config-file        | **c**             | global configuration file (optional)                                                                                                         | /etc/acertmgr/acertmgr.conf          |
-        | -d/--config-dir         | **c**             | directory containing domain configuration files (ending with .conf, globalconfig will be excluded automatically if in same directory)        | /etc/acertmgr/*.conf                 |
-        | -w/--work-dir           | **c**             | working directory containing csr/certificates/keys/ca files                                                                                  | /etc/acertmgr                        |
-        | --force-renew           | **c**             | (or --renew-now) Immediately renew all certificates containing the given domain(s)                                                           |                                      |
-        | --revoke                | **c**             | Revoke the certificate at the given path                                                                                                     |                                      |
-        | --revoke-reason         | **c**             | Provide a reason code for the revocation (see https://tools.ietf.org/html/rfc5280#section-5.3.1 for valid values)                            |                                      |
-        | domain (san-domain...): | **d**             | (domainconfig section start) Domains to use in the cert request. This value will be MD5-hashed as cert_id.                                   |                                      |
-        | api                     | d,**g**           | Determines the API version used                                                                                                              | v2                                   |
-        | authority               | d,**g**           | URL to the certificate authorities API                                                                                                       | https://acme-v02.api.letsencrypt.org |
-        | authority_tos_agreement | d,**g**,c         | Indicates agreement to the ToS of the certificate authority (--authority-tos-agreement on command line)                                      |                                      |
-        | authority_contact_email | d,**g**           | (v2 API only) Contact e-mail to be registered with your account key                                                                          |                                      |
-        | account_key             | d,**g**           | Path to the account key                                                                                                                      | {work_dir}/account.key               |
-        | account_key_algorithm   | d,**g**           | Key-algorithm for newly generated account keys (RSA, EC, ED25519, ED448)                                                                     | RSA                                  |
-        | account_key_length      | d,**g**           | Key-length for newly generated RSA account keys (in bits) or EC curve (256=P-256, 384=P-384, 521=P-521)                                      | depends on account_key_algorithm     |
-        | ttl_days                | d,**g**           | Renew certificate if it has less than this value validity left                                                                               | 30                                   |
-        | validate_ocsp           | d,**g**           | Renew certificate if it's OCSP status is REVOKED. Allowed values for this key are: false, sha1, sha224, sha256, sha384, sha512               | sha1 (as mandated by RFC5019)        |
-        | cert_dir                | d,**g**           | Directory containing all certificate related data (crt,key,csr)                                                                              | {work_dir}                           |
-        | key_algorithm           | d,**g**           | Key-algorithm for newly generated private keys (RSA, EC, ED25519, ED448)                                                                     | RSA                                  |
-        | key_length              | d,**g**           | Key-length for newly generated RSA private keys (in bits) or EC curve (256=P-256, 384=P-384, 521=P-521)                                      | depends on key_algorithm             |
-        | csr_static              | **d**,g           | Whether to re-use a static CSR or generate a new dynamic CSR                                                                                 | false                                |
-        | csr_file                | **d**,g           | Path to store (and load) the certificate CSR file                                                                                            | {cert_dir}/{cert_id}.csr             |
-        | ca_static               | **d**,g           | Whether to re-use a static CA or download a CA file                                                                                          | false                                |
-        | ca_file                 | **d**,g           | Path to store (and load) the certificate authority file                                                                                      | {cert_dir}/{cert_id}.ca              |
-        | cert_file               | **d**             | Path to store (and load) the certificate file                                                                                                | {cert_dir}/{cert_id}.crt             |
-        | cert_revoke_superseded  | **d**,g           | Revoke the previous certificate with reason "superseded" after successful deployment                                                         | false                                |
-        | cert_must_staple        | **d**,g           | Generate a certificate (request) with the OCSP must-staple flag (will be honoured on the next newly generated CSR if using csr_static=true)  | false                                |
-        | key_file                | **d**,g           | Path to store (and load) the private key file                                                                                                | {cert_dir}/{cert_id}.key             |
-        | mode                    | **d**,g           | Mode of challenge handling used                                                                                                              | standalone                           |
-        | webdir                  | **d**,g           | [webdir] Put acme challenges into this path                                                                                                  | /var/www/acme-challenge/             |
-        | http_verify             | **d**,g           | [webdir/standalone] Verify challenge before attempting authorization                                                                         | true                                 |
-        | bind_address            | **d**,g           | [standalone] Serve the challenge using a HTTP server on given IP                                                                             |                                      |
-        | port                    | **d**,g           | [standalone] Serve the challenge using a HTTP server on this port                                                                            | 80                                   |
-        | dns_ttl                 | **d**,g           | [dns.*] Write TXT records with this TTL (also determines the update wait time at twice this value                                            | 60                                   |
-        | dns_updatedomain        | **d**,g           | [dns.*] Write the TXT records to this domain (you have to create the necessary CNAME on the real challenge domain manually)                  |                                      |
-        | dns_verify_interval     | **d**,g           | [dns.*] Do verification checks when starting the challenge every {dns_verify_interval} seconds                                               | 10                                   |
-        | dns_verify_failtime     | **d**,g           | [dns.*] Fail challenge TXT record verification after {dns_verify_failtime} seconds                                                           | {dns_waittime} + 1                   |
-        | dns_verify_waittime     | **d**,g           | [dns.*] Assume DNS challenges are valid after {dns_verify_waittime}                                                                          | 2 * {dns_ttl}                        |
-        | dns_verify_all_ns       | **d**,g           | [dns.*] Verify DNS challenges by querying all known zone NS servers (resolved by zone master from SOA or dns_verify_server)                  | false                                |
-        | dns_verify_server       | **d**,g           | [dns.*] Verify DNS challenges by querying this DNS server unless 'dns_verify_all_ns' is enabled, then use to determine zone NS               |                                      |
-        | nsupdate_server         | **d**,g           | [dns.nsupdate] DNS Server to delegate the update to                                                                                          | {determine from zone SOA}            |
-        | nsupdate_verify         | **d**,g           | [dns.nsupdate] Verify TXT record on the update server upon creation                                                                          | true                                 |
-        | nsupdate_keyfile        | **d**,g           | [dns.nsupdate] Bind-formatted TSIG key file to use for updates (may be used instead of nsupdate_key*)                                        |                                      |
-        | nsupdate_keyname        | **d**,g           | [dns.nsupdate] TSIG key name to use for updates                                                                                              |                                      |
-        | nsupdate_keyvalue       | **d**,g           | [dns.nsupdate] TSIG key value to use for updates                                                                                             |                                      |
-        | nsupdate_keyalgorithm   | **d**,g           | [dns.nsupdate] TSIG key algorithm to use for updates                                                                                         | HMAC-MD5.SIG-ALG.REG.INT             |
-        | defaults:               | **g**             | Default deployment action settings used by all domains                                                                                       |                                      |
-        | path                    | **d**             | (deployment) deploy certificate data to the given file                                                                                       |                                      |
-        | format                  | **d**,g(defaults) | (deployment) deploy one or more of the following data to the file at path: key,crt,ca                                                        |                                      |
-        | user                    | **d**,g(defaults) | (deployment) change the user of the file deployed at path to this value (optional, defaults to acertmgr current effective user)              |                                      |
-        | group                   | **d**,g(defaults) | (deployment) change the group of the file deployed at path to this value (optional,defaults to acertmgr current effective group)             |                                      |
-        | perm                    | **d**,g(defaults) | (deployment) change the permissions of the file deployed at path to this value (optional, CAUTION: uses system defaults for new files)       |                                      |
-        | action                  | **d**,g(defaults) | (deployment) run the following action after deployment is finished. This command will be run in a shell and supports it's syntax. (optional) |                                      |
-        
-        Security
-        --------
-        
-        Please keep the following in mind when using this software:
-        
-          * DO read the source code, since it (usually) will be run as root
-          * Make sure that your configuration files are NOT writable by other users - arbitrary commands can be executed after updating certificates
-          * Try to run this program non-privileged if possible. This requires you to:
-             * Create a dedicated user for acertmgr (e.g. acertmgr)
-             * Run a acertmgr as that user (add acertmgr to that users cron!)
-             * Access rights to read/write all files configured with the created user
-             * Run any programs/scripts defined on cert update as the created user (might need work-arounds with sudo or wrapper scripts)
 Keywords: acme letsencrypt
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
 Classifier: Environment :: Console
 Classifier: Topic :: Security :: Cryptography
 Classifier: License :: OSI Approved :: ISC License (ISCL)
 Description-Content-Type: text/markdown
 Provides-Extra: dns
 Provides-Extra: yaml
 Provides-Extra: idna
 Provides-Extra: ocsp-must-staple
 Provides-Extra: ocsp-validation
 Provides-Extra: ed25519
+License-File: LICENSE
+
+ACERTMGR
+========
+
+This is an automated certificate manager using ACME/letsencrypt with minimal dependencies.
+
+Running ACERTMGR
+----------------
+
+The main file acertmgr.py is intended to be run regularly (e.g. as daily cron job / systemd timer) as root or user with enough privileges.
+
+Requirements
+------------
+
+  * Python (2.7+ and 3.5+ should work)
+  * cryptography>=0.6
+
+Optional requirements (to use specified features)
+------------------------------------------------------
+
+  * PyYAML: to parse YAML-formatted configuration files
+  * dnspython: used by dns.* challenge handlers
+  * idna: to allow automatic conversion of unicode domain names to their IDNA2008 counterparts
+  * cryptography>=2.1: for creating certificates with the OCSP must-staple flag (cert_must_staple)
+  * cryptography>=2.6: for usage of Ed25519/Ed448 keys
+
+Setup
+-----
+
+You should decide which challenge mode you want to use with acertmgr:
+  * webdir: In this mode, responses to challenges are put into a directory, to be served by an existing webserver
+  * standalone: In this mode, challenges are completed by acertmgr directly. This starts a webserver to solve the challenges, which can be used standalone or together with an existing webserver that forwards request to a specified local port/address.
+  * dns.*: This mode puts the challenge into a TXT record for the domain (usually _acme-challenge.<domain>) where it will be parsed from by the authority
+  * dns.* (Alias mode): Can be used similar to the above but allows redirection of _acme-challenge.<domain> to any other (updatable domain) defined in dns_updatedomain via CNAME (e.g. _acme-challenge.example.net IN CNAME bla.foo.bar with dns_updatedomain="bla.foo.bar" in domainconfig)
+  * dns.nsupdate: Updates the TXT record using RFC2136
+
+You can optionally provide the private key files to be used with the ACME protocol (if you do not they will be automatically created):
+  * The account private key is (by default) expected at `/etc/acertmgr/account.key` (used to register an account with the authorities server)
+  * The domain private keys are (by default) expected at `/etc/acertmgr/{cert_id}.key`
+  * If you are missing these keys, they will be created for you (using RSA with the configured key_length) or you can create them using e.g. `openssl genrsa 4096 > /etc/acertmgr/account.key`
+  * Do not forget to set proper permissions of the keys using `chmod 0400 /etc/acertmgr/*.key` if you created those manually
+
+Finally, you need to setup the configuration files, as shown in the next section.
+While testing, you can use the acme-staging authority instead, in order to avoid issuing too many certificates.
+
+Authorities (e.g. our default Let's Encrypt) will require you to accept their Terms of Service. This can be done either in the optional global config file and/or via a commandline parameter (see acertmgr.py --help).
+
+Configuration
+-------------
+
+Configuration examples are included in the `docs/` directory. All configuration files can use yaml (requires PyYAML) or json syntax. (Note: The JSON examples may be incomplete due to inability to express comments in JSON)
+
+Unless specified with a commandline parameter (see acertmgr.py --help) the optional global configuration is read from `/etc/acertmgr/acertmgr.conf`.
+Domains for which certificates should be obtained/renewed are be configured in `/etc/acertmgr/*.conf` (the global configuration is always excluded if it is in the same directory).
+By default the directory (work_dir) containing the working data (csr,certificate,key and ca files) is located at `/etc/acertmgr/`.
+
+4 configuration contexts are known (*domainconfig (d) > globalconfig (g) > commandline (c) > built-in defaults*) with the following directives (subject to change, usual usage context written bold):
+
+| Directive               | Context           | Description                                                                                                                                  | Built-in Default                     |
+| ---                     | ---               |----------------------------------------------------------------------------------------------------------------------------------------------| ---                                  |
+| -c/--config-file        | **c**             | global configuration file (optional)                                                                                                         | /etc/acertmgr/acertmgr.conf          |
+| -d/--config-dir         | **c**             | directory containing domain configuration files (ending with .conf, globalconfig will be excluded automatically if in same directory)        | /etc/acertmgr/*.conf                 |
+| -w/--work-dir           | **c**             | working directory containing csr/certificates/keys/ca files                                                                                  | /etc/acertmgr                        |
+| --force-renew           | **c**             | (or --renew-now) Immediately renew all certificates containing the given domain(s)                                                           |                                      |
+| --revoke                | **c**             | Revoke the certificate at the given path                                                                                                     |                                      |
+| --revoke-reason         | **c**             | Provide a reason code for the revocation (see https://tools.ietf.org/html/rfc5280#section-5.3.1 for valid values)                            |                                      |
+| domain (san-domain...): | **d**             | (domainconfig section start) Domains to use in the cert request. This value will be MD5-hashed as cert_id.                                   |                                      |
+| api                     | d,**g**           | Determines the API version used                                                                                                              | v2                                   |
+| authority               | d,**g**           | URL to the certificate authorities ACME API root (without trailing /directory or similar)                                                    | https://acme-v02.api.letsencrypt.org |
+| authority_tos_agreement | d,**g**,c         | Indicates agreement to the ToS of the certificate authority (--authority-tos-agreement on command line)                                      |                                      |
+| authority_contact_email | d,**g**           | (v2 API only) Contact e-mail to be registered with your account key                                                                          |                                      |
+| account_key             | d,**g**           | Path to the account key                                                                                                                      | {work_dir}/account.key               |
+| account_key_algorithm   | d,**g**           | Key-algorithm for newly generated account keys (RSA, EC, ED25519, ED448)                                                                     | RSA                                  |
+| account_key_length      | d,**g**           | Key-length for newly generated RSA account keys (in bits) or EC curve (256=P-256, 384=P-384, 521=P-521)                                      | depends on account_key_algorithm     |
+| ttl_days                | d,**g**           | Renew certificate if it has less than this value validity left                                                                               | 30                                   |
+| validate_ocsp           | d,**g**           | Renew certificate if it's OCSP status is REVOKED. Allowed values for this key are: false, sha1, sha224, sha256, sha384, sha512               | sha1 (as mandated by RFC5019)        |
+| cert_dir                | d,**g**           | Directory containing all certificate related data (crt,key,csr)                                                                              | {work_dir}                           |
+| key_algorithm           | d,**g**           | Key-algorithm for newly generated private keys (RSA, ECC, ED25519, ED448)                                                                    | RSA                                  |
+| key_length              | d,**g**           | Key-length for newly generated RSA private keys (in bits) or EC curve (256=P-256, 384=P-384, 521=P-521)                                      | depends on key_algorithm             |
+| csr_static              | **d**,g           | Whether to re-use a static CSR or generate a new dynamic CSR                                                                                 | false                                |
+| csr_file                | **d**,g           | Path to store (and load) the certificate CSR file                                                                                            | {cert_dir}/{cert_id}.csr             |
+| ca_static               | **d**,g           | Whether to re-use a static CA or download a CA file                                                                                          | false                                |
+| ca_file                 | **d**,g           | Path to store (and load) the certificate authority file                                                                                      | {cert_dir}/{cert_id}.ca              |
+| cert_file               | **d**             | Path to store (and load) the certificate file                                                                                                | {cert_dir}/{cert_id}.crt             |
+| cert_revoke_superseded  | **d**,g           | Revoke the previous certificate with reason "superseded" after successful deployment                                                         | false                                |
+| cert_must_staple        | **d**,g           | Generate a certificate (request) with the OCSP must-staple flag (will be honoured on the next newly generated CSR if using csr_static=true)  | false                                |
+| key_file                | **d**,g           | Path to store (and load) the private key file                                                                                                | {cert_dir}/{cert_id}.key             |
+| mode                    | **d**,g           | Mode of challenge handling used                                                                                                              | standalone                           |
+| webdir                  | **d**,g           | [webdir] Put acme challenges into this path                                                                                                  | /var/www/acme-challenge/             |
+| http_verify             | **d**,g           | [webdir/standalone] Verify challenge before attempting authorization                                                                         | true                                 |
+| bind_address            | **d**,g           | [standalone] Serve the challenge using a HTTP server on given IP                                                                             |                                      |
+| port                    | **d**,g           | [standalone] Serve the challenge using a HTTP server on this port                                                                            | 80                                   |
+| dns_ttl                 | **d**,g           | [dns.*] Write TXT records with this TTL (also determines the update wait time at twice this value                                            | 60                                   |
+| dns_updatedomain        | **d**,g           | [dns.*] Write the TXT records to this domain (you have to create the necessary CNAME on the real challenge domain manually)                  |                                      |
+| dns_verify_interval     | **d**,g           | [dns.*] Do verification checks when starting the challenge every {dns_verify_interval} seconds                                               | 10                                   |
+| dns_verify_failtime     | **d**,g           | [dns.*] Fail challenge TXT record verification after {dns_verify_failtime} seconds                                                           | {dns_waittime} + 1                   |
+| dns_verify_waittime     | **d**,g           | [dns.*] Assume DNS challenges are valid after {dns_verify_waittime}                                                                          | 2 * {dns_ttl}                        |
+| dns_verify_all_ns       | **d**,g           | [dns.*] Verify DNS challenges by querying all known zone NS servers (resolved by zone master from SOA or dns_verify_server)                  | false                                |
+| dns_verify_server       | **d**,g           | [dns.*] Verify DNS challenges by querying this DNS server unless 'dns_verify_all_ns' is enabled, then use to determine zone NS               |                                      |
+| nsupdate_server         | **d**,g           | [dns.nsupdate] DNS Server to delegate the update to                                                                                          | {determine from zone SOA}            |
+| nsupdate_verify         | **d**,g           | [dns.nsupdate] Verify TXT record on the update server upon creation                                                                          | true                                 |
+| nsupdate_keyfile        | **d**,g           | [dns.nsupdate] Bind-formatted TSIG key file to use for updates (may be used instead of nsupdate_key*)                                        |                                      |
+| nsupdate_keyname        | **d**,g           | [dns.nsupdate] TSIG key name to use for updates                                                                                              |                                      |
+| nsupdate_keyvalue       | **d**,g           | [dns.nsupdate] TSIG key value to use for updates                                                                                             |                                      |
+| nsupdate_keyalgorithm   | **d**,g           | [dns.nsupdate] TSIG key algorithm to use for updates                                                                                         | HMAC-MD5.SIG-ALG.REG.INT             |
+| defaults:               | **g**             | Default deployment action settings used by all domains                                                                                       |                                      |
+| path                    | **d**             | (deployment) deploy certificate data to the given file                                                                                       |                                      |
+| format                  | **d**,g(defaults) | (deployment) deploy one or more of the following data to the file at path: key,crt,ca                                                        |                                      |
+| user                    | **d**,g(defaults) | (deployment) change the user of the file deployed at path to this value (optional, defaults to acertmgr current effective user)              |                                      |
+| group                   | **d**,g(defaults) | (deployment) change the group of the file deployed at path to this value (optional,defaults to acertmgr current effective group)             |                                      |
+| perm                    | **d**,g(defaults) | (deployment) change the permissions of the file deployed at path to this value (optional, CAUTION: uses system defaults for new files)       |                                      |
+| action                  | **d**,g(defaults) | (deployment) run the following action after deployment is finished. This command will be run in a shell and supports it's syntax. (optional) |                                      |
+
+Security
+--------
+
+Please keep the following in mind when using this software:
+
+  * DO read the source code, since it (usually) will be run as root
+  * Make sure that your configuration files are NOT writable by other users - arbitrary commands can be executed after updating certificates
+  * Try to run this program non-privileged if possible. This requires you to:
+     * Create a dedicated user for acertmgr (e.g. acertmgr)
+     * Run a acertmgr as that user (add acertmgr to that users cron!)
+     * Access rights to read/write all files configured with the created user
+     * Run any programs/scripts defined on cert update as the created user (might need work-arounds with sudo or wrapper scripts)
```

### Comparing `acertmgr-1.0.4/acertmgr.egg-info/SOURCES.txt` & `acertmgr-1.0.5/acertmgr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `acertmgr-1.0.4/acertmgr.egg-info/PKG-INFO` & `acertmgr-1.0.5/acertmgr.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,146 +1,147 @@
 Metadata-Version: 2.1
 Name: acertmgr
-Version: 1.0.4
+Version: 1.0.5
 Summary: An automated certificate manager using ACME/letsencrypt
 Home-page: https://github.com/moepman/acertmgr
 Author: Markus Hauschild
 Author-email: moepman@binary-kitchen.de
 License: ISC
-Description: ACERTMGR
-        ========
-        
-        This is an automated certificate manager using ACME/letsencrypt with minimal dependencies.
-        
-        Running ACERTMGR
-        ----------------
-        
-        The main file acertmgr.py is intended to be run regularly (e.g. as daily cron job / systemd timer) as root or user with enough privileges.
-        
-        Requirements
-        ------------
-        
-          * Python (2.7+ and 3.5+ should work)
-          * cryptography>=0.6 (usually includes the optional idna module)
-        
-        Optional requirements (to use specified features)
-        ------------------------------------------------------
-        
-          * PyYAML: to parse YAML-formatted configuration files
-          * dnspython: used by dns.* challenge handlers
-          * idna: to allow automatic conversion of unicode domain names to their IDNA2008 counterparts
-          * cryptography>=2.1: for creating certificates with the OCSP must-staple flag (cert_must_staple)
-          * cryptography>=2.6: for usage of Ed25519/Ed448 keys
-        
-        Setup
-        -----
-        
-        You should decide which challenge mode you want to use with acertmgr:
-          * webdir: In this mode, responses to challenges are put into a directory, to be served by an existing webserver
-          * standalone: In this mode, challenges are completed by acertmgr directly. This starts a webserver to solve the challenges, which can be used standalone or together with an existing webserver that forwards request to a specified local port/address.
-          * dns.*: This mode puts the challenge into a TXT record for the domain (usually _acme-challenge.<domain>) where it will be parsed from by the authority
-          * dns.* (Alias mode): Can be used similar to the above but allows redirection of _acme-challenge.<domain> to any other (updatable domain) defined in dns_updatedomain via CNAME (e.g. _acme-challenge.example.net IN CNAME bla.foo.bar with dns_updatedomain="bla.foo.bar" in domainconfig)
-          * dns.nsupdate: Updates the TXT record using RFC2136
-        
-        You can optionally provide the private key files to be used with the ACME protocol (if you do not they will be automatically created):
-          * The account private key is (by default) expected at `/etc/acertmgr/account.key` (used to register an account with the authorities server)
-          * The domain private keys are (by default) expected at `/etc/acertmgr/{cert_id}.key`
-          * If you are missing these keys, they will be created for you (using RSA with the configured key_length) or you can create them using e.g. `openssl genrsa 4096 > /etc/acertmgr/account.key`
-          * Do not forget to set proper permissions of the keys using `chmod 0400 /etc/acertmgr/*.key` if you created those manually
-        
-        Finally, you need to setup the configuration files, as shown in the next section.
-        While testing, you can use the acme-staging authority instead, in order to avoid issuing too many certificates.
-        
-        Authorities (e.g. our default Let's Encrypt) will require you to accept their Terms of Service. This can be done either in the optional global config file and/or via a commandline parameter (see acertmgr.py --help).
-        
-        Configuration
-        -------------
-        
-        Configuration examples are included in the `docs/` directory. All configuration files can use yaml (requires PyYAML) or json syntax. (Note: The JSON examples may be incomplete due to inability to express comments in JSON)
-        
-        Unless specified with a commandline parameter (see acertmgr.py --help) the optional global configuration is read from `/etc/acertmgr/acertmgr.conf`.
-        Domains for which certificates should be obtained/renewed are be configured in `/etc/acertmgr/*.conf` (the global configuration is always excluded if it is in the same directory).
-        By default the directory (work_dir) containing the working data (csr,certificate,key and ca files) is located at `/etc/acertmgr/`.
-        
-        4 configuration contexts are known (*domainconfig (d) > globalconfig (g) > commandline (c) > built-in defaults*) with the following directives (subject to change, usual usage context written bold):
-        
-        | Directive               | Context           | Description                                                                                                                                  | Built-in Default                     |
-        | ---                     | ---               | ---                                                                                                                                          | ---                                  |
-        | -c/--config-file        | **c**             | global configuration file (optional)                                                                                                         | /etc/acertmgr/acertmgr.conf          |
-        | -d/--config-dir         | **c**             | directory containing domain configuration files (ending with .conf, globalconfig will be excluded automatically if in same directory)        | /etc/acertmgr/*.conf                 |
-        | -w/--work-dir           | **c**             | working directory containing csr/certificates/keys/ca files                                                                                  | /etc/acertmgr                        |
-        | --force-renew           | **c**             | (or --renew-now) Immediately renew all certificates containing the given domain(s)                                                           |                                      |
-        | --revoke                | **c**             | Revoke the certificate at the given path                                                                                                     |                                      |
-        | --revoke-reason         | **c**             | Provide a reason code for the revocation (see https://tools.ietf.org/html/rfc5280#section-5.3.1 for valid values)                            |                                      |
-        | domain (san-domain...): | **d**             | (domainconfig section start) Domains to use in the cert request. This value will be MD5-hashed as cert_id.                                   |                                      |
-        | api                     | d,**g**           | Determines the API version used                                                                                                              | v2                                   |
-        | authority               | d,**g**           | URL to the certificate authorities API                                                                                                       | https://acme-v02.api.letsencrypt.org |
-        | authority_tos_agreement | d,**g**,c         | Indicates agreement to the ToS of the certificate authority (--authority-tos-agreement on command line)                                      |                                      |
-        | authority_contact_email | d,**g**           | (v2 API only) Contact e-mail to be registered with your account key                                                                          |                                      |
-        | account_key             | d,**g**           | Path to the account key                                                                                                                      | {work_dir}/account.key               |
-        | account_key_algorithm   | d,**g**           | Key-algorithm for newly generated account keys (RSA, EC, ED25519, ED448)                                                                     | RSA                                  |
-        | account_key_length      | d,**g**           | Key-length for newly generated RSA account keys (in bits) or EC curve (256=P-256, 384=P-384, 521=P-521)                                      | depends on account_key_algorithm     |
-        | ttl_days                | d,**g**           | Renew certificate if it has less than this value validity left                                                                               | 30                                   |
-        | validate_ocsp           | d,**g**           | Renew certificate if it's OCSP status is REVOKED. Allowed values for this key are: false, sha1, sha224, sha256, sha384, sha512               | sha1 (as mandated by RFC5019)        |
-        | cert_dir                | d,**g**           | Directory containing all certificate related data (crt,key,csr)                                                                              | {work_dir}                           |
-        | key_algorithm           | d,**g**           | Key-algorithm for newly generated private keys (RSA, EC, ED25519, ED448)                                                                     | RSA                                  |
-        | key_length              | d,**g**           | Key-length for newly generated RSA private keys (in bits) or EC curve (256=P-256, 384=P-384, 521=P-521)                                      | depends on key_algorithm             |
-        | csr_static              | **d**,g           | Whether to re-use a static CSR or generate a new dynamic CSR                                                                                 | false                                |
-        | csr_file                | **d**,g           | Path to store (and load) the certificate CSR file                                                                                            | {cert_dir}/{cert_id}.csr             |
-        | ca_static               | **d**,g           | Whether to re-use a static CA or download a CA file                                                                                          | false                                |
-        | ca_file                 | **d**,g           | Path to store (and load) the certificate authority file                                                                                      | {cert_dir}/{cert_id}.ca              |
-        | cert_file               | **d**             | Path to store (and load) the certificate file                                                                                                | {cert_dir}/{cert_id}.crt             |
-        | cert_revoke_superseded  | **d**,g           | Revoke the previous certificate with reason "superseded" after successful deployment                                                         | false                                |
-        | cert_must_staple        | **d**,g           | Generate a certificate (request) with the OCSP must-staple flag (will be honoured on the next newly generated CSR if using csr_static=true)  | false                                |
-        | key_file                | **d**,g           | Path to store (and load) the private key file                                                                                                | {cert_dir}/{cert_id}.key             |
-        | mode                    | **d**,g           | Mode of challenge handling used                                                                                                              | standalone                           |
-        | webdir                  | **d**,g           | [webdir] Put acme challenges into this path                                                                                                  | /var/www/acme-challenge/             |
-        | http_verify             | **d**,g           | [webdir/standalone] Verify challenge before attempting authorization                                                                         | true                                 |
-        | bind_address            | **d**,g           | [standalone] Serve the challenge using a HTTP server on given IP                                                                             |                                      |
-        | port                    | **d**,g           | [standalone] Serve the challenge using a HTTP server on this port                                                                            | 80                                   |
-        | dns_ttl                 | **d**,g           | [dns.*] Write TXT records with this TTL (also determines the update wait time at twice this value                                            | 60                                   |
-        | dns_updatedomain        | **d**,g           | [dns.*] Write the TXT records to this domain (you have to create the necessary CNAME on the real challenge domain manually)                  |                                      |
-        | dns_verify_interval     | **d**,g           | [dns.*] Do verification checks when starting the challenge every {dns_verify_interval} seconds                                               | 10                                   |
-        | dns_verify_failtime     | **d**,g           | [dns.*] Fail challenge TXT record verification after {dns_verify_failtime} seconds                                                           | {dns_waittime} + 1                   |
-        | dns_verify_waittime     | **d**,g           | [dns.*] Assume DNS challenges are valid after {dns_verify_waittime}                                                                          | 2 * {dns_ttl}                        |
-        | dns_verify_all_ns       | **d**,g           | [dns.*] Verify DNS challenges by querying all known zone NS servers (resolved by zone master from SOA or dns_verify_server)                  | false                                |
-        | dns_verify_server       | **d**,g           | [dns.*] Verify DNS challenges by querying this DNS server unless 'dns_verify_all_ns' is enabled, then use to determine zone NS               |                                      |
-        | nsupdate_server         | **d**,g           | [dns.nsupdate] DNS Server to delegate the update to                                                                                          | {determine from zone SOA}            |
-        | nsupdate_verify         | **d**,g           | [dns.nsupdate] Verify TXT record on the update server upon creation                                                                          | true                                 |
-        | nsupdate_keyfile        | **d**,g           | [dns.nsupdate] Bind-formatted TSIG key file to use for updates (may be used instead of nsupdate_key*)                                        |                                      |
-        | nsupdate_keyname        | **d**,g           | [dns.nsupdate] TSIG key name to use for updates                                                                                              |                                      |
-        | nsupdate_keyvalue       | **d**,g           | [dns.nsupdate] TSIG key value to use for updates                                                                                             |                                      |
-        | nsupdate_keyalgorithm   | **d**,g           | [dns.nsupdate] TSIG key algorithm to use for updates                                                                                         | HMAC-MD5.SIG-ALG.REG.INT             |
-        | defaults:               | **g**             | Default deployment action settings used by all domains                                                                                       |                                      |
-        | path                    | **d**             | (deployment) deploy certificate data to the given file                                                                                       |                                      |
-        | format                  | **d**,g(defaults) | (deployment) deploy one or more of the following data to the file at path: key,crt,ca                                                        |                                      |
-        | user                    | **d**,g(defaults) | (deployment) change the user of the file deployed at path to this value (optional, defaults to acertmgr current effective user)              |                                      |
-        | group                   | **d**,g(defaults) | (deployment) change the group of the file deployed at path to this value (optional,defaults to acertmgr current effective group)             |                                      |
-        | perm                    | **d**,g(defaults) | (deployment) change the permissions of the file deployed at path to this value (optional, CAUTION: uses system defaults for new files)       |                                      |
-        | action                  | **d**,g(defaults) | (deployment) run the following action after deployment is finished. This command will be run in a shell and supports it's syntax. (optional) |                                      |
-        
-        Security
-        --------
-        
-        Please keep the following in mind when using this software:
-        
-          * DO read the source code, since it (usually) will be run as root
-          * Make sure that your configuration files are NOT writable by other users - arbitrary commands can be executed after updating certificates
-          * Try to run this program non-privileged if possible. This requires you to:
-             * Create a dedicated user for acertmgr (e.g. acertmgr)
-             * Run a acertmgr as that user (add acertmgr to that users cron!)
-             * Access rights to read/write all files configured with the created user
-             * Run any programs/scripts defined on cert update as the created user (might need work-arounds with sudo or wrapper scripts)
 Keywords: acme letsencrypt
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
 Classifier: Environment :: Console
 Classifier: Topic :: Security :: Cryptography
 Classifier: License :: OSI Approved :: ISC License (ISCL)
 Description-Content-Type: text/markdown
 Provides-Extra: dns
 Provides-Extra: yaml
 Provides-Extra: idna
 Provides-Extra: ocsp-must-staple
 Provides-Extra: ocsp-validation
 Provides-Extra: ed25519
+License-File: LICENSE
+
+ACERTMGR
+========
+
+This is an automated certificate manager using ACME/letsencrypt with minimal dependencies.
+
+Running ACERTMGR
+----------------
+
+The main file acertmgr.py is intended to be run regularly (e.g. as daily cron job / systemd timer) as root or user with enough privileges.
+
+Requirements
+------------
+
+  * Python (2.7+ and 3.5+ should work)
+  * cryptography>=0.6
+
+Optional requirements (to use specified features)
+------------------------------------------------------
+
+  * PyYAML: to parse YAML-formatted configuration files
+  * dnspython: used by dns.* challenge handlers
+  * idna: to allow automatic conversion of unicode domain names to their IDNA2008 counterparts
+  * cryptography>=2.1: for creating certificates with the OCSP must-staple flag (cert_must_staple)
+  * cryptography>=2.6: for usage of Ed25519/Ed448 keys
+
+Setup
+-----
+
+You should decide which challenge mode you want to use with acertmgr:
+  * webdir: In this mode, responses to challenges are put into a directory, to be served by an existing webserver
+  * standalone: In this mode, challenges are completed by acertmgr directly. This starts a webserver to solve the challenges, which can be used standalone or together with an existing webserver that forwards request to a specified local port/address.
+  * dns.*: This mode puts the challenge into a TXT record for the domain (usually _acme-challenge.<domain>) where it will be parsed from by the authority
+  * dns.* (Alias mode): Can be used similar to the above but allows redirection of _acme-challenge.<domain> to any other (updatable domain) defined in dns_updatedomain via CNAME (e.g. _acme-challenge.example.net IN CNAME bla.foo.bar with dns_updatedomain="bla.foo.bar" in domainconfig)
+  * dns.nsupdate: Updates the TXT record using RFC2136
+
+You can optionally provide the private key files to be used with the ACME protocol (if you do not they will be automatically created):
+  * The account private key is (by default) expected at `/etc/acertmgr/account.key` (used to register an account with the authorities server)
+  * The domain private keys are (by default) expected at `/etc/acertmgr/{cert_id}.key`
+  * If you are missing these keys, they will be created for you (using RSA with the configured key_length) or you can create them using e.g. `openssl genrsa 4096 > /etc/acertmgr/account.key`
+  * Do not forget to set proper permissions of the keys using `chmod 0400 /etc/acertmgr/*.key` if you created those manually
+
+Finally, you need to setup the configuration files, as shown in the next section.
+While testing, you can use the acme-staging authority instead, in order to avoid issuing too many certificates.
+
+Authorities (e.g. our default Let's Encrypt) will require you to accept their Terms of Service. This can be done either in the optional global config file and/or via a commandline parameter (see acertmgr.py --help).
+
+Configuration
+-------------
+
+Configuration examples are included in the `docs/` directory. All configuration files can use yaml (requires PyYAML) or json syntax. (Note: The JSON examples may be incomplete due to inability to express comments in JSON)
+
+Unless specified with a commandline parameter (see acertmgr.py --help) the optional global configuration is read from `/etc/acertmgr/acertmgr.conf`.
+Domains for which certificates should be obtained/renewed are be configured in `/etc/acertmgr/*.conf` (the global configuration is always excluded if it is in the same directory).
+By default the directory (work_dir) containing the working data (csr,certificate,key and ca files) is located at `/etc/acertmgr/`.
+
+4 configuration contexts are known (*domainconfig (d) > globalconfig (g) > commandline (c) > built-in defaults*) with the following directives (subject to change, usual usage context written bold):
+
+| Directive               | Context           | Description                                                                                                                                  | Built-in Default                     |
+| ---                     | ---               |----------------------------------------------------------------------------------------------------------------------------------------------| ---                                  |
+| -c/--config-file        | **c**             | global configuration file (optional)                                                                                                         | /etc/acertmgr/acertmgr.conf          |
+| -d/--config-dir         | **c**             | directory containing domain configuration files (ending with .conf, globalconfig will be excluded automatically if in same directory)        | /etc/acertmgr/*.conf                 |
+| -w/--work-dir           | **c**             | working directory containing csr/certificates/keys/ca files                                                                                  | /etc/acertmgr                        |
+| --force-renew           | **c**             | (or --renew-now) Immediately renew all certificates containing the given domain(s)                                                           |                                      |
+| --revoke                | **c**             | Revoke the certificate at the given path                                                                                                     |                                      |
+| --revoke-reason         | **c**             | Provide a reason code for the revocation (see https://tools.ietf.org/html/rfc5280#section-5.3.1 for valid values)                            |                                      |
+| domain (san-domain...): | **d**             | (domainconfig section start) Domains to use in the cert request. This value will be MD5-hashed as cert_id.                                   |                                      |
+| api                     | d,**g**           | Determines the API version used                                                                                                              | v2                                   |
+| authority               | d,**g**           | URL to the certificate authorities ACME API root (without trailing /directory or similar)                                                    | https://acme-v02.api.letsencrypt.org |
+| authority_tos_agreement | d,**g**,c         | Indicates agreement to the ToS of the certificate authority (--authority-tos-agreement on command line)                                      |                                      |
+| authority_contact_email | d,**g**           | (v2 API only) Contact e-mail to be registered with your account key                                                                          |                                      |
+| account_key             | d,**g**           | Path to the account key                                                                                                                      | {work_dir}/account.key               |
+| account_key_algorithm   | d,**g**           | Key-algorithm for newly generated account keys (RSA, EC, ED25519, ED448)                                                                     | RSA                                  |
+| account_key_length      | d,**g**           | Key-length for newly generated RSA account keys (in bits) or EC curve (256=P-256, 384=P-384, 521=P-521)                                      | depends on account_key_algorithm     |
+| ttl_days                | d,**g**           | Renew certificate if it has less than this value validity left                                                                               | 30                                   |
+| validate_ocsp           | d,**g**           | Renew certificate if it's OCSP status is REVOKED. Allowed values for this key are: false, sha1, sha224, sha256, sha384, sha512               | sha1 (as mandated by RFC5019)        |
+| cert_dir                | d,**g**           | Directory containing all certificate related data (crt,key,csr)                                                                              | {work_dir}                           |
+| key_algorithm           | d,**g**           | Key-algorithm for newly generated private keys (RSA, ECC, ED25519, ED448)                                                                    | RSA                                  |
+| key_length              | d,**g**           | Key-length for newly generated RSA private keys (in bits) or EC curve (256=P-256, 384=P-384, 521=P-521)                                      | depends on key_algorithm             |
+| csr_static              | **d**,g           | Whether to re-use a static CSR or generate a new dynamic CSR                                                                                 | false                                |
+| csr_file                | **d**,g           | Path to store (and load) the certificate CSR file                                                                                            | {cert_dir}/{cert_id}.csr             |
+| ca_static               | **d**,g           | Whether to re-use a static CA or download a CA file                                                                                          | false                                |
+| ca_file                 | **d**,g           | Path to store (and load) the certificate authority file                                                                                      | {cert_dir}/{cert_id}.ca              |
+| cert_file               | **d**             | Path to store (and load) the certificate file                                                                                                | {cert_dir}/{cert_id}.crt             |
+| cert_revoke_superseded  | **d**,g           | Revoke the previous certificate with reason "superseded" after successful deployment                                                         | false                                |
+| cert_must_staple        | **d**,g           | Generate a certificate (request) with the OCSP must-staple flag (will be honoured on the next newly generated CSR if using csr_static=true)  | false                                |
+| key_file                | **d**,g           | Path to store (and load) the private key file                                                                                                | {cert_dir}/{cert_id}.key             |
+| mode                    | **d**,g           | Mode of challenge handling used                                                                                                              | standalone                           |
+| webdir                  | **d**,g           | [webdir] Put acme challenges into this path                                                                                                  | /var/www/acme-challenge/             |
+| http_verify             | **d**,g           | [webdir/standalone] Verify challenge before attempting authorization                                                                         | true                                 |
+| bind_address            | **d**,g           | [standalone] Serve the challenge using a HTTP server on given IP                                                                             |                                      |
+| port                    | **d**,g           | [standalone] Serve the challenge using a HTTP server on this port                                                                            | 80                                   |
+| dns_ttl                 | **d**,g           | [dns.*] Write TXT records with this TTL (also determines the update wait time at twice this value                                            | 60                                   |
+| dns_updatedomain        | **d**,g           | [dns.*] Write the TXT records to this domain (you have to create the necessary CNAME on the real challenge domain manually)                  |                                      |
+| dns_verify_interval     | **d**,g           | [dns.*] Do verification checks when starting the challenge every {dns_verify_interval} seconds                                               | 10                                   |
+| dns_verify_failtime     | **d**,g           | [dns.*] Fail challenge TXT record verification after {dns_verify_failtime} seconds                                                           | {dns_waittime} + 1                   |
+| dns_verify_waittime     | **d**,g           | [dns.*] Assume DNS challenges are valid after {dns_verify_waittime}                                                                          | 2 * {dns_ttl}                        |
+| dns_verify_all_ns       | **d**,g           | [dns.*] Verify DNS challenges by querying all known zone NS servers (resolved by zone master from SOA or dns_verify_server)                  | false                                |
+| dns_verify_server       | **d**,g           | [dns.*] Verify DNS challenges by querying this DNS server unless 'dns_verify_all_ns' is enabled, then use to determine zone NS               |                                      |
+| nsupdate_server         | **d**,g           | [dns.nsupdate] DNS Server to delegate the update to                                                                                          | {determine from zone SOA}            |
+| nsupdate_verify         | **d**,g           | [dns.nsupdate] Verify TXT record on the update server upon creation                                                                          | true                                 |
+| nsupdate_keyfile        | **d**,g           | [dns.nsupdate] Bind-formatted TSIG key file to use for updates (may be used instead of nsupdate_key*)                                        |                                      |
+| nsupdate_keyname        | **d**,g           | [dns.nsupdate] TSIG key name to use for updates                                                                                              |                                      |
+| nsupdate_keyvalue       | **d**,g           | [dns.nsupdate] TSIG key value to use for updates                                                                                             |                                      |
+| nsupdate_keyalgorithm   | **d**,g           | [dns.nsupdate] TSIG key algorithm to use for updates                                                                                         | HMAC-MD5.SIG-ALG.REG.INT             |
+| defaults:               | **g**             | Default deployment action settings used by all domains                                                                                       |                                      |
+| path                    | **d**             | (deployment) deploy certificate data to the given file                                                                                       |                                      |
+| format                  | **d**,g(defaults) | (deployment) deploy one or more of the following data to the file at path: key,crt,ca                                                        |                                      |
+| user                    | **d**,g(defaults) | (deployment) change the user of the file deployed at path to this value (optional, defaults to acertmgr current effective user)              |                                      |
+| group                   | **d**,g(defaults) | (deployment) change the group of the file deployed at path to this value (optional,defaults to acertmgr current effective group)             |                                      |
+| perm                    | **d**,g(defaults) | (deployment) change the permissions of the file deployed at path to this value (optional, CAUTION: uses system defaults for new files)       |                                      |
+| action                  | **d**,g(defaults) | (deployment) run the following action after deployment is finished. This command will be run in a shell and supports it's syntax. (optional) |                                      |
+
+Security
+--------
+
+Please keep the following in mind when using this software:
+
+  * DO read the source code, since it (usually) will be run as root
+  * Make sure that your configuration files are NOT writable by other users - arbitrary commands can be executed after updating certificates
+  * Try to run this program non-privileged if possible. This requires you to:
+     * Create a dedicated user for acertmgr (e.g. acertmgr)
+     * Run a acertmgr as that user (add acertmgr to that users cron!)
+     * Access rights to read/write all files configured with the created user
+     * Run any programs/scripts defined on cert update as the created user (might need work-arounds with sudo or wrapper scripts)
```

### Comparing `acertmgr-1.0.4/acertmgr/tools.py` & `acertmgr-1.0.5/acertmgr/tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,14 +34,16 @@
     pass
 
 try:
     from urllib.request import urlopen, Request  # Python 3
 except ImportError:
     from urllib2 import urlopen, Request  # Python 2
 
+LOG_REPLACEMENTS = {}
+
 
 class InvalidCertificateError(Exception):
     pass
 
 
 # @brief a simple, portable indent function
 def indent(text, spaces=0):
@@ -55,14 +57,17 @@
         prefix = "Error: "
     elif warning:
         prefix = "Warning: "
     else:
         prefix = ""
 
     output = prefix + msg
+    for k, v in LOG_REPLACEMENTS.items():
+        output = output.replace(k, v)
+
     if exc:
         _, exc_value, _ = sys.exc_info()
         if not getattr(exc, '__traceback__', None) and exc == exc_value:
             # Traceback handling on Python 2 is ugly, so we only output it if the exception is the current sys one
             formatted_exc = traceback.format_exc()
         else:
             formatted_exc = traceback.format_exception(type(exc), exc, getattr(exc, '__traceback__', None))
@@ -135,15 +140,15 @@
             key_size = 4096
         key_format = serialization.PrivateFormat.TraditionalOpenSSL
         private_key = rsa.generate_private_key(
             public_exponent=65537,
             key_size=key_size,
             backend=default_backend()
         )
-    elif key_algo.lower() == 'ec':
+    elif key_algo.lower() == 'ec' or key_algo.lower() == 'ecc':
         if not key_size or key_size == 256:
             key_curve = ec.SECP256R1
         elif key_size == 384:
             key_curve = ec.SECP384R1
         elif key_size == 521:
             key_curve = ec.SECP521R1
         else:
@@ -239,16 +244,15 @@
 def get_cert_domains(cert):
     san_cert = cert.extensions.get_extension_for_oid(ExtensionOID.SUBJECT_ALTERNATIVE_NAME)
     domains = set()
     domains.add(cert.subject.get_attributes_for_oid(NameOID.COMMON_NAME)[0].value)
     if san_cert:
         for d in san_cert.value:
             domains.add(d.value)
-    # Convert IDNA domain to correct representation and return the list
-    return [x for x, _ in idna_convert(domains)]
+    return domains
 
 
 # @brief determine certificate cn
 def get_cert_cn(cert):
     return "CN={}".format(cert.subject.get_attributes_for_oid(NameOID.COMMON_NAME)[0].value)
 
 
@@ -381,34 +385,27 @@
     if not os.path.isfile(target):
         return False
     target_date = os.path.getmtime(target)
     crt_date = os.path.getmtime(file)
     return target_date >= crt_date
 
 
-# @brief convert domain list to idna representation (if applicable
-def idna_convert(domainlist):
-    if any(ord(c) >= 128 for c in ''.join(domainlist)):
-        try:
-            domaintranslation = list()
-            for domain in domainlist:
-                if any(ord(c) >= 128 for c in domain):
-                    # Translate IDNA domain name from a unicode domain (handle wildcards separately)
-                    if domain.startswith('*.'):
-                        idna_domain = "*.{}".format(domain[2:].encode('idna').decode('ascii'))
-                    else:
-                        idna_domain = domain.encode('idna').decode('ascii')
-                    result = idna_domain, domain
-                else:
-                    result = domain, domain
-                domaintranslation.append(result)
-            return domaintranslation
-        except Exception as e:
-            log("Unicode domain(s) found but IDNA names could not be translated due to error: {}".format(e), error=True)
-    return [(x, x) for x in domainlist]
+# @brief convert domain to idna representation (if applicable
+def idna_convert(domain):
+    try:
+        if any(ord(c) >= 128 for c in domain):
+            # Translate IDNA domain name from a unicode domain (handle wildcards separately)
+            if domain.startswith('*.'):
+                idna_domain = "*.{}".format(domain[2:].encode('idna').decode('ascii'))
+            else:
+                idna_domain = domain.encode('idna').decode('ascii')
+            return idna_domain
+    except Exception as e:
+        log("Unicode domain(s) found but IDNA names could not be translated due to error: {}".format(e), error=True)
+    return domain
 
 
 # @brief validate the OCSP status for a given certificate by the given issuer
 def is_ocsp_valid(cert, issuer, hash_algo):
     if hash_algo == 'sha1':
         algorithm = hashes.SHA1
     elif hash_algo == 'sha224':
@@ -431,15 +428,15 @@
         aia = cert.extensions.get_extension_for_oid(ExtensionOID.AUTHORITY_INFORMATION_ACCESS)
         for data in aia.value:
             if data.access_method == x509.OID_OCSP:
                 ocsp_urls.append(data.access_location.value)
 
         # This is a bit of a hack due to validation problems within cryptography (TODO: Check if this is still true)
         # Correct replacement:  ocsprequest = ocsp.OCSPRequestBuilder().add_certificate(cert, issuer, algorithm).build()
-        ocsprequest = ocsp.OCSPRequestBuilder((cert, issuer, algorithm)).build()
+        ocsprequest = ocsp.OCSPRequestBuilder((cert, issuer, (algorithm)())).build()
         ocsprequestdata = ocsprequest.public_bytes(serialization.Encoding.DER)
         for ocsp_url in ocsp_urls:
             response = get_url(ocsp_url,
                                ocsprequestdata,
                                {
                                    'Accept': 'application/ocsp-response',
                                    'Content-Type': 'application/ocsp-request',
```

### Comparing `acertmgr-1.0.4/acertmgr/__init__.py` & `acertmgr-1.0.5/acertmgr/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 import stat
 import subprocess
 import sys
 
 from acertmgr import configuration, tools
 from acertmgr.authority import authority
 from acertmgr.modes import challenge_handler
-from acertmgr.tools import log
+from acertmgr.tools import log, LOG_REPLACEMENTS
 
 try:
     import pwd
     import grp
 except ImportError:
     # Warnings will be reported upon usage below
     pass
@@ -135,14 +135,18 @@
     acme.register_account()
     acme.revoke_crt(cert, reason)
 
 
 def main():
     # load config
     runtimeconfig, domainconfigs = configuration.load()
+    # register idna-mapped domains as LOG_REPLACEMENTS for better readability of log output
+    for domainconfig in domainconfigs:
+        LOG_REPLACEMENTS.update({k: "{} [{}]".format(k, v) for k, v in domainconfig['domainlist_idna_mapped'].items()})
+    # Start processing
     if runtimeconfig.get('mode') == 'revoke':
         # Mode: revoke certificate
         log("Revoking {}".format(runtimeconfig['revoke']))
         cert_revoke(tools.read_pem_file(runtimeconfig['revoke']),
                     domainconfigs,
                     runtimeconfig['fallback_authority'],
                     runtimeconfig['revoke_reason'])
```

### Comparing `acertmgr-1.0.4/acertmgr/modes/abstract.py` & `acertmgr-1.0.5/acertmgr/modes/abstract.py`

 * *Files identical despite different names*

### Comparing `acertmgr-1.0.4/acertmgr/modes/standalone.py` & `acertmgr-1.0.5/acertmgr/modes/standalone.py`

 * *Files identical despite different names*

### Comparing `acertmgr-1.0.4/acertmgr/modes/dns/abstract.py` & `acertmgr-1.0.5/acertmgr/modes/dns/abstract.py`

 * *Files identical despite different names*

### Comparing `acertmgr-1.0.4/acertmgr/modes/dns/nsupdate.py` & `acertmgr-1.0.5/acertmgr/modes/dns/nsupdate.py`

 * *Files identical despite different names*

### Comparing `acertmgr-1.0.4/acertmgr/modes/__init__.py` & `acertmgr-1.0.5/acertmgr/modes/__init__.py`

 * *Files identical despite different names*

### Comparing `acertmgr-1.0.4/acertmgr/modes/webdir.py` & `acertmgr-1.0.5/acertmgr/modes/webdir.py`

 * *Files identical despite different names*

### Comparing `acertmgr-1.0.4/acertmgr/configuration.py` & `acertmgr-1.0.5/acertmgr/configuration.py`

 * *Files 3% similar despite different names*

```diff
@@ -86,17 +86,22 @@
 
     # Basic domain information
     domains, localconfig = entry
     config['domainlist'] = domains.split(' ')
     config['id'] = hashlib.md5(domains.encode('utf-8')).hexdigest()
 
     # Convert unicode to IDNA domains
-    config['domaintranslation'] = idna_convert(config['domainlist'])
-    if len(config['domaintranslation']) > 0:
-        config['domainlist'] = [x for x, _ in config['domaintranslation']]
+    config['domainlist_idna_mapped'] = {}
+    for idx in range(0, len(config['domainlist'])):
+        if any(ord(c) >= 128 for c in config['domainlist'][idx]):
+            domain_human = config['domainlist'][idx]
+            domain_idna = idna_convert(domain_human)
+            if domain_idna != domain_human:
+                config['domainlist'][idx] = domain_idna  # Update domain with idna counterpart
+                config['domainlist_idna_mapped'][domain_idna] = domain_human  # Store original domain for reference
 
     # Action config defaults
     config['defaults'] = globalconfig.get('defaults', {})
 
     # Authority related config options
     config['authority'] = parse_authority(localconfig, globalconfig, runtimeconfig)
 
@@ -115,33 +120,37 @@
 
     # Whether to include request for OCSP must-staple in the certificate
     update_config_value(config, 'cert_must_staple', localconfig, globalconfig, "false")
 
     # Use a static cert request
     update_config_value(config, 'csr_static', localconfig, globalconfig, "false")
 
+    # SSL key algorithm (if key has to be (re-)generated)
+    update_config_value(config, 'key_algorithm', localconfig, globalconfig, None)
+    # Update config id if we have a key algorithm set to allow for
+    # multiple certs with different algorithms for the same set of domains
+    if config.get('key_algorithm', None):
+        config['id'] += "_" + config['key_algorithm'].lower()
+
+    # SSL key length (if key has to be (re-)generated, converted to int)
+    update_config_value(config, 'key_length', localconfig, globalconfig, None)
+    config['key_length'] = int(config['key_length']) if config['key_length'] else None
+
     # SSL cert request location
     update_config_value(config, 'csr_file', localconfig, globalconfig,
                         os.path.join(config['cert_dir'], "{}.csr".format(config['id'])))
 
     # SSL cert location (with compatibility to older versions)
     update_config_value(config, 'cert_file', localconfig, globalconfig,
                         os.path.join(config['cert_dir'], "{}.crt".format(config['id'])))
 
     # SSL key location (with compatibility to older versions)
     update_config_value(config, 'key_file', localconfig, globalconfig,
                         os.path.join(config['cert_dir'], "{}.key".format(config['id'])))
 
-    # SSL key algorithm (if key has to be (re-)generated)
-    update_config_value(config, 'key_algorithm', localconfig, globalconfig, None)
-
-    # SSL key length (if key has to be (re-)generated, converted to int)
-    update_config_value(config, 'key_length', localconfig, globalconfig, None)
-    config['key_length'] = int(config['key_length']) if config['key_length'] else None
-
     # SSL CA location / use static
     update_config_value(config, 'ca_file', localconfig, globalconfig,
                         os.path.join(config['cert_dir'], "{}.ca".format(config['id'])))
     update_config_value(config, 'ca_static', localconfig, globalconfig, "false")
 
     # Domain action configuration
     config['actions'] = list()
@@ -158,16 +167,16 @@
 
         # Determine generic domain handler config values
         genericfgs = [x for x in handlerconfigs if 'domain' not in x]
         if len(genericfgs) > 0:
             cfg.update(genericfgs[0])
 
         # Update handler config with more specific values (use original names for translated unicode domains)
-        _domain = _domaintranslation_dict.get(domain, domain)
-        specificcfgs = [x for x in handlerconfigs if 'domain' in x and x['domain'] == _domain]
+        specificcfgs = [x for x in handlerconfigs if
+                        'domain' in x and x['domain'] == config['domainlist_idna_mapped'].get(domain, domain)]
         if len(specificcfgs) > 0:
             cfg.update(specificcfgs[0])
 
         config['handlers'][domain] = cfg
 
     return config
 
@@ -218,17 +227,17 @@
     if args.authority_tos_agreement:
         runtimeconfig['authority_tos_agreement'] = args.authority_tos_agreement
     else:
         runtimeconfig['authority_tos_agreement'] = None
 
     # - force-rewew
     if args.force_renew:
-        domaintranslation = idna_convert(args.force_renew.split(' '))
+        domaintranslation = [idna_convert(d) for d in args.force_renew.split(' ')]
         if len(domaintranslation) > 0:
-            runtimeconfig['force_renew'] = [x for x, _ in domaintranslation]
+            runtimeconfig['force_renew'] = domaintranslation
         else:
             runtimeconfig['force_renew'] = args.force_renew.split(' ')
 
     # - revoke
     if args.revoke:
         runtimeconfig['mode'] = 'revoke'
         runtimeconfig['revoke'] = args.revoke
@@ -251,19 +260,33 @@
         for domain_config_file in os.listdir(domain_config_dir):
             domain_config_file = os.path.join(domain_config_dir, domain_config_file)
             # check file extension and skip if global config file
             if domain_config_file.endswith(".conf") and \
                     os.path.abspath(domain_config_file) != os.path.abspath(global_config_file):
                 with io.open(domain_config_file) as config_fd:
                     try:
-                        for entry in json.load(config_fd).items():
-                            domainconfigs.append(parse_config_entry(entry, globalconfig, runtimeconfig))
+                        data = json.load(config_fd)
                     except ValueError:
                         import yaml
                         config_fd.seek(0)
-                        for entry in yaml.safe_load(config_fd).items():
-                            domainconfigs.append(parse_config_entry(entry, globalconfig, runtimeconfig))
+                        data = yaml.safe_load(config_fd)
+                    if isinstance(data, list):
+                        # Handle newer config in list format (allows for multiple entries with same domains)
+                        entries = list()
+                        for element in data:
+                            entries += element.items()
+                    else:
+                        # Handle older config format with just one entry per same domain set
+                        entries = data.items()
+                    for entry in entries:
+                        domainconfigs.append(parse_config_entry(entry, globalconfig, runtimeconfig))
 
     # Define a fallback authority from global configuration / defaults
     runtimeconfig['fallback_authority'] = parse_authority([], globalconfig, runtimeconfig)
 
     return runtimeconfig, domainconfigs
+
+
+if __name__ == '__main__':
+    # Simple configuration load test and output
+    from pprint import pprint
+    pprint(load())
```

### Comparing `acertmgr-1.0.4/acertmgr/authority/acme.py` & `acertmgr-1.0.5/acertmgr/authority/acme.py`

 * *Files identical despite different names*

### Comparing `acertmgr-1.0.4/acertmgr/authority/__init__.py` & `acertmgr-1.0.5/acertmgr/authority/__init__.py`

 * *Files identical despite different names*

### Comparing `acertmgr-1.0.4/acertmgr/authority/v2.py` & `acertmgr-1.0.5/acertmgr/authority/v2.py`

 * *Files identical despite different names*

### Comparing `acertmgr-1.0.4/acertmgr/authority/v1.py` & `acertmgr-1.0.5/acertmgr/authority/v1.py`

 * *Files identical despite different names*

