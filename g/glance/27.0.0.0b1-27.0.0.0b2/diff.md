# Comparing `tmp/glance-27.0.0.0b1.tar.gz` & `tmp/glance-27.0.0.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glance-27.0.0.0b1.tar", last modified: Fri May 12 14:41:11 2023, max compression
+gzip compressed data, was "glance-27.0.0.0b2.tar", last modified: Thu Jul 13 12:16:37 2023, max compression
```

## Comparing `glance-27.0.0.0b1.tar` & `glance-27.0.0.0b2.tar`

### file list

```diff
@@ -1,975 +1,976 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:41:11.049159 glance-27.0.0.0b1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       89 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/.coveragerc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1207 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/.mailmap
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/.stestr.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14352 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/.zuul.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    25701 2023-05-12 14:41:10.000000 glance-27.0.0.0b1/AUTHORS
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      588 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/CONTRIBUTING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   225773 2023-05-12 14:41:09.000000 glance-27.0.0.0b1/ChangeLog
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      786 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/HACKING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/LICENSE
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3272 2023-05-12 14:41:11.049159 glance-27.0.0.0b1/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1955 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:41:10.849062 glance-27.0.0.0b1/api-ref/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:41:10.869072 glance-27.0.0.0b1/api-ref/source/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6702 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/api-ref/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      569 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/api-ref/source/heading-level-guide.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      845 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/api-ref/source/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:41:10.877076 glance-27.0.0.0b1/api-ref/source/v2/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      742 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/api-ref/source/v2/cache-manage-parameters.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1516 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/api-ref/source/v2/cache-manage.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1594 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/api-ref/source/v2/discovery-parameters.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3045 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/api-ref/source/v2/discovery.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4662 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/api-ref/source/v2/images-data.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    22513 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/api-ref/source/v2/images-images-v2.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13388 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/api-ref/source/v2/images-import.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1353 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/api-ref/source/v2/images-parameters-descriptions.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    21246 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/api-ref/source/v2/images-parameters.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2688 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/api-ref/source/v2/images-schemas.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9338 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/api-ref/source/v2/images-sharing-v2.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      803 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/api-ref/source/v2/images-tags.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1155 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/api-ref/source/v2/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2776 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/api-ref/source/v2/metadefs-index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6577 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/api-ref/source/v2/metadefs-namespaces-objects.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6374 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/api-ref/source/v2/metadefs-namespaces-properties.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5884 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/api-ref/source/v2/metadefs-namespaces-tags.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8772 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/api-ref/source/v2/metadefs-namespaces.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13711 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/api-ref/source/v2/metadefs-parameters.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3729 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/api-ref/source/v2/metadefs-resourcetypes.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6920 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/api-ref/source/v2/metadefs-schemas.inc
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:41:10.893084 glance-27.0.0.0b1/api-ref/source/v2/samples/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      390 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/api-ref/source/v2/samples/cache-list-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      133 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/api-ref/source/v2/samples/image-create-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      726 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/api-ref/source/v2/samples/image-create-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      893 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/api-ref/source/v2/samples/image-details-deactivate-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      174 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/api-ref/source/v2/samples/image-import-c-i-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      151 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/api-ref/source/v2/samples/image-import-g-d-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      189 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/api-ref/source/v2/samples/image-import-gd-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      206 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/api-ref/source/v2/samples/image-import-w-d-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      196 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/api-ref/source/v2/samples/image-info-import-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       53 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/api-ref/source/v2/samples/image-member-create-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      257 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/api-ref/source/v2/samples/image-member-create-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      257 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/api-ref/source/v2/samples/image-member-details-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       29 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/api-ref/source/v2/samples/image-member-update-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      258 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/api-ref/source/v2/samples/image-member-update-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      662 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/api-ref/source/v2/samples/image-members-list-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      888 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/api-ref/source/v2/samples/image-show-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      988 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/api-ref/source/v2/samples/image-tasks-show-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      229 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/api-ref/source/v2/samples/image-update-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      910 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/api-ref/source/v2/samples/image-update-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2246 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/api-ref/source/v2/samples/images-list-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      220 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/api-ref/source/v2/samples/metadef-namespace-create-request-simple.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1102 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/api-ref/source/v2/samples/metadef-namespace-create-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      470 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/api-ref/source/v2/samples/metadef-namespace-create-response-simple.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1213 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/api-ref/source/v2/samples/metadef-namespace-create-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1173 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/api-ref/source/v2/samples/metadef-namespace-details-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1179 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/api-ref/source/v2/samples/metadef-namespace-details-with-rt-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      333 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/api-ref/source/v2/samples/metadef-namespace-update-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      577 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/api-ref/source/v2/samples/metadef-namespace-update-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3629 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/api-ref/source/v2/samples/metadef-namespaces-list-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1634 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/api-ref/source/v2/samples/metadef-object-create-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1840 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/api-ref/source/v2/samples/metadef-object-create-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1840 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/api-ref/source/v2/samples/metadef-object-details-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      635 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/api-ref/source/v2/samples/metadef-object-update-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      841 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/api-ref/source/v2/samples/metadef-object-update-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7469 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/api-ref/source/v2/samples/metadef-objects-list-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4387 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/api-ref/source/v2/samples/metadef-properties-list-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      577 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/api-ref/source/v2/samples/metadef-property-create-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      577 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/api-ref/source/v2/samples/metadef-property-create-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      577 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/api-ref/source/v2/samples/metadef-property-details-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      577 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/api-ref/source/v2/samples/metadef-property-update-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      577 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/api-ref/source/v2/samples/metadef-property-update-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      176 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/api-ref/source/v2/samples/metadef-resource-type-assoc-create-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      324 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/api-ref/source/v2/samples/metadef-resource-type-assoc-list-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       92 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/api-ref/source/v2/samples/metadef-resource-type-create-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      841 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/api-ref/source/v2/samples/metadef-resource-types-list-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      119 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/api-ref/source/v2/samples/metadef-tag-create-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      114 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/api-ref/source/v2/samples/metadef-tag-details-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       31 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/api-ref/source/v2/samples/metadef-tag-update-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      115 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/api-ref/source/v2/samples/metadef-tag-update-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      188 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/api-ref/source/v2/samples/metadef-tags-create-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      188 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/api-ref/source/v2/samples/metadef-tags-create-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      188 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/api-ref/source/v2/samples/metadef-tags-list-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1033 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/api-ref/source/v2/samples/schemas-image-member-show-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1742 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/api-ref/source/v2/samples/schemas-image-members-list-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7811 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/api-ref/source/v2/samples/schemas-image-show-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11491 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/api-ref/source/v2/samples/schemas-images-list-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7210 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/api-ref/source/v2/samples/schemas-metadef-namespace-show-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9122 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/api-ref/source/v2/samples/schemas-metadef-namespaces-list-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5035 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/api-ref/source/v2/samples/schemas-metadef-object-show-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6101 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/api-ref/source/v2/samples/schemas-metadef-objects-list-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4593 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/api-ref/source/v2/samples/schemas-metadef-properties-list-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2861 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/api-ref/source/v2/samples/schemas-metadef-property-show-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1593 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/api-ref/source/v2/samples/schemas-metadef-resource-type-association-show-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2625 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/api-ref/source/v2/samples/schemas-metadef-resource-type-associations-list-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      602 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/api-ref/source/v2/samples/schemas-metadef-tag-show-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1458 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/api-ref/source/v2/samples/schemas-metadef-tags-list-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2072 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/api-ref/source/v2/samples/schemas-task-show-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2455 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/api-ref/source/v2/samples/schemas-tasks-list-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1252 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/api-ref/source/v2/samples/stores-list-detail-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      589 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/api-ref/source/v2/samples/stores-list-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      278 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/api-ref/source/v2/samples/task-create-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      621 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/api-ref/source/v2/samples/task-create-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      696 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/api-ref/source/v2/samples/task-show-failure-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      589 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/api-ref/source/v2/samples/task-show-processing-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      714 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/api-ref/source/v2/samples/task-show-success-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      911 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/api-ref/source/v2/samples/tasks-list-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      391 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/api-ref/source/v2/samples/usage-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      610 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/api-ref/source/v2/stores.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5095 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/api-ref/source/v2/tasks-parameters.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1345 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/api-ref/source/v2/tasks-schemas.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3542 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/api-ref/source/v2/tasks.inc
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:41:10.893084 glance-27.0.0.0b1/api-ref/source/versions/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3668 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/api-ref/source/versions/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:41:10.893084 glance-27.0.0.0b1/api-ref/source/versions/samples/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4454 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/api-ref/source/versions/samples/image-versions-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      798 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/api-ref/source/versions/versions.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1200 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/bindep.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:41:10.893084 glance-27.0.0.0b1/doc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      468 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/doc/requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:41:10.893084 glance-27.0.0.0b1/doc/source/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:41:10.893084 glance-27.0.0.0b1/doc/source/_extra/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3326 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/doc/source/_extra/.htaccess
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:41:10.893084 glance-27.0.0.0b1/doc/source/_static/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/doc/source/_static/.placeholder
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:41:10.901088 glance-27.0.0.0b1/doc/source/admin/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3142 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/doc/source/admin/apache-httpd.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3779 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/doc/source/admin/authentication.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9196 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/doc/source/admin/cache.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8121 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/doc/source/admin/controllingservers.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2159 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/doc/source/admin/db-sqlalchemy-migrate.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9263 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/doc/source/admin/db.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      831 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/doc/source/admin/flows.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      479 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/doc/source/admin/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    31604 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/doc/source/admin/interoperable-image-import.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13329 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/doc/source/admin/manage-images.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7589 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/doc/source/admin/multistores.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5366 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/doc/source/admin/notifications.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1314 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/doc/source/admin/os_hash_algo.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6217 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/doc/source/admin/policies.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3824 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/doc/source/admin/property-protections.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7509 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/doc/source/admin/quotas.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3479 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/doc/source/admin/requirements.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5569 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/doc/source/admin/rollingupgrades.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7053 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/doc/source/admin/tasks.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16419 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/doc/source/admin/troubleshooting.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    26318 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/doc/source/admin/useful-image-properties.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8112 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/doc/source/admin/zero-downtime-db-upgrade.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:41:10.901088 glance-27.0.0.0b1/doc/source/cli/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      212 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/doc/source/cli/footer.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2295 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/doc/source/cli/general_options.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      500 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/doc/source/cli/glanceapi.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      992 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/doc/source/cli/glancecachecleaner.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1767 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/doc/source/cli/glancecachemanage.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      558 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/doc/source/cli/glancecacheprefetcher.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      619 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/doc/source/cli/glancecachepruner.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1146 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/doc/source/cli/glancecontrol.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3961 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/doc/source/cli/glancemanage.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2017 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/doc/source/cli/glancereplicator.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5295 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/doc/source/cli/glancescrubber.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2416 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/doc/source/cli/glancestatus.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      195 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/doc/source/cli/header.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/doc/source/cli/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      734 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/doc/source/cli/openstack_options.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5557 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/doc/source/conf.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:41:10.905089 glance-27.0.0.0b1/doc/source/configuration/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    60955 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/doc/source/configuration/configuring.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      148 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/doc/source/configuration/glance_api.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      158 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/doc/source/configuration/glance_cache.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      163 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/doc/source/configuration/glance_manage.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      268 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/doc/source/configuration/glance_policy.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      173 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/doc/source/configuration/glance_scrubber.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      414 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/doc/source/configuration/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1792 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/doc/source/configuration/sample-configuration.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:41:10.909091 glance-27.0.0.0b1/doc/source/contributor/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3839 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/doc/source/contributor/architecture.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3275 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/doc/source/contributor/blueprints.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8712 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/doc/source/contributor/contributing.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5869 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/doc/source/contributor/core_reviewer_guidelines.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10493 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/doc/source/contributor/database_architecture.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13229 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/doc/source/contributor/database_migrations.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3780 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/doc/source/contributor/documentation.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4965 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/doc/source/contributor/domain_implementation.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10110 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/doc/source/contributor/domain_model.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1839 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/doc/source/contributor/gerrit.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4297 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/doc/source/contributor/glance-groups.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1453 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/doc/source/contributor/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4650 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/doc/source/contributor/minor-code-changes.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2918 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/doc/source/contributor/refreshing-configs.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12244 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/doc/source/contributor/release-cpl.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2487 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/doc/source/contributor/release-notes.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5452 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/doc/source/contributor/releasecycle.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       84 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/doc/source/deprecation-note.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   120177 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/doc/source/glossary.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:41:10.909091 glance-27.0.0.0b1/doc/source/images/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    48303 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/doc/source/images/architecture.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   108006 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/doc/source/images/glance_db.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    32606 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/doc/source/images/glance_layers.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   250651 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/doc/source/images/image_status_transition.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    28449 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/doc/source/images/instance-life-1.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    39847 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/doc/source/images/instance-life-2.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    30176 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/doc/source/images/instance-life-3.png
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:41:10.913093 glance-27.0.0.0b1/doc/source/images_src/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    57938 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/doc/source/images_src/architecture.graphml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12358 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/doc/source/images_src/glance_db.graphml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    21398 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/doc/source/images_src/glance_layers.graphml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2040 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/doc/source/images_src/image_status_transition.dot
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4167 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/doc/source/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:41:10.913093 glance-27.0.0.0b1/doc/source/install/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1152 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/doc/source/install/configure-quotas.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3378 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/doc/source/install/get-started.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      774 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/doc/source/install/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8181 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/doc/source/install/install-debian.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8543 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/doc/source/install/install-obs.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8311 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/doc/source/install/install-rdo.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8170 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/doc/source/install/install-ubuntu.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      272 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/doc/source/install/install.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      310 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/doc/source/install/note_configuration_vary_by_distribution.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3277 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/doc/source/install/register-quotas.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4183 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/doc/source/install/verify.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:41:10.917095 glance-27.0.0.0b1/doc/source/user/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3511 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/doc/source/user/common-image-properties.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6185 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/doc/source/user/formats.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    34733 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/doc/source/user/glanceapi.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1090 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/doc/source/user/glanceclient.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    19470 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/doc/source/user/glancemetadefcatalogapi.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1036 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/doc/source/user/identifiers.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      256 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/doc/source/user/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8930 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/doc/source/user/metadefs-concepts.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4682 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/doc/source/user/os_hash_algo.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6281 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/doc/source/user/signature.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6027 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/doc/source/user/statuses.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:41:10.917095 glance-27.0.0.0b1/doc/test/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4624 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/doc/test/redirect-tests.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:41:10.921097 glance-27.0.0.0b1/etc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2711 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/etc/glance-api-paste.ini
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   204249 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/etc/glance-api.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    82774 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/etc/glance-cache.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8409 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/etc/glance-image-import.conf.sample
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10401 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/etc/glance-manage.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       66 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/etc/glance-policy-generator.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    85943 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/etc/glance-scrubber.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      606 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/etc/glance-swift.conf.sample
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:41:10.925099 glance-27.0.0.0b1/etc/metadefs/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      270 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/etc/metadefs/README
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5190 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/etc/metadefs/cim-processor-allocation-setting-data.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7051 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/etc/metadefs/cim-resource-allocation-setting-data.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5168 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/etc/metadefs/cim-storage-allocation-setting-data.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5239 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/etc/metadefs/cim-virtual-system-setting-data.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1090 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/etc/metadefs/compute-aggr-disk-filter.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1043 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/etc/metadefs/compute-aggr-iops-filter.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      897 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/etc/metadefs/compute-aggr-num-instances.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      737 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/etc/metadefs/compute-cpu-mode.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1295 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/etc/metadefs/compute-cpu-pinning.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1145 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/etc/metadefs/compute-guest-memory-backing.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      944 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/etc/metadefs/compute-guest-shutdown.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9206 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/etc/metadefs/compute-host-capabilities.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2269 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/etc/metadefs/compute-hypervisor.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1861 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/etc/metadefs/compute-instance-data.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7583 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/etc/metadefs/compute-libvirt-image.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1985 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/etc/metadefs/compute-libvirt.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7204 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/etc/metadefs/compute-quota.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1052 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/etc/metadefs/compute-randomgen.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2004 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/etc/metadefs/compute-vcputopology.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1773 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/etc/metadefs/compute-vmware-flavor.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1644 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/etc/metadefs/compute-vmware-quota-flavor.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8441 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/etc/metadefs/compute-vmware.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      799 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/etc/metadefs/compute-vtpm-hw.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1071 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/etc/metadefs/compute-vtpm.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1430 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/etc/metadefs/compute-watchdog.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      998 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/etc/metadefs/compute-xenapi.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3455 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/etc/metadefs/glance-common-image-props.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1687 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/etc/metadefs/image-signature-verification.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1314 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/etc/metadefs/operating-system.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18731 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/etc/metadefs/software-databases.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5252 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/etc/metadefs/software-runtimes.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5772 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/etc/metadefs/software-webservers.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1100 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/etc/metadefs/storage-volume-type.json
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:41:10.925099 glance-27.0.0.0b1/etc/oslo-config-generator/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      527 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/etc/oslo-config-generator/glance-api.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      185 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/etc/oslo-config-generator/glance-cache.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       97 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/etc/oslo-config-generator/glance-image-import.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      137 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/etc/oslo-config-generator/glance-manage.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      240 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/etc/oslo-config-generator/glance-scrubber.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/etc/ovf-metadata.json.sample
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1402 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/etc/property-protections-policies.conf.sample
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1101 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/etc/property-protections-roles.conf.sample
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2145 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/etc/schema-image.json
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:41:10.929101 glance-27.0.0.0b1/glance/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:41:10.933103 glance-27.0.0.0b1/glance/api/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      839 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/api/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8321 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/api/common.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:41:10.933103 glance-27.0.0.0b1/glance/api/middleware/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/api/middleware/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12611 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/api/middleware/cache.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3034 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/api/middleware/cache_manage.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5750 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/api/middleware/context.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2279 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/api/middleware/gzip.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4515 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/api/middleware/version_negotiation.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7339 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/api/policy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5096 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/api/property_protections.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:41:10.933103 glance-27.0.0.0b1/glance/api/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/api/v1/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1053 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/api/v1/router.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:41:10.937105 glance-27.0.0.0b1/glance/api/v2/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/api/v2/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10253 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/api/v2/cached_images.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6717 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/api/v2/discovery.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4763 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/api/v2/image_actions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    26019 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/api/v2/image_data.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    19505 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/api/v2/image_members.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4696 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/api/v2/image_tags.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    84250 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/api/v2/images.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    38032 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/api/v2/metadef_namespaces.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18163 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/api/v2/metadef_objects.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16423 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/api/v2/metadef_properties.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14015 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/api/v2/metadef_resource_types.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    19240 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/api/v2/metadef_tags.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:41:10.937105 glance-27.0.0.0b1/glance/api/v2/model/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/api/v2/model/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3021 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/api/v2/model/metadef_namespace.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1768 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/api/v2/model/metadef_object.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      906 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/api/v2/model/metadef_property_item_type.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2354 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/api/v2/model/metadef_property_type.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2186 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/api/v2/model/metadef_resource_type.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1139 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/api/v2/model/metadef_tag.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17869 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/api/v2/policy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    29774 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/api/v2/router.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3947 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/api/v2/schemas.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16565 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/api/v2/tasks.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4435 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/api/versions.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:41:10.941107 glance-27.0.0.0b1/glance/async_/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7077 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/async_/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:41:10.941107 glance-27.0.0.0b1/glance/async_/flows/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/async_/flows/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:41:10.941107 glance-27.0.0.0b1/glance/async_/flows/_internal_plugins/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7580 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/async_/flows/_internal_plugins/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5451 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/async_/flows/_internal_plugins/base_download.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5889 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/async_/flows/_internal_plugins/copy_image.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4711 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/async_/flows/_internal_plugins/glance_download.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3600 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/async_/flows/_internal_plugins/web_download.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    41972 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/async_/flows/api_image_import.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    20847 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/async_/flows/base_import.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5962 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/async_/flows/convert.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3550 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/async_/flows/introspect.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11075 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/async_/flows/ovf_process.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:41:10.945109 glance-27.0.0.0b1/glance/async_/flows/plugins/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1202 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/async_/flows/plugins/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7617 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/async_/flows/plugins/image_conversion.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5747 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/async_/flows/plugins/image_decompression.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2975 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/async_/flows/plugins/inject_image_metadata.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1882 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/async_/flows/plugins/no_op.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1492 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/async_/flows/plugins/plugin_opts.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7319 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/async_/taskflow_executor.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4214 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/async_/utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:41:10.945109 glance-27.0.0.0b1/glance/cmd/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/cmd/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4199 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/cmd/api.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2156 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/cmd/cache_cleaner.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17537 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/cmd/cache_manage.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2134 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/cmd/cache_prefetcher.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1753 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/cmd/cache_pruner.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13626 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/cmd/control.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    23152 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/cmd/manage.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    27453 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/cmd/replicator.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6100 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/cmd/scrubber.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2924 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/cmd/status.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:41:10.949111 glance-27.0.0.0b1/glance/common/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/common/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12068 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/common/auth.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    22672 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/common/client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    28492 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/common/config.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3208 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/common/crypt.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14512 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/common/exception.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)    25753 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/common/format_inspector.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:41:10.949111 glance-27.0.0.0b1/glance/common/location_strategy/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4768 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/common/location_strategy/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1080 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/common/location_strategy/location_order.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4352 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/common/location_strategy/store_type.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9594 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/common/property_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1354 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/common/removed_config.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:41:10.949111 glance-27.0.0.0b1/glance/common/scripts/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2439 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/common/scripts/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:41:10.949111 glance-27.0.0.0b1/glance/common/scripts/api_image_import/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/common/scripts/api_image_import/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5424 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/common/scripts/api_image_import/main.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:41:10.949111 glance-27.0.0.0b1/glance/common/scripts/image_import/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/common/scripts/image_import/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6684 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/common/scripts/image_import/main.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8395 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/common/scripts/utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9190 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/common/store_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4854 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/common/swift_store_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2890 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/common/timeutils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4550 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/common/trust_auth.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    25407 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/common/utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    47333 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/common/wsgi.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5539 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/common/wsgi_app.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2324 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/common/wsme_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3636 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/context.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:41:10.953113 glance-27.0.0.0b1/glance/db/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    35376 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/db/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2122 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/db/metadata.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1097 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/db/migration.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:41:10.953113 glance-27.0.0.0b1/glance/db/simple/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      153 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/db/simple/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    70123 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/db/simple/api.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:41:10.953113 glance-27.0.0.0b1/glance/db/sqlalchemy/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/db/sqlalchemy/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:41:10.957115 glance-27.0.0.0b1/glance/db/sqlalchemy/alembic_migrations/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       39 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/db/sqlalchemy/alembic_migrations/README
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3058 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/db/sqlalchemy/alembic_migrations/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10416 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/db/sqlalchemy/alembic_migrations/add_artifacts_tables.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8936 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/db/sqlalchemy/alembic_migrations/add_images_tables.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7878 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/db/sqlalchemy/alembic_migrations/add_metadefs_tables.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2846 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/db/sqlalchemy/alembic_migrations/add_tasks_tables.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1557 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/db/sqlalchemy/alembic_migrations/alembic.ini
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:41:10.957115 glance-27.0.0.0b1/glance/db/sqlalchemy/alembic_migrations/data_migrations/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      826 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/db/sqlalchemy/alembic_migrations/data_migrations/2023_1_migrate01_empty.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2331 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/db/sqlalchemy/alembic_migrations/data_migrations/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3938 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/db/sqlalchemy/alembic_migrations/data_migrations/ocata_migrate01_community_images.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      905 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/db/sqlalchemy/alembic_migrations/data_migrations/pike_migrate01_empty.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      823 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/db/sqlalchemy/alembic_migrations/data_migrations/queens_migrate01_empty.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      826 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/db/sqlalchemy/alembic_migrations/data_migrations/rocky_migrate01_empty.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      831 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/db/sqlalchemy/alembic_migrations/data_migrations/rocky_migrate02_empty.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2173 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/db/sqlalchemy/alembic_migrations/data_migrations/train_migrate01_backend_to_store.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      826 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/db/sqlalchemy/alembic_migrations/data_migrations/ussuri_migrate01_empty.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      826 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/db/sqlalchemy/alembic_migrations/data_migrations/wallaby_migrate01_empty.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      826 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/db/sqlalchemy/alembic_migrations/data_migrations/xena_migrate01_empty.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      826 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/db/sqlalchemy/alembic_migrations/data_migrations/yoga_migrate01_empty.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      826 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/db/sqlalchemy/alembic_migrations/data_migrations/zed_migrate01_empty.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2674 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/db/sqlalchemy/alembic_migrations/env.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      993 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/db/sqlalchemy/alembic_migrations/migrate.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      431 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/db/sqlalchemy/alembic_migrations/script.py.mako
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:41:10.961117 glance-27.0.0.0b1/glance/db/sqlalchemy/alembic_migrations/versions/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      814 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/db/sqlalchemy/alembic_migrations/versions/2023_1_contract01_empty.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      921 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/db/sqlalchemy/alembic_migrations/versions/2023_1_expand01_empty.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/db/sqlalchemy/alembic_migrations/versions/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1289 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/db/sqlalchemy/alembic_migrations/versions/liberty_initial.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1432 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/db/sqlalchemy/alembic_migrations/versions/mitaka01_add_image_created_updated_idx.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1272 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/db/sqlalchemy/alembic_migrations/versions/mitaka02_update_metadef_os_nova_server.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2355 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/db/sqlalchemy/alembic_migrations/versions/ocata_contract01_drop_is_public.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5934 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/db/sqlalchemy/alembic_migrations/versions/ocata_expand01_add_visibility.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1337 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/db/sqlalchemy/alembic_migrations/versions/pike_contract01_drop_artifacts_tables.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      887 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/db/sqlalchemy/alembic_migrations/versions/pike_expand01_empty.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      813 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/db/sqlalchemy/alembic_migrations/versions/queens_contract01_empty.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      796 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/db/sqlalchemy/alembic_migrations/versions/queens_expand01_empty.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      816 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/db/sqlalchemy/alembic_migrations/versions/rocky_contract01_empty.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      820 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/db/sqlalchemy/alembic_migrations/versions/rocky_contract02_empty.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1135 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/db/sqlalchemy/alembic_migrations/versions/rocky_expand01_add_os_hidden.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1222 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/db/sqlalchemy/alembic_migrations/versions/rocky_expand02_add_os_hash_.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      814 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/db/sqlalchemy/alembic_migrations/versions/train_contract01_empty.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      922 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/db/sqlalchemy/alembic_migrations/versions/train_expand01_empty.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      816 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/db/sqlalchemy/alembic_migrations/versions/ussuri_contract01_empty.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      923 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/db/sqlalchemy/alembic_migrations/versions/ussuri_expand01_empty.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      819 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/db/sqlalchemy/alembic_migrations/versions/wallaby_contract01_empty.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1388 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/db/sqlalchemy/alembic_migrations/versions/wallaby_expand01_add_user_imageid_requestid_to_tasks.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      814 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/db/sqlalchemy/alembic_migrations/versions/xena_contract01_empty.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      923 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/db/sqlalchemy/alembic_migrations/versions/xena_expand01_empty.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      811 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/db/sqlalchemy/alembic_migrations/versions/yoga_contract01_empty.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      920 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/db/sqlalchemy/alembic_migrations/versions/yoga_expand01_empty.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      809 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/db/sqlalchemy/alembic_migrations/versions/zed_contract01_empty.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      919 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/db/sqlalchemy/alembic_migrations/versions/zed_expand01_empty.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    82565 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/db/sqlalchemy/api.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17923 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/db/sqlalchemy/metadata.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:41:10.965119 glance-27.0.0.0b1/glance/db/sqlalchemy/metadef_api/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/db/sqlalchemy/metadef_api/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10906 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/db/sqlalchemy/metadef_api/namespace.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5734 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/db/sqlalchemy/metadef_api/object.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6085 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/db/sqlalchemy/metadef_api/property.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3635 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/db/sqlalchemy/metadef_api/resource_type.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8277 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/db/sqlalchemy/metadef_api/resource_type_association.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7798 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/db/sqlalchemy/metadef_api/tag.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      921 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/db/sqlalchemy/metadef_api/utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10581 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/db/sqlalchemy/models.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7149 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/db/sqlalchemy/models_metadef.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1486 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/db/sqlalchemy/schema.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2522 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/db/utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:41:10.965119 glance-27.0.0.0b1/glance/domain/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    23897 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/domain/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    20262 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/domain/proxy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8814 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/gateway.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:41:10.965119 glance-27.0.0.0b1/glance/hacking/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/hacking/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4119 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/hacking/checks.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4519 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/housekeeping.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1351 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/i18n.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:41:10.965119 glance-27.0.0.0b1/glance/image_cache/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16440 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/image_cache/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      733 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/image_cache/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      797 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/image_cache/cleaner.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4433 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/image_cache/client.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:41:10.969121 glance-27.0.0.0b1/glance/image_cache/drivers/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/image_cache/drivers/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6566 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/image_cache/drivers/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17261 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/image_cache/drivers/sqlite.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16698 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/image_cache/drivers/xattr.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3455 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/image_cache/prefetcher.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      782 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/image_cache/pruner.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:41:10.861068 glance-27.0.0.0b1/glance/locale/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:41:10.857066 glance-27.0.0.0b1/glance/locale/de/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:41:10.969121 glance-27.0.0.0b1/glance/locale/de/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    59075 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/locale/de/LC_MESSAGES/glance.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:41:10.857066 glance-27.0.0.0b1/glance/locale/en_GB/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:41:10.969121 glance-27.0.0.0b1/glance/locale/en_GB/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   168210 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/locale/en_GB/LC_MESSAGES/glance.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:41:10.857066 glance-27.0.0.0b1/glance/locale/es/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:41:10.969121 glance-27.0.0.0b1/glance/locale/es/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    53588 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/locale/es/LC_MESSAGES/glance.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:41:10.857066 glance-27.0.0.0b1/glance/locale/fr/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:41:10.969121 glance-27.0.0.0b1/glance/locale/fr/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    54628 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/locale/fr/LC_MESSAGES/glance.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:41:10.857066 glance-27.0.0.0b1/glance/locale/it/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:41:10.969121 glance-27.0.0.0b1/glance/locale/it/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    53703 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/locale/it/LC_MESSAGES/glance.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:41:10.857066 glance-27.0.0.0b1/glance/locale/ja/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:41:10.969121 glance-27.0.0.0b1/glance/locale/ja/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    66528 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/locale/ja/LC_MESSAGES/glance.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:41:10.861068 glance-27.0.0.0b1/glance/locale/ko_KR/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:41:10.969121 glance-27.0.0.0b1/glance/locale/ko_KR/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    56596 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/locale/ko_KR/LC_MESSAGES/glance.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:41:10.861068 glance-27.0.0.0b1/glance/locale/pt_BR/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:41:10.969121 glance-27.0.0.0b1/glance/locale/pt_BR/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    53118 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/locale/pt_BR/LC_MESSAGES/glance.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:41:10.861068 glance-27.0.0.0b1/glance/locale/ru/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:41:10.969121 glance-27.0.0.0b1/glance/locale/ru/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    65007 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/locale/ru/LC_MESSAGES/glance.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:41:10.861068 glance-27.0.0.0b1/glance/locale/tr_TR/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:41:10.973123 glance-27.0.0.0b1/glance/locale/tr_TR/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    44846 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/locale/tr_TR/LC_MESSAGES/glance.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:41:10.861068 glance-27.0.0.0b1/glance/locale/zh_CN/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:41:10.973123 glance-27.0.0.0b1/glance/locale/zh_CN/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    49820 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/locale/zh_CN/LC_MESSAGES/glance.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:41:10.861068 glance-27.0.0.0b1/glance/locale/zh_TW/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:41:10.973123 glance-27.0.0.0b1/glance/locale/zh_TW/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    48320 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/locale/zh_TW/LC_MESSAGES/glance.po
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    25816 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/location.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    32705 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/notifier.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4822 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/opts.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:41:10.973123 glance-27.0.0.0b1/glance/policies/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1027 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/policies/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5231 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/policies/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2434 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/policies/cache.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1053 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/policies/discovery.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11416 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/policies/image.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12900 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/policies/metadef.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4471 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/policies/tasks.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:41:10.973123 glance-27.0.0.0b1/glance/quota/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14945 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/quota/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6472 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/quota/keystone.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8048 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/schema.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15248 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/scrubber.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:41:10.973123 glance-27.0.0.0b1/glance/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1861 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:41:10.977125 glance-27.0.0.0b1/glance/tests/etc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      516 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/etc/glance-swift.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      214 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/etc/policy.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      923 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/etc/property-protections-policies.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1467 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/etc/property-protections.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        3 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/etc/schema-image.json
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:41:10.977125 glance-27.0.0.0b1/glance/tests/functional/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    70237 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/functional/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:41:10.981127 glance-27.0.0.0b1/glance/tests/functional/db/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1077 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/functional/db/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   116440 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/functional/db/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    32013 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/functional/db/base_metadef.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:41:10.981127 glance-27.0.0.0b1/glance/tests/functional/db/migrations/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/functional/db/migrations/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1862 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/functional/db/migrations/test_mitaka01.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2752 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/functional/db/migrations/test_mitaka02.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2884 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/functional/db/migrations/test_ocata_contract01.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7914 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/functional/db/migrations/test_ocata_expand01.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7733 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/functional/db/migrations/test_ocata_migrate01.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1957 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/functional/db/migrations/test_pike_contract01.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1799 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/functional/db/migrations/test_pike_expand01.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1009 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/functional/db/migrations/test_pike_migrate01.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1650 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/functional/db/migrations/test_rocky_expand01.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1749 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/functional/db/migrations/test_rocky_expand02.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5578 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/functional/db/migrations/test_train_migrate01.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2346 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/functional/db/migrations/test_wallaby_expand01.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11099 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/functional/db/test_migrations.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17729 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/functional/db/test_sqlalchemy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6831 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/functional/ft_utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:41:10.985129 glance-27.0.0.0b1/glance/tests/functional/serial/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/functional/serial/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16797 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/functional/serial/test_scrubber.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2859 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/functional/store_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6839 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/functional/test_api.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16376 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/functional/test_cache_middleware.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4522 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/functional/test_client_exceptions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5036 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/functional/test_client_redirects.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3750 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/functional/test_cors_middleware.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7257 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/functional/test_glance_manage.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1689 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/functional/test_gzip_middleware.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1798 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/functional/test_healthcheck_middleware.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2790 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/functional/test_logging.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5833 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/functional/test_reload.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1348 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/functional/test_sqlite.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7126 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/functional/test_wsgi.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:41:10.989131 glance-27.0.0.0b1/glance/tests/functional/v2/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/functional/v2/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2481 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/functional/v2/metadef_base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14754 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/functional/v2/test_cache_api.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8759 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/functional/v2/test_cache_api_policy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6175 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/functional/v2/test_discovery.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   320466 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/functional/v2/test_images.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    40391 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/functional/v2/test_images_api_policy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9095 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/functional/v2/test_images_import_locking.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12996 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/functional/v2/test_legacy_update_cinder_store.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9384 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/functional/v2/test_member_api_policy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    31238 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/functional/v2/test_metadef_namespace_api_policy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18312 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/functional/v2/test_metadef_namespaces.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12372 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/functional/v2/test_metadef_object_api_policy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18926 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/functional/v2/test_metadef_objects.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16330 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/functional/v2/test_metadef_properties.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12598 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/functional/v2/test_metadef_property_api_policy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10282 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/functional/v2/test_metadef_resourcetype_api_policy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11533 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/functional/v2/test_metadef_resourcetypes.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14844 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/functional/v2/test_metadef_tag_api_policy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16401 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/functional/v2/test_metadef_tags.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2430 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/functional/v2/test_schemas.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4906 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/functional/v2/test_tasks.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3995 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/functional/v2/test_tasks_api_policy.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:41:10.989131 glance-27.0.0.0b1/glance/tests/integration/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/integration/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:41:10.989131 glance-27.0.0.0b1/glance/tests/integration/v2/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/integration/v2/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5707 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/integration/v2/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5408 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/integration/v2/test_property_quota_violations.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    20800 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/integration/v2/test_tasks_api.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4104 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/stubs.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4171 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/test_hacking.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:41:10.997135 glance-27.0.0.0b1/glance/tests/unit/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/unit/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:41:10.997135 glance-27.0.0.0b1/glance/tests/unit/api/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/unit/api/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:41:10.997135 glance-27.0.0.0b1/glance/tests/unit/api/middleware/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/unit/api/middleware/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6390 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/unit/api/middleware/test_cache_manage.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9192 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/unit/api/test_cmd.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5882 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/unit/api/test_common.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14130 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/unit/api/test_property_protections.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:41:10.997135 glance-27.0.0.0b1/glance/tests/unit/async_/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/unit/async_/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:41:11.001137 glance-27.0.0.0b1/glance/tests/unit/async_/flows/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/unit/async_/flows/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:41:11.001137 glance-27.0.0.0b1/glance/tests/unit/async_/flows/plugins/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/unit/async_/flows/plugins/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15047 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/unit/async_/flows/plugins/test_image_conversion.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4986 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/unit/async_/flows/plugins/test_inject_image_metadata.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    59084 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/unit/async_/flows/test_api_image_import.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8957 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/unit/async_/flows/test_base_download.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8260 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/unit/async_/flows/test_convert.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9323 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/unit/async_/flows/test_copy_image.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7858 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/unit/async_/flows/test_glance_download.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18116 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/unit/async_/flows/test_import.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4801 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/unit/async_/flows/test_introspect.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7116 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/unit/async_/flows/test_ovf_process.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6610 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/unit/async_/flows/test_web_download.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12007 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/unit/async_/test_async.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6448 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/unit/async_/test_taskflow_executor.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2968 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/unit/async_/test_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6263 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/unit/base.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:41:11.001137 glance-27.0.0.0b1/glance/tests/unit/cmd/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/unit/cmd/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3054 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/unit/cmd/test_status.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:41:11.005138 glance-27.0.0.0b1/glance/tests/unit/common/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/unit/common/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:41:11.005138 glance-27.0.0.0b1/glance/tests/unit/common/scripts/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/unit/common/scripts/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:41:11.005138 glance-27.0.0.0b1/glance/tests/unit/common/scripts/image_import/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/unit/common/scripts/image_import/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6491 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/unit/common/scripts/image_import/test_main.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8539 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/unit/common/scripts/test_scripts_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2442 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/unit/common/test_client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4355 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/unit/common/test_config.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2060 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/unit/common/test_exception.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15011 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/unit/common/test_format_inspector.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8449 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/unit/common/test_location_strategy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    24239 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/unit/common/test_property_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1456 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/unit/common/test_scripts.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3682 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/unit/common/test_swift_store_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8765 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/unit/common/test_timeutils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    32837 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/unit/common/test_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    33403 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/unit/common/test_wsgi.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6569 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/unit/common/test_wsgi_app.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3150 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/unit/fake_rados.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6211 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/unit/fixtures.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:41:11.005138 glance-27.0.0.0b1/glance/tests/unit/image_cache/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/unit/image_cache/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:41:11.005138 glance-27.0.0.0b1/glance/tests/unit/image_cache/drivers/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/unit/image_cache/drivers/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1234 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/unit/image_cache/drivers/test_sqlite.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:41:11.005138 glance-27.0.0.0b1/glance/tests/unit/keymgr/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/unit/keymgr/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      901 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/unit/keymgr/fake.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    20879 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/unit/test_auth.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4007 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/unit/test_cache_manage.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17310 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/unit/test_cache_middleware.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17069 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/unit/test_cached_images.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8667 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/unit/test_context.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6238 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/unit/test_context_middleware.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8656 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/unit/test_data_migration_framework.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    41382 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/unit/test_db.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    24028 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/unit/test_db_metadef.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    24646 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/unit/test_domain.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11419 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/unit/test_domain_proxy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7533 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/unit/test_gateway.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4556 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/unit/test_glance_manage.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    23570 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/unit/test_glance_replicator.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10568 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/unit/test_housekeeping.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    23350 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/unit/test_image_cache.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    33977 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/unit/test_manage.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2784 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/unit/test_misc.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    34473 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/unit/test_notifier.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18800 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/unit/test_policy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    37417 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/unit/test_quota.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5937 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/unit/test_schema.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6931 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/unit/test_scrubber.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    48017 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/unit/test_store_image.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3218 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/unit/test_store_location.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1312 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/unit/test_test_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17889 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/unit/test_versions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12410 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/unit/utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:41:11.009141 glance-27.0.0.0b1/glance/tests/unit/v2/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/unit/v2/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6387 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/unit/v2/test_cache_management_api.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1765 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/unit/v2/test_discovery_image_import.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4930 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/unit/v2/test_discovery_stores.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6487 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/unit/v2/test_image_actions_resource.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    48624 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/unit/v2/test_image_data_resource.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    24562 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/unit/v2/test_image_members_resource.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4188 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/unit/v2/test_image_tags_resource.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   286556 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/unit/v2/test_images_resource.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   100689 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/unit/v2/test_metadef_resources.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3167 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/unit/v2/test_schemas_resource.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    38857 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/unit/v2/test_tasks_resource.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    38246 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/unit/v2/test_v2_policy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    25420 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:41:11.009141 glance-27.0.0.0b1/glance/tests/var/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1285 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/var/ca.crt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1704 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/var/ca.key
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5518 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/var/certificate.crt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3243 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/var/privatekey.key
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10240 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/var/testserver-bad-ovf.ova
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    20480 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/var/testserver-no-disk.ova
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10240 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/var/testserver-no-ovf.ova
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   164385 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/var/testserver-not-tar.ova
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    20480 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/tests/var/testserver.ova
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      731 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/glance/version.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:41:10.929101 glance-27.0.0.0b1/glance.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3272 2023-05-12 14:41:10.000000 glance-27.0.0.0b1/glance.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    39213 2023-05-12 14:41:10.000000 glance-27.0.0.0b1/glance.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-05-12 14:41:10.000000 glance-27.0.0.0b1/glance.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2147 2023-05-12 14:41:10.000000 glance-27.0.0.0b1/glance.egg-info/entry_points.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-05-12 14:41:10.000000 glance-27.0.0.0b1/glance.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       47 2023-05-12 14:41:10.000000 glance-27.0.0.0b1/glance.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      808 2023-05-12 14:41:10.000000 glance-27.0.0.0b1/glance.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        7 2023-05-12 14:41:10.000000 glance-27.0.0.0b1/glance.egg-info/top_level.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:41:11.013142 glance-27.0.0.0b1/httpd/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       91 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/httpd/README
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      388 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/httpd/glance-api-uwsgi.ini
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       93 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/httpd/uwsgi-glance-api.conf
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:41:11.013142 glance-27.0.0.0b1/playbooks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       40 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/playbooks/enable-fips.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      803 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/playbooks/post-check-metadata-injection.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:41:11.013142 glance-27.0.0.0b1/rally-jobs/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1048 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/rally-jobs/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:41:11.013142 glance-27.0.0.0b1/rally-jobs/extra/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      172 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/rally-jobs/extra/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/rally-jobs/extra/fake.img
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      979 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/rally-jobs/glance.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:41:11.013142 glance-27.0.0.0b1/rally-jobs/plugins/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      394 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/rally-jobs/plugins/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:41:10.865070 glance-27.0.0.0b1/releasenotes/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:41:11.041155 glance-27.0.0.0b1/releasenotes/notes/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/releasenotes/notes/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      407 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/releasenotes/notes/Prevent-removing-last-image-location-d5ee3e00efe14f34.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3197 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/releasenotes/notes/Stein-reno-rc1-0a03f8394934a2e7.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      756 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/releasenotes/notes/Train-milestone3-be5520106a182fa0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      117 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/releasenotes/notes/add-all-visibility-image-filter-ea2f3948ff778fe3.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      180 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/releasenotes/notes/add-cli-and-cache-opts-902f28d65c8fb827.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3422 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/releasenotes/notes/add-compressed-format-185e537187a202bd.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      153 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/releasenotes/notes/add-cpu-thread-pinning-metadata-09b1866b875c4647.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      503 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/releasenotes/notes/add-description-common-image-property-95ab1139d41579d2.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      489 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/releasenotes/notes/add-glance-download-method-be6d9e927b8b0a43.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      394 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/releasenotes/notes/add-ploop-format-fdd583849504ab15.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      511 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/releasenotes/notes/add-processlimits-to-qemu-img-c215f5d90f741d8a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      385 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/releasenotes/notes/add-vhdx-format-2be99354ad320cca.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       90 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/releasenotes/notes/add_capability_to_purge_all_deleted_rows-7b3b9b767669b1a5.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      530 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/releasenotes/notes/add_policy_enforcement_for_metadef_delete_apis-95d2b16cc444840a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      444 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/releasenotes/notes/added-quota-usage-api-f1914054132f2021.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      169 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/releasenotes/notes/added-store-detail-api-215810aa85dfbb99.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1947 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/releasenotes/notes/alembic-migrations-902b31edae7a5d7d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      632 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/releasenotes/notes/antelope-milestone-2-d89e39412f9c0334.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      954 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/releasenotes/notes/antelope-milestone-3-b9a4f7fdba31f628.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2905 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/releasenotes/notes/api-2-6-current-9eeb83b7ecc0a562.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      651 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/releasenotes/notes/api-2.16-8417b1e23322fedb.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1462 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/releasenotes/notes/api-minor-ver-bump-2-6-aa3591fc58f08055.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      926 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/releasenotes/notes/api-minor-version-bump-bbd69dc457fc731c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/releasenotes/notes/bobcat-milestone-1-releasenotes-2d109105530877d6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2223 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/releasenotes/notes/bp-barbican-secret-deletion-support-40cffa5ffa33447e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1721 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/releasenotes/notes/bp-inject-image-metadata-0a08af539bcce7f2.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      373 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/releasenotes/notes/bp-mitigate-ossn-0075-c0e74e60d86d8ea2.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      450 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/releasenotes/notes/bp-upgrade-checks-b3272c3ddb4e8cf7.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      515 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/releasenotes/notes/bug-1537903-54b2822eac6cfc09.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      206 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/releasenotes/notes/bug-1593177-8ef35458d29ec93c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      400 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/releasenotes/notes/bug-1719252-name-validation-443a2e2a36be2cec.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      161 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/releasenotes/notes/bug-1861334-ebc2026b85675d47.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      197 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/releasenotes/notes/bug-1881958-d0e16538f3c0ffaa.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      212 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/releasenotes/notes/bug-1979699-70182ec2aead0383.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      539 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/releasenotes/notes/bug-1980049-623d2eb0fa074136.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      436 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/releasenotes/notes/bump-api-2-4-efa266aef0928e04.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      369 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/releasenotes/notes/cache-api-b806ccfb8c5d9bb6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      611 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/releasenotes/notes/cinder-store-migration-non-owner-80a2a8114d8602aa.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      447 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/releasenotes/notes/clean-up-acceptable-values-store_type_preference-39081e4045894731.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      437 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/releasenotes/notes/cleanout_registry_data-api-9d91368aed83497e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       95 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/releasenotes/notes/cleanup-enable_v2_api-9b9b467f4ae8c3b1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1450 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/releasenotes/notes/consistent-store-names-57374b9505d530d0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      706 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/releasenotes/notes/copy-existing-image-94fd0b8d24bc16a0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      434 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/releasenotes/notes/delete_from_store-a1d9b9bd5cf27546.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2952 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/releasenotes/notes/deprecate-admin_role-2f9d33ed0785d082.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      729 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/releasenotes/notes/deprecate-allow_additional_image_props-0e3b2f1ffa4e55e1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1160 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/releasenotes/notes/deprecate-checksum-a602853403e1c4a8.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      317 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/releasenotes/notes/deprecate-glance-api-opts-23bdbd1ad7625999.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1008 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/releasenotes/notes/deprecate-json-formatted-policy-file-5cb692fe889eb52b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      346 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/releasenotes/notes/deprecate-owner_is_tenant-ec8ea36a3f7e9268.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      569 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/releasenotes/notes/deprecate-registry-ff286df90df793f0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1456 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/releasenotes/notes/deprecate-show-multiple-location-9890a1e961def2f6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1146 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/releasenotes/notes/deprecate-show-multiple-location-continued-646f91b21cd771f7.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      929 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/releasenotes/notes/deprecate-show-multiple-location-continued-ussuri-16e8d9d8a59da1bc.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      887 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/releasenotes/notes/deprecate-v1-api-6c7dbefb90fd8772.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      571 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/releasenotes/notes/distributed-image-import-82cff4426731beac.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      211 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/releasenotes/notes/drop-py-2-7-863871c7bc047146.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      129 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/releasenotes/notes/drop-python-3-6-and-3-7-c6f051d5b2b40329.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      270 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/releasenotes/notes/drop-sheepdog-b55aae84807d31d9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      363 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/releasenotes/notes/drop-support-for-sqlalchemy-migrate-4bcbe7b200697586.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      465 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/releasenotes/notes/enable-enforce-scope-and-new-defaults-ef543183e6c2eabb.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      308 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/releasenotes/notes/exp-emc-mig-fix-a7e28d547ac38f9e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      304 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/releasenotes/notes/expanding-stores-details-d3aa8ebb76ad68d9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2050 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/releasenotes/notes/experimental-multi-store-d2c26f9dbb9c835b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      326 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/releasenotes/notes/fix-md-tag-create-multiple-c04756cf5155983d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      155 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/releasenotes/notes/fix_1889640-95d543629d7dadce.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      202 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/releasenotes/notes/fix_1889676-f8d302fd240c8a57.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      150 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/releasenotes/notes/fix_httpd_docs-3efff0395f96a94d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      367 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/releasenotes/notes/glance-unified-quotas-fba62fabb00379af.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2209 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/releasenotes/notes/glare-ectomy-72a1f80f306f2e3b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      500 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/releasenotes/notes/image-conversion-plugin-5aee45e1a1a5bb2b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      469 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/releasenotes/notes/image-not-found-policy-override-removed-52616c483a270bcf.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      578 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/releasenotes/notes/image-tasks-api-f21b42eab91c2079.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8505 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/releasenotes/notes/image-visibility-changes-fa5aa18dc67244c4.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      249 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/releasenotes/notes/image_decompression_plugin-5f085666aae01f29.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      377 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/releasenotes/notes/immediate-caching-image-e38055575c361d32.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1048 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/releasenotes/notes/implement-lite-spec-db-sync-check-3e2e147aec0ae82b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      642 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/releasenotes/notes/import-locking-behavior-901c691f3839fe0a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1056 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/releasenotes/notes/import-multi-stores-3e781f2878b3134d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1321 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/releasenotes/notes/improved-config-options-221c58a8c37602ba.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1827 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/releasenotes/notes/location-add-status-checks-b70db66100bc96b7.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      212 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/releasenotes/notes/lock_path_config_option-2771feaa649e4563.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      730 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/releasenotes/notes/make-task-api-admin-only-by-default-7def996262e18f7a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      347 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/releasenotes/notes/metadef-api-admin-operations-b9a2d863913b0cae.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2867 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/releasenotes/notes/multihash-081466a98601da20.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      749 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/releasenotes/notes/mutistore-support-for-scrubber-6b360394ef32774a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      805 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/releasenotes/notes/new_image_filters-c888361e6ecf495c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      871 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/releasenotes/notes/newton-1-release-065334d464f78fc5.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2494 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/releasenotes/notes/newton-bugs-06ed3727b973c271.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      151 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/releasenotes/notes/no_plugins_for_copy-image-26c0e384a368bf6a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      432 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/releasenotes/notes/os-glance-injection-disallowed-5dad244dfb071938.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      303 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/releasenotes/notes/os-glance-namespace-reserved-1fcb8a5fddca4e0f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      796 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/releasenotes/notes/oslo-log-use-stderr-changes-07f5daf3e6abdcd6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      311 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/releasenotes/notes/pending-delete-rollback-444ff94c0056bbdb.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      586 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/releasenotes/notes/pike-metadefs-changes-95b54e0bf8bbefd6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2543 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/releasenotes/notes/pike-rc-1-a5d3f6e8877b52c6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3977 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/releasenotes/notes/pike-rc-2-acc173005045e16a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1224 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/releasenotes/notes/policy-in-code-7e0c6c070d32d136.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      732 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/releasenotes/notes/policy-in-code-implications-438449a73af2893c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      713 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/releasenotes/notes/policy-refactor-xena-0cddb7f2d492cb3a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      986 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/releasenotes/notes/queens-metadefs-changes-daf02bef18d049f4.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1746 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/releasenotes/notes/queens-uwsgi-issues-4cee9e4fdf62c646.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      582 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/releasenotes/notes/range-header-request-83cf11eebf865fb1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1098 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/releasenotes/notes/rbac-updates-ba0fcb886fe4085c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      211 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/releasenotes/notes/remove-admin_role-f508754e98331fc4.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      440 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/releasenotes/notes/remove-db-downgrade-0d1cc45b97605775.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      617 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/releasenotes/notes/remove-enforce-secure-rbac-ec9a0249870460c2.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      711 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/releasenotes/notes/remove-osprofiler-paste-ini-options-c620dedc8f9728ff.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      489 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/releasenotes/notes/remove-owner_is_tenant-b30150def293effc.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      490 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/releasenotes/notes/remove-s3-driver-639c60b71761eb6f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      360 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/releasenotes/notes/remove_enable_image_import_option-ec4a859ac9a7ea7b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      796 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/releasenotes/notes/remove_native_ssl-c16d5a127b57583d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      329 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/releasenotes/notes/remove_secure_proxy_ssl_header-2a95ad48ffa471ad.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1346 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/releasenotes/notes/reordered-store-config-opts-newton-3a6575b5908c0e0f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      252 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/releasenotes/notes/replicator-token-cleanup-4a573c86f1acccc0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      863 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/releasenotes/notes/restrict_location_updates-05454bb765a8c92c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2735 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/releasenotes/notes/rethinking-filesystem-access-120bc46064b3d40a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      478 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/releasenotes/notes/rocky-metadefs-changes-cb00c006ff51b541.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1945 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/releasenotes/notes/rocky-rc-b0ea7628b7a74c96.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      394 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/releasenotes/notes/scrubber-exit-e5d77f6f1a38ffb7.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      475 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/releasenotes/notes/scrubber-refactor-73ddbd61ebbf1e86.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2674 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/releasenotes/notes/secure-rbac-project-personas-fb0d9792b9dc3783.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      368 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/releasenotes/notes/soft_delete-tasks-43ea983695faa565.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      380 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/releasenotes/notes/support-cinder-multiple-stores-eb4e6d912d549ee9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      805 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/releasenotes/notes/train-metadefs-changes-c4380754cdd13a19.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      386 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/releasenotes/notes/trust-support-registry-cfd17a6a9ab21d70.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      404 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/releasenotes/notes/update-show_multiple_locations-helptext-7fa692642b6b6d52.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      900 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/releasenotes/notes/use-cursive-c6b15d94845232da.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      547 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/releasenotes/notes/use-webob-1.8.1-5c3cd1b1382f063e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1315 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/releasenotes/notes/ussuri-final-b377a21508ada060.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1657 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/releasenotes/notes/victoria-m2-release-notes-8a6ae2fdb3d29dae.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1033 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/releasenotes/notes/victoria-m3-releasenotes-9209cea98a29abc4.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      800 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/releasenotes/notes/victoria-rc1-release-notes-d928355cf90d608d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      325 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/releasenotes/notes/virtuozzo-hypervisor-fada477b64ae829d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      416 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/releasenotes/notes/wallaby-m3-releasenotes-bdc9fe6938aba8cc.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       64 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/releasenotes/notes/windows-support-f4aae61681dba569.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2369 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/releasenotes/notes/wsgi-containerization-369880238a5e793d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      411 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/releasenotes/notes/xena-m2-releasenotes-e68fd81ece1d514a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      944 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/releasenotes/notes/xena-m3-releasenotes-a92d55d29eecc8f6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      845 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/releasenotes/notes/xena-rc1-release-notes-12dbe0ac528ce483.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      755 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/releasenotes/notes/yoga-rc1-release-notes-153932161f52a038.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      757 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/releasenotes/notes/zed-milestone-1-592415040e67924e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      655 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/releasenotes/notes/zed-milestone-2-a782e75cdbd8fe13.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      633 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/releasenotes/notes/zed-milestone-3-3e38697ae4677a81.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:41:11.045157 glance-27.0.0.0b1/releasenotes/source/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/releasenotes/source/2023.1.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:41:11.045157 glance-27.0.0.0b1/releasenotes/source/_static/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/releasenotes/source/_static/.placeholder
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:41:11.045157 glance-27.0.0.0b1/releasenotes/source/_templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/releasenotes/source/_templates/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8927 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/releasenotes/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      264 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/releasenotes/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      146 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/releasenotes/source/liberty.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:41:10.865070 glance-27.0.0.0b1/releasenotes/source/locale/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:41:10.865070 glance-27.0.0.0b1/releasenotes/source/locale/en_GB/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:41:11.045157 glance-27.0.0.0b1/releasenotes/source/locale/en_GB/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   244590 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/releasenotes/source/locale/en_GB/LC_MESSAGES/releasenotes.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:41:10.865070 glance-27.0.0.0b1/releasenotes/source/locale/fr/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:41:11.045157 glance-27.0.0.0b1/releasenotes/source/locale/fr/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1540 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/releasenotes/source/locale/fr/LC_MESSAGES/releasenotes.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:41:10.865070 glance-27.0.0.0b1/releasenotes/source/locale/ja/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:41:11.045157 glance-27.0.0.0b1/releasenotes/source/locale/ja/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   123718 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/releasenotes/source/locale/ja/LC_MESSAGES/releasenotes.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:41:10.865070 glance-27.0.0.0b1/releasenotes/source/locale/ko_KR/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:41:11.045157 glance-27.0.0.0b1/releasenotes/source/locale/ko_KR/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12811 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/releasenotes/source/locale/ko_KR/LC_MESSAGES/releasenotes.po
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/releasenotes/source/mitaka.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      183 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/releasenotes/source/newton.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/releasenotes/source/ocata.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/releasenotes/source/pike.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      203 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/releasenotes/source/queens.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/releasenotes/source/rocky.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/releasenotes/source/stein.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/releasenotes/source/train.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      112 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/releasenotes/source/unreleased.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/releasenotes/source/ussuri.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/releasenotes/source/victoria.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/releasenotes/source/wallaby.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/releasenotes/source/xena.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/releasenotes/source/yoga.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/releasenotes/source/zed.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1654 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3115 2023-05-12 14:41:11.049159 glance-27.0.0.0b1/setup.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      766 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/setup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1050 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/test-requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:41:11.045157 glance-27.0.0.0b1/tools/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     3184 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/tools/test-setup.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     4037 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/tools/test_format_inspector.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5764 2023-05-12 14:40:42.000000 glance-27.0.0.0b1/tox.ini
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 12:16:37.896140 glance-27.0.0.0b2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       89 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/.coveragerc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1207 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/.mailmap
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/.stestr.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14545 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/.zuul.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    25701 2023-07-13 12:16:37.000000 glance-27.0.0.0b2/AUTHORS
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      588 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/CONTRIBUTING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   226275 2023-07-13 12:16:37.000000 glance-27.0.0.0b2/ChangeLog
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      786 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/HACKING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/LICENSE
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3272 2023-07-13 12:16:37.896140 glance-27.0.0.0b2/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1955 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 12:16:37.776143 glance-27.0.0.0b2/api-ref/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 12:16:37.788143 glance-27.0.0.0b2/api-ref/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6702 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/api-ref/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      569 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/api-ref/source/heading-level-guide.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      845 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/api-ref/source/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 12:16:37.788143 glance-27.0.0.0b2/api-ref/source/v2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      742 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/api-ref/source/v2/cache-manage-parameters.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1516 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/api-ref/source/v2/cache-manage.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1594 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/api-ref/source/v2/discovery-parameters.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3045 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/api-ref/source/v2/discovery.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4662 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/api-ref/source/v2/images-data.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    22513 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/api-ref/source/v2/images-images-v2.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13388 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/api-ref/source/v2/images-import.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1353 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/api-ref/source/v2/images-parameters-descriptions.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    21246 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/api-ref/source/v2/images-parameters.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2688 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/api-ref/source/v2/images-schemas.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9338 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/api-ref/source/v2/images-sharing-v2.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      803 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/api-ref/source/v2/images-tags.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1155 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/api-ref/source/v2/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2776 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/api-ref/source/v2/metadefs-index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6577 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/api-ref/source/v2/metadefs-namespaces-objects.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6374 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/api-ref/source/v2/metadefs-namespaces-properties.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5884 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/api-ref/source/v2/metadefs-namespaces-tags.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8772 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/api-ref/source/v2/metadefs-namespaces.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13711 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/api-ref/source/v2/metadefs-parameters.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3729 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/api-ref/source/v2/metadefs-resourcetypes.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6920 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/api-ref/source/v2/metadefs-schemas.inc
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 12:16:37.800143 glance-27.0.0.0b2/api-ref/source/v2/samples/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      390 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/api-ref/source/v2/samples/cache-list-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      133 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/api-ref/source/v2/samples/image-create-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      726 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/api-ref/source/v2/samples/image-create-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      893 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/api-ref/source/v2/samples/image-details-deactivate-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      174 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/api-ref/source/v2/samples/image-import-c-i-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      151 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/api-ref/source/v2/samples/image-import-g-d-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      189 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/api-ref/source/v2/samples/image-import-gd-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      206 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/api-ref/source/v2/samples/image-import-w-d-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      196 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/api-ref/source/v2/samples/image-info-import-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       53 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/api-ref/source/v2/samples/image-member-create-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      257 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/api-ref/source/v2/samples/image-member-create-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      257 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/api-ref/source/v2/samples/image-member-details-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       29 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/api-ref/source/v2/samples/image-member-update-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      258 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/api-ref/source/v2/samples/image-member-update-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      662 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/api-ref/source/v2/samples/image-members-list-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      888 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/api-ref/source/v2/samples/image-show-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      988 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/api-ref/source/v2/samples/image-tasks-show-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      229 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/api-ref/source/v2/samples/image-update-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      910 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/api-ref/source/v2/samples/image-update-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2246 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/api-ref/source/v2/samples/images-list-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      220 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/api-ref/source/v2/samples/metadef-namespace-create-request-simple.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1102 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/api-ref/source/v2/samples/metadef-namespace-create-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      470 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/api-ref/source/v2/samples/metadef-namespace-create-response-simple.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1213 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/api-ref/source/v2/samples/metadef-namespace-create-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1173 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/api-ref/source/v2/samples/metadef-namespace-details-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1179 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/api-ref/source/v2/samples/metadef-namespace-details-with-rt-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      333 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/api-ref/source/v2/samples/metadef-namespace-update-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      577 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/api-ref/source/v2/samples/metadef-namespace-update-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3629 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/api-ref/source/v2/samples/metadef-namespaces-list-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1634 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/api-ref/source/v2/samples/metadef-object-create-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1840 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/api-ref/source/v2/samples/metadef-object-create-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1840 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/api-ref/source/v2/samples/metadef-object-details-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      635 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/api-ref/source/v2/samples/metadef-object-update-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      841 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/api-ref/source/v2/samples/metadef-object-update-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7469 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/api-ref/source/v2/samples/metadef-objects-list-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4387 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/api-ref/source/v2/samples/metadef-properties-list-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      577 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/api-ref/source/v2/samples/metadef-property-create-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      577 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/api-ref/source/v2/samples/metadef-property-create-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      577 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/api-ref/source/v2/samples/metadef-property-details-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      577 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/api-ref/source/v2/samples/metadef-property-update-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      577 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/api-ref/source/v2/samples/metadef-property-update-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      176 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/api-ref/source/v2/samples/metadef-resource-type-assoc-create-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      324 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/api-ref/source/v2/samples/metadef-resource-type-assoc-list-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       92 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/api-ref/source/v2/samples/metadef-resource-type-create-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      841 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/api-ref/source/v2/samples/metadef-resource-types-list-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      119 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/api-ref/source/v2/samples/metadef-tag-create-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      114 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/api-ref/source/v2/samples/metadef-tag-details-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       31 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/api-ref/source/v2/samples/metadef-tag-update-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      115 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/api-ref/source/v2/samples/metadef-tag-update-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      188 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/api-ref/source/v2/samples/metadef-tags-create-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      188 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/api-ref/source/v2/samples/metadef-tags-create-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      188 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/api-ref/source/v2/samples/metadef-tags-list-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1033 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/api-ref/source/v2/samples/schemas-image-member-show-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1742 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/api-ref/source/v2/samples/schemas-image-members-list-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7811 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/api-ref/source/v2/samples/schemas-image-show-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11491 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/api-ref/source/v2/samples/schemas-images-list-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7210 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/api-ref/source/v2/samples/schemas-metadef-namespace-show-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9122 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/api-ref/source/v2/samples/schemas-metadef-namespaces-list-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5035 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/api-ref/source/v2/samples/schemas-metadef-object-show-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6101 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/api-ref/source/v2/samples/schemas-metadef-objects-list-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4593 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/api-ref/source/v2/samples/schemas-metadef-properties-list-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2861 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/api-ref/source/v2/samples/schemas-metadef-property-show-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1593 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/api-ref/source/v2/samples/schemas-metadef-resource-type-association-show-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2625 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/api-ref/source/v2/samples/schemas-metadef-resource-type-associations-list-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      602 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/api-ref/source/v2/samples/schemas-metadef-tag-show-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1458 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/api-ref/source/v2/samples/schemas-metadef-tags-list-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2072 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/api-ref/source/v2/samples/schemas-task-show-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2455 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/api-ref/source/v2/samples/schemas-tasks-list-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1252 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/api-ref/source/v2/samples/stores-list-detail-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      589 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/api-ref/source/v2/samples/stores-list-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      278 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/api-ref/source/v2/samples/task-create-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      621 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/api-ref/source/v2/samples/task-create-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      696 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/api-ref/source/v2/samples/task-show-failure-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      589 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/api-ref/source/v2/samples/task-show-processing-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      714 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/api-ref/source/v2/samples/task-show-success-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      911 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/api-ref/source/v2/samples/tasks-list-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      391 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/api-ref/source/v2/samples/usage-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      610 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/api-ref/source/v2/stores.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5095 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/api-ref/source/v2/tasks-parameters.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1345 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/api-ref/source/v2/tasks-schemas.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3542 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/api-ref/source/v2/tasks.inc
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 12:16:37.800143 glance-27.0.0.0b2/api-ref/source/versions/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3668 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/api-ref/source/versions/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 12:16:37.800143 glance-27.0.0.0b2/api-ref/source/versions/samples/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4454 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/api-ref/source/versions/samples/image-versions-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      798 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/api-ref/source/versions/versions.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1200 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/bindep.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 12:16:37.800143 glance-27.0.0.0b2/doc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      468 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/doc/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 12:16:37.800143 glance-27.0.0.0b2/doc/source/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 12:16:37.800143 glance-27.0.0.0b2/doc/source/_extra/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3326 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/doc/source/_extra/.htaccess
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 12:16:37.800143 glance-27.0.0.0b2/doc/source/_static/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/doc/source/_static/.placeholder
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 12:16:37.804143 glance-27.0.0.0b2/doc/source/admin/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3142 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/doc/source/admin/apache-httpd.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3779 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/doc/source/admin/authentication.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9196 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/doc/source/admin/cache.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8121 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/doc/source/admin/controllingservers.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2159 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/doc/source/admin/db-sqlalchemy-migrate.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9263 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/doc/source/admin/db.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      831 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/doc/source/admin/flows.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      479 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/doc/source/admin/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    31604 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/doc/source/admin/interoperable-image-import.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13329 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/doc/source/admin/manage-images.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7589 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/doc/source/admin/multistores.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5366 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/doc/source/admin/notifications.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1314 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/doc/source/admin/os_hash_algo.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6217 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/doc/source/admin/policies.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3824 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/doc/source/admin/property-protections.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7509 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/doc/source/admin/quotas.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3479 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/doc/source/admin/requirements.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5569 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/doc/source/admin/rollingupgrades.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7053 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/doc/source/admin/tasks.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16419 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/doc/source/admin/troubleshooting.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    26318 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/doc/source/admin/useful-image-properties.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8112 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/doc/source/admin/zero-downtime-db-upgrade.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 12:16:37.804143 glance-27.0.0.0b2/doc/source/cli/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      212 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/doc/source/cli/footer.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2295 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/doc/source/cli/general_options.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      500 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/doc/source/cli/glanceapi.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      992 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/doc/source/cli/glancecachecleaner.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1767 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/doc/source/cli/glancecachemanage.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      558 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/doc/source/cli/glancecacheprefetcher.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      619 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/doc/source/cli/glancecachepruner.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1146 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/doc/source/cli/glancecontrol.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3961 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/doc/source/cli/glancemanage.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2017 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/doc/source/cli/glancereplicator.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5295 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/doc/source/cli/glancescrubber.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2416 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/doc/source/cli/glancestatus.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      195 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/doc/source/cli/header.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/doc/source/cli/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      734 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/doc/source/cli/openstack_options.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5557 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/doc/source/conf.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 12:16:37.804143 glance-27.0.0.0b2/doc/source/configuration/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    60956 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/doc/source/configuration/configuring.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      148 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/doc/source/configuration/glance_api.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      158 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/doc/source/configuration/glance_cache.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      163 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/doc/source/configuration/glance_manage.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      268 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/doc/source/configuration/glance_policy.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      173 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/doc/source/configuration/glance_scrubber.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      414 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/doc/source/configuration/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1792 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/doc/source/configuration/sample-configuration.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 12:16:37.808143 glance-27.0.0.0b2/doc/source/contributor/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3839 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/doc/source/contributor/architecture.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3275 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/doc/source/contributor/blueprints.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8712 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/doc/source/contributor/contributing.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5869 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/doc/source/contributor/core_reviewer_guidelines.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10493 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/doc/source/contributor/database_architecture.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13229 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/doc/source/contributor/database_migrations.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3780 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/doc/source/contributor/documentation.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4965 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/doc/source/contributor/domain_implementation.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10110 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/doc/source/contributor/domain_model.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1839 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/doc/source/contributor/gerrit.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4297 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/doc/source/contributor/glance-groups.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1453 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/doc/source/contributor/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4650 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/doc/source/contributor/minor-code-changes.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2918 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/doc/source/contributor/refreshing-configs.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12244 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/doc/source/contributor/release-cpl.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2487 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/doc/source/contributor/release-notes.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5452 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/doc/source/contributor/releasecycle.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       84 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/doc/source/deprecation-note.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   120177 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/doc/source/glossary.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 12:16:37.808143 glance-27.0.0.0b2/doc/source/images/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    48303 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/doc/source/images/architecture.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   108006 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/doc/source/images/glance_db.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    32606 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/doc/source/images/glance_layers.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   250651 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/doc/source/images/image_status_transition.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    28449 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/doc/source/images/instance-life-1.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    39847 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/doc/source/images/instance-life-2.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    30176 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/doc/source/images/instance-life-3.png
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 12:16:37.808143 glance-27.0.0.0b2/doc/source/images_src/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    57938 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/doc/source/images_src/architecture.graphml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12358 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/doc/source/images_src/glance_db.graphml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    21398 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/doc/source/images_src/glance_layers.graphml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2040 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/doc/source/images_src/image_status_transition.dot
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4167 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/doc/source/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 12:16:37.812142 glance-27.0.0.0b2/doc/source/install/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1152 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/doc/source/install/configure-quotas.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3378 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/doc/source/install/get-started.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      774 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/doc/source/install/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8181 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/doc/source/install/install-debian.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8543 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/doc/source/install/install-obs.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8311 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/doc/source/install/install-rdo.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8170 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/doc/source/install/install-ubuntu.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      272 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/doc/source/install/install.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      310 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/doc/source/install/note_configuration_vary_by_distribution.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3277 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/doc/source/install/register-quotas.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4183 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/doc/source/install/verify.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 12:16:37.812142 glance-27.0.0.0b2/doc/source/user/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3511 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/doc/source/user/common-image-properties.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6185 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/doc/source/user/formats.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    34733 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/doc/source/user/glanceapi.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1090 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/doc/source/user/glanceclient.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    19470 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/doc/source/user/glancemetadefcatalogapi.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1036 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/doc/source/user/identifiers.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      256 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/doc/source/user/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8930 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/doc/source/user/metadefs-concepts.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4682 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/doc/source/user/os_hash_algo.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6281 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/doc/source/user/signature.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6027 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/doc/source/user/statuses.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 12:16:37.812142 glance-27.0.0.0b2/doc/test/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4624 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/doc/test/redirect-tests.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 12:16:37.812142 glance-27.0.0.0b2/etc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3271 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/etc/glance-api-paste.ini
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   204467 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/etc/glance-api.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    82774 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/etc/glance-cache.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8409 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/etc/glance-image-import.conf.sample
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10401 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/etc/glance-manage.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       66 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/etc/glance-policy-generator.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    85943 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/etc/glance-scrubber.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      606 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/etc/glance-swift.conf.sample
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 12:16:37.816142 glance-27.0.0.0b2/etc/metadefs/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      270 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/etc/metadefs/README
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5190 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/etc/metadefs/cim-processor-allocation-setting-data.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7051 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/etc/metadefs/cim-resource-allocation-setting-data.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5168 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/etc/metadefs/cim-storage-allocation-setting-data.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5239 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/etc/metadefs/cim-virtual-system-setting-data.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1090 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/etc/metadefs/compute-aggr-disk-filter.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1043 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/etc/metadefs/compute-aggr-iops-filter.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      897 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/etc/metadefs/compute-aggr-num-instances.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      737 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/etc/metadefs/compute-cpu-mode.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1295 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/etc/metadefs/compute-cpu-pinning.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1145 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/etc/metadefs/compute-guest-memory-backing.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      944 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/etc/metadefs/compute-guest-shutdown.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9206 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/etc/metadefs/compute-host-capabilities.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2269 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/etc/metadefs/compute-hypervisor.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1861 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/etc/metadefs/compute-instance-data.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7583 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/etc/metadefs/compute-libvirt-image.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1985 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/etc/metadefs/compute-libvirt.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7204 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/etc/metadefs/compute-quota.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1052 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/etc/metadefs/compute-randomgen.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2004 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/etc/metadefs/compute-vcputopology.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1773 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/etc/metadefs/compute-vmware-flavor.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1644 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/etc/metadefs/compute-vmware-quota-flavor.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8441 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/etc/metadefs/compute-vmware.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      799 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/etc/metadefs/compute-vtpm-hw.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1071 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/etc/metadefs/compute-vtpm.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1430 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/etc/metadefs/compute-watchdog.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      998 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/etc/metadefs/compute-xenapi.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3455 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/etc/metadefs/glance-common-image-props.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1687 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/etc/metadefs/image-signature-verification.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1314 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/etc/metadefs/operating-system.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18731 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/etc/metadefs/software-databases.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5252 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/etc/metadefs/software-runtimes.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5772 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/etc/metadefs/software-webservers.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1100 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/etc/metadefs/storage-volume-type.json
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 12:16:37.820142 glance-27.0.0.0b2/etc/oslo-config-generator/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      527 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/etc/oslo-config-generator/glance-api.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      185 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/etc/oslo-config-generator/glance-cache.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       97 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/etc/oslo-config-generator/glance-image-import.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      137 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/etc/oslo-config-generator/glance-manage.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      240 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/etc/oslo-config-generator/glance-scrubber.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/etc/ovf-metadata.json.sample
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1402 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/etc/property-protections-policies.conf.sample
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1101 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/etc/property-protections-roles.conf.sample
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2145 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/etc/schema-image.json
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 12:16:37.820142 glance-27.0.0.0b2/glance/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 12:16:37.820142 glance-27.0.0.0b2/glance/api/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1255 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/api/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8321 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/api/common.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 12:16:37.824142 glance-27.0.0.0b2/glance/api/middleware/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/api/middleware/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12611 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/api/middleware/cache.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3034 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/api/middleware/cache_manage.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5750 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/api/middleware/context.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2279 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/api/middleware/gzip.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4515 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/api/middleware/version_negotiation.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7339 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/api/policy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5096 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/api/property_protections.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 12:16:37.824142 glance-27.0.0.0b2/glance/api/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/api/v1/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1053 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/api/v1/router.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 12:16:37.824142 glance-27.0.0.0b2/glance/api/v2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/api/v2/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10253 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/api/v2/cached_images.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6717 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/api/v2/discovery.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4763 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/api/v2/image_actions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    26019 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/api/v2/image_data.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    19505 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/api/v2/image_members.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4696 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/api/v2/image_tags.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    84250 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/api/v2/images.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    38032 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/api/v2/metadef_namespaces.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18163 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/api/v2/metadef_objects.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16423 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/api/v2/metadef_properties.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14015 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/api/v2/metadef_resource_types.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    19240 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/api/v2/metadef_tags.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 12:16:37.824142 glance-27.0.0.0b2/glance/api/v2/model/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/api/v2/model/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3021 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/api/v2/model/metadef_namespace.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1768 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/api/v2/model/metadef_object.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      906 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/api/v2/model/metadef_property_item_type.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2354 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/api/v2/model/metadef_property_type.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2186 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/api/v2/model/metadef_resource_type.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1139 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/api/v2/model/metadef_tag.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17869 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/api/v2/policy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    29774 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/api/v2/router.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3947 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/api/v2/schemas.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16565 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/api/v2/tasks.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4435 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/api/versions.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 12:16:37.824142 glance-27.0.0.0b2/glance/async_/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7077 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/async_/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 12:16:37.828142 glance-27.0.0.0b2/glance/async_/flows/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/async_/flows/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 12:16:37.828142 glance-27.0.0.0b2/glance/async_/flows/_internal_plugins/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7580 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/async_/flows/_internal_plugins/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5431 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/async_/flows/_internal_plugins/base_download.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5889 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/async_/flows/_internal_plugins/copy_image.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4711 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/async_/flows/_internal_plugins/glance_download.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3600 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/async_/flows/_internal_plugins/web_download.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    41972 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/async_/flows/api_image_import.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    20847 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/async_/flows/base_import.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5962 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/async_/flows/convert.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3550 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/async_/flows/introspect.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11075 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/async_/flows/ovf_process.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 12:16:37.828142 glance-27.0.0.0b2/glance/async_/flows/plugins/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1202 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/async_/flows/plugins/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7617 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/async_/flows/plugins/image_conversion.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5747 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/async_/flows/plugins/image_decompression.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2975 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/async_/flows/plugins/inject_image_metadata.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1882 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/async_/flows/plugins/no_op.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1492 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/async_/flows/plugins/plugin_opts.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7319 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/async_/taskflow_executor.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4214 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/async_/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 12:16:37.828142 glance-27.0.0.0b2/glance/cmd/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/cmd/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4199 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/cmd/api.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2156 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/cmd/cache_cleaner.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17537 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/cmd/cache_manage.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2134 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/cmd/cache_prefetcher.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1753 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/cmd/cache_pruner.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13626 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/cmd/control.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    23152 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/cmd/manage.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    27453 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/cmd/replicator.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6100 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/cmd/scrubber.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2924 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/cmd/status.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 12:16:37.832142 glance-27.0.0.0b2/glance/common/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/common/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12068 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/common/auth.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    22672 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/common/client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    28492 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/common/config.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3208 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/common/crypt.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14512 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/common/exception.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)    25753 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/common/format_inspector.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 12:16:37.832142 glance-27.0.0.0b2/glance/common/location_strategy/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4768 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/common/location_strategy/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1080 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/common/location_strategy/location_order.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4352 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/common/location_strategy/store_type.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9594 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/common/property_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1354 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/common/removed_config.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 12:16:37.832142 glance-27.0.0.0b2/glance/common/scripts/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2439 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/common/scripts/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 12:16:37.832142 glance-27.0.0.0b2/glance/common/scripts/api_image_import/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/common/scripts/api_image_import/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5424 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/common/scripts/api_image_import/main.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 12:16:37.832142 glance-27.0.0.0b2/glance/common/scripts/image_import/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/common/scripts/image_import/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6684 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/common/scripts/image_import/main.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8395 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/common/scripts/utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9190 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/common/store_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4854 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/common/swift_store_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2890 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/common/timeutils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4550 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/common/trust_auth.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    25407 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/common/utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    47333 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/common/wsgi.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5539 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/common/wsgi_app.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2324 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/common/wsme_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3636 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/context.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 12:16:37.832142 glance-27.0.0.0b2/glance/db/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    35376 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/db/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2122 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/db/metadata.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1097 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/db/migration.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 12:16:37.832142 glance-27.0.0.0b2/glance/db/simple/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      153 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/db/simple/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    70123 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/db/simple/api.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 12:16:37.836142 glance-27.0.0.0b2/glance/db/sqlalchemy/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/db/sqlalchemy/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 12:16:37.836142 glance-27.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       39 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/README
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3058 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10416 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/add_artifacts_tables.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8936 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/add_images_tables.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7878 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/add_metadefs_tables.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2846 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/add_tasks_tables.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1557 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/alembic.ini
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 12:16:37.836142 glance-27.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/data_migrations/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      826 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/data_migrations/2023_1_migrate01_empty.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2331 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/data_migrations/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3938 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/data_migrations/ocata_migrate01_community_images.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      905 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/data_migrations/pike_migrate01_empty.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      823 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/data_migrations/queens_migrate01_empty.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      826 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/data_migrations/rocky_migrate01_empty.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      831 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/data_migrations/rocky_migrate02_empty.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2173 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/data_migrations/train_migrate01_backend_to_store.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      826 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/data_migrations/ussuri_migrate01_empty.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      826 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/data_migrations/wallaby_migrate01_empty.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      826 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/data_migrations/xena_migrate01_empty.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      826 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/data_migrations/yoga_migrate01_empty.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      826 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/data_migrations/zed_migrate01_empty.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2674 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/env.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      993 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/migrate.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      431 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/script.py.mako
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 12:16:37.840142 glance-27.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/versions/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      814 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/versions/2023_1_contract01_empty.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      921 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/versions/2023_1_expand01_empty.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/versions/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1289 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/versions/liberty_initial.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1432 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/versions/mitaka01_add_image_created_updated_idx.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1272 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/versions/mitaka02_update_metadef_os_nova_server.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2355 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/versions/ocata_contract01_drop_is_public.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5934 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/versions/ocata_expand01_add_visibility.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1337 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/versions/pike_contract01_drop_artifacts_tables.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      887 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/versions/pike_expand01_empty.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      813 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/versions/queens_contract01_empty.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      796 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/versions/queens_expand01_empty.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      816 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/versions/rocky_contract01_empty.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      820 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/versions/rocky_contract02_empty.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1135 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/versions/rocky_expand01_add_os_hidden.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1222 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/versions/rocky_expand02_add_os_hash_.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      814 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/versions/train_contract01_empty.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      922 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/versions/train_expand01_empty.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      816 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/versions/ussuri_contract01_empty.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      923 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/versions/ussuri_expand01_empty.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      819 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/versions/wallaby_contract01_empty.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1388 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/versions/wallaby_expand01_add_user_imageid_requestid_to_tasks.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      814 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/versions/xena_contract01_empty.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      923 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/versions/xena_expand01_empty.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      811 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/versions/yoga_contract01_empty.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      920 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/versions/yoga_expand01_empty.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      809 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/versions/zed_contract01_empty.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      919 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/versions/zed_expand01_empty.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    82565 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/db/sqlalchemy/api.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17923 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/db/sqlalchemy/metadata.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 12:16:37.840142 glance-27.0.0.0b2/glance/db/sqlalchemy/metadef_api/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/db/sqlalchemy/metadef_api/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10906 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/db/sqlalchemy/metadef_api/namespace.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5734 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/db/sqlalchemy/metadef_api/object.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6085 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/db/sqlalchemy/metadef_api/property.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3635 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/db/sqlalchemy/metadef_api/resource_type.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8277 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/db/sqlalchemy/metadef_api/resource_type_association.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7798 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/db/sqlalchemy/metadef_api/tag.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      921 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/db/sqlalchemy/metadef_api/utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10581 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/db/sqlalchemy/models.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7149 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/db/sqlalchemy/models_metadef.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1486 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/db/sqlalchemy/schema.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2522 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/db/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 12:16:37.840142 glance-27.0.0.0b2/glance/domain/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    23897 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/domain/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    20262 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/domain/proxy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8814 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/gateway.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 12:16:37.840142 glance-27.0.0.0b2/glance/hacking/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/hacking/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4119 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/hacking/checks.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4519 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/housekeeping.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1351 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/i18n.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 12:16:37.844141 glance-27.0.0.0b2/glance/image_cache/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16440 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/image_cache/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      733 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/image_cache/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      797 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/image_cache/cleaner.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4433 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/image_cache/client.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 12:16:37.844141 glance-27.0.0.0b2/glance/image_cache/drivers/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/image_cache/drivers/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6566 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/image_cache/drivers/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17261 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/image_cache/drivers/sqlite.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16698 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/image_cache/drivers/xattr.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3455 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/image_cache/prefetcher.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      782 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/image_cache/pruner.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 12:16:37.780143 glance-27.0.0.0b2/glance/locale/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 12:16:37.780143 glance-27.0.0.0b2/glance/locale/de/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 12:16:37.844141 glance-27.0.0.0b2/glance/locale/de/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    59075 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/locale/de/LC_MESSAGES/glance.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 12:16:37.780143 glance-27.0.0.0b2/glance/locale/en_GB/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 12:16:37.844141 glance-27.0.0.0b2/glance/locale/en_GB/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   168210 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/locale/en_GB/LC_MESSAGES/glance.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 12:16:37.780143 glance-27.0.0.0b2/glance/locale/es/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 12:16:37.844141 glance-27.0.0.0b2/glance/locale/es/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    53588 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/locale/es/LC_MESSAGES/glance.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 12:16:37.780143 glance-27.0.0.0b2/glance/locale/fr/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 12:16:37.844141 glance-27.0.0.0b2/glance/locale/fr/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    54628 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/locale/fr/LC_MESSAGES/glance.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 12:16:37.780143 glance-27.0.0.0b2/glance/locale/it/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 12:16:37.844141 glance-27.0.0.0b2/glance/locale/it/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    53703 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/locale/it/LC_MESSAGES/glance.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 12:16:37.780143 glance-27.0.0.0b2/glance/locale/ja/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 12:16:37.844141 glance-27.0.0.0b2/glance/locale/ja/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    66528 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/locale/ja/LC_MESSAGES/glance.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 12:16:37.780143 glance-27.0.0.0b2/glance/locale/ko_KR/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 12:16:37.844141 glance-27.0.0.0b2/glance/locale/ko_KR/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    56596 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/locale/ko_KR/LC_MESSAGES/glance.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 12:16:37.780143 glance-27.0.0.0b2/glance/locale/pt_BR/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 12:16:37.844141 glance-27.0.0.0b2/glance/locale/pt_BR/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    53118 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/locale/pt_BR/LC_MESSAGES/glance.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 12:16:37.780143 glance-27.0.0.0b2/glance/locale/ru/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 12:16:37.844141 glance-27.0.0.0b2/glance/locale/ru/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    65007 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/locale/ru/LC_MESSAGES/glance.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 12:16:37.780143 glance-27.0.0.0b2/glance/locale/tr_TR/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 12:16:37.844141 glance-27.0.0.0b2/glance/locale/tr_TR/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    44846 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/locale/tr_TR/LC_MESSAGES/glance.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 12:16:37.780143 glance-27.0.0.0b2/glance/locale/zh_CN/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 12:16:37.844141 glance-27.0.0.0b2/glance/locale/zh_CN/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    49820 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/locale/zh_CN/LC_MESSAGES/glance.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 12:16:37.780143 glance-27.0.0.0b2/glance/locale/zh_TW/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 12:16:37.844141 glance-27.0.0.0b2/glance/locale/zh_TW/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    48320 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/locale/zh_TW/LC_MESSAGES/glance.po
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    25816 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/location.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    32705 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/notifier.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4822 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/opts.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 12:16:37.848141 glance-27.0.0.0b2/glance/policies/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1027 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/policies/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5231 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/policies/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2434 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/policies/cache.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1053 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/policies/discovery.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11416 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/policies/image.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12900 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/policies/metadef.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4471 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/policies/tasks.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 12:16:37.848141 glance-27.0.0.0b2/glance/quota/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14945 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/quota/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6472 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/quota/keystone.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8048 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/schema.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15248 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/scrubber.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 12:16:37.848141 glance-27.0.0.0b2/glance/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1861 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 12:16:37.848141 glance-27.0.0.0b2/glance/tests/etc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      516 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/etc/glance-swift.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      214 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/etc/policy.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      923 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/etc/property-protections-policies.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1467 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/etc/property-protections.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        3 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/etc/schema-image.json
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 12:16:37.848141 glance-27.0.0.0b2/glance/tests/functional/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    71295 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/functional/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 12:16:37.852141 glance-27.0.0.0b2/glance/tests/functional/db/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1077 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/functional/db/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   116440 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/functional/db/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    32013 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/functional/db/base_metadef.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 12:16:37.852141 glance-27.0.0.0b2/glance/tests/functional/db/migrations/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/functional/db/migrations/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1862 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/functional/db/migrations/test_mitaka01.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2752 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/functional/db/migrations/test_mitaka02.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2884 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/functional/db/migrations/test_ocata_contract01.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7914 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/functional/db/migrations/test_ocata_expand01.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7733 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/functional/db/migrations/test_ocata_migrate01.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1957 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/functional/db/migrations/test_pike_contract01.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1799 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/functional/db/migrations/test_pike_expand01.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1009 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/functional/db/migrations/test_pike_migrate01.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1650 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/functional/db/migrations/test_rocky_expand01.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1749 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/functional/db/migrations/test_rocky_expand02.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5578 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/functional/db/migrations/test_train_migrate01.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2346 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/functional/db/migrations/test_wallaby_expand01.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11099 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/functional/db/test_migrations.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17729 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/functional/db/test_sqlalchemy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6831 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/functional/ft_utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 12:16:37.852141 glance-27.0.0.0b2/glance/tests/functional/serial/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/functional/serial/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16797 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/functional/serial/test_scrubber.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2859 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/functional/store_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6839 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/functional/test_api.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16376 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/functional/test_cache_middleware.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4522 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/functional/test_client_exceptions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5036 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/functional/test_client_redirects.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3750 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/functional/test_cors_middleware.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7257 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/functional/test_glance_manage.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1689 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/functional/test_gzip_middleware.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1798 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/functional/test_healthcheck_middleware.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2790 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/functional/test_logging.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5833 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/functional/test_reload.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1348 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/functional/test_sqlite.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7126 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/functional/test_wsgi.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 12:16:37.856141 glance-27.0.0.0b2/glance/tests/functional/v2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/functional/v2/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2481 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/functional/v2/metadef_base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14754 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/functional/v2/test_cache_api.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8759 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/functional/v2/test_cache_api_policy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6175 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/functional/v2/test_discovery.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   320466 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/functional/v2/test_images.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    40391 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/functional/v2/test_images_api_policy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9095 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/functional/v2/test_images_import_locking.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12996 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/functional/v2/test_legacy_update_cinder_store.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9384 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/functional/v2/test_member_api_policy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    31238 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/functional/v2/test_metadef_namespace_api_policy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18312 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/functional/v2/test_metadef_namespaces.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12372 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/functional/v2/test_metadef_object_api_policy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18926 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/functional/v2/test_metadef_objects.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16330 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/functional/v2/test_metadef_properties.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12598 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/functional/v2/test_metadef_property_api_policy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10282 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/functional/v2/test_metadef_resourcetype_api_policy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11533 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/functional/v2/test_metadef_resourcetypes.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14844 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/functional/v2/test_metadef_tag_api_policy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16401 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/functional/v2/test_metadef_tags.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2430 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/functional/v2/test_schemas.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4906 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/functional/v2/test_tasks.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3995 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/functional/v2/test_tasks_api_policy.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 12:16:37.856141 glance-27.0.0.0b2/glance/tests/integration/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/integration/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 12:16:37.856141 glance-27.0.0.0b2/glance/tests/integration/v2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/integration/v2/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6182 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/integration/v2/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5408 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/integration/v2/test_property_quota_violations.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    20800 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/integration/v2/test_tasks_api.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4104 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/stubs.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4171 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/test_hacking.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 12:16:37.860141 glance-27.0.0.0b2/glance/tests/unit/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/unit/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 12:16:37.860141 glance-27.0.0.0b2/glance/tests/unit/api/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/unit/api/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 12:16:37.864141 glance-27.0.0.0b2/glance/tests/unit/api/middleware/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/unit/api/middleware/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6390 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/unit/api/middleware/test_cache_manage.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9192 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/unit/api/test_cmd.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5882 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/unit/api/test_common.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14130 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/unit/api/test_property_protections.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 12:16:37.864141 glance-27.0.0.0b2/glance/tests/unit/async_/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/unit/async_/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 12:16:37.864141 glance-27.0.0.0b2/glance/tests/unit/async_/flows/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/unit/async_/flows/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 12:16:37.864141 glance-27.0.0.0b2/glance/tests/unit/async_/flows/plugins/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/unit/async_/flows/plugins/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15047 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/unit/async_/flows/plugins/test_image_conversion.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4986 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/unit/async_/flows/plugins/test_inject_image_metadata.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    59084 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/unit/async_/flows/test_api_image_import.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8957 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/unit/async_/flows/test_base_download.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8260 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/unit/async_/flows/test_convert.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9323 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/unit/async_/flows/test_copy_image.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7858 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/unit/async_/flows/test_glance_download.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18116 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/unit/async_/flows/test_import.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4801 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/unit/async_/flows/test_introspect.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7116 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/unit/async_/flows/test_ovf_process.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6610 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/unit/async_/flows/test_web_download.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12007 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/unit/async_/test_async.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6448 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/unit/async_/test_taskflow_executor.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2968 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/unit/async_/test_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6263 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/unit/base.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 12:16:37.864141 glance-27.0.0.0b2/glance/tests/unit/cmd/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/unit/cmd/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3054 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/unit/cmd/test_status.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 12:16:37.868141 glance-27.0.0.0b2/glance/tests/unit/common/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/unit/common/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 12:16:37.868141 glance-27.0.0.0b2/glance/tests/unit/common/scripts/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/unit/common/scripts/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 12:16:37.868141 glance-27.0.0.0b2/glance/tests/unit/common/scripts/image_import/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/unit/common/scripts/image_import/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6491 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/unit/common/scripts/image_import/test_main.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8539 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/unit/common/scripts/test_scripts_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2442 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/unit/common/test_client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4581 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/unit/common/test_config.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2060 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/unit/common/test_exception.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15011 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/unit/common/test_format_inspector.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8449 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/unit/common/test_location_strategy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    24239 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/unit/common/test_property_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1456 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/unit/common/test_scripts.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3682 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/unit/common/test_swift_store_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8765 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/unit/common/test_timeutils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    32837 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/unit/common/test_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    33403 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/unit/common/test_wsgi.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6569 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/unit/common/test_wsgi_app.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3150 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/unit/fake_rados.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6211 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/unit/fixtures.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 12:16:37.868141 glance-27.0.0.0b2/glance/tests/unit/image_cache/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/unit/image_cache/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 12:16:37.868141 glance-27.0.0.0b2/glance/tests/unit/image_cache/drivers/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/unit/image_cache/drivers/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1234 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/unit/image_cache/drivers/test_sqlite.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 12:16:37.868141 glance-27.0.0.0b2/glance/tests/unit/keymgr/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/unit/keymgr/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      901 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/unit/keymgr/fake.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    20879 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/unit/test_auth.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4007 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/unit/test_cache_manage.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17310 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/unit/test_cache_middleware.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17069 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/unit/test_cached_images.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8667 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/unit/test_context.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6238 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/unit/test_context_middleware.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8656 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/unit/test_data_migration_framework.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    41382 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/unit/test_db.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    24028 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/unit/test_db_metadef.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    24646 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/unit/test_domain.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11419 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/unit/test_domain_proxy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7533 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/unit/test_gateway.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4556 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/unit/test_glance_manage.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    23570 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/unit/test_glance_replicator.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10568 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/unit/test_housekeeping.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    23350 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/unit/test_image_cache.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    33977 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/unit/test_manage.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2784 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/unit/test_misc.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    34473 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/unit/test_notifier.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18800 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/unit/test_policy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    37417 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/unit/test_quota.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5937 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/unit/test_schema.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6931 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/unit/test_scrubber.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    48017 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/unit/test_store_image.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3218 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/unit/test_store_location.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1312 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/unit/test_test_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17889 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/unit/test_versions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12410 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/unit/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 12:16:37.872141 glance-27.0.0.0b2/glance/tests/unit/v2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/unit/v2/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6387 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/unit/v2/test_cache_management_api.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1765 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/unit/v2/test_discovery_image_import.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4930 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/unit/v2/test_discovery_stores.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6487 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/unit/v2/test_image_actions_resource.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    48624 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/unit/v2/test_image_data_resource.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    24562 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/unit/v2/test_image_members_resource.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4188 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/unit/v2/test_image_tags_resource.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   286556 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/unit/v2/test_images_resource.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   100689 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/unit/v2/test_metadef_resources.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3167 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/unit/v2/test_schemas_resource.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    38857 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/unit/v2/test_tasks_resource.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    38246 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/unit/v2/test_v2_policy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    25420 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 12:16:37.872141 glance-27.0.0.0b2/glance/tests/var/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1285 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/var/ca.crt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1704 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/var/ca.key
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5518 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/var/certificate.crt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3243 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/var/privatekey.key
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10240 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/var/testserver-bad-ovf.ova
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    20480 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/var/testserver-no-disk.ova
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10240 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/var/testserver-no-ovf.ova
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   164385 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/var/testserver-not-tar.ova
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    20480 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/tests/var/testserver.ova
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      731 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/glance/version.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 12:16:37.820142 glance-27.0.0.0b2/glance.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3272 2023-07-13 12:16:37.000000 glance-27.0.0.0b2/glance.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    39286 2023-07-13 12:16:37.000000 glance-27.0.0.0b2/glance.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-07-13 12:16:37.000000 glance-27.0.0.0b2/glance.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2147 2023-07-13 12:16:37.000000 glance-27.0.0.0b2/glance.egg-info/entry_points.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-07-13 12:16:37.000000 glance-27.0.0.0b2/glance.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       47 2023-07-13 12:16:37.000000 glance-27.0.0.0b2/glance.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      808 2023-07-13 12:16:37.000000 glance-27.0.0.0b2/glance.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        7 2023-07-13 12:16:37.000000 glance-27.0.0.0b2/glance.egg-info/top_level.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 12:16:37.872141 glance-27.0.0.0b2/httpd/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       91 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/httpd/README
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      388 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/httpd/glance-api-uwsgi.ini
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       93 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/httpd/uwsgi-glance-api.conf
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 12:16:37.872141 glance-27.0.0.0b2/playbooks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       40 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/playbooks/enable-fips.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      964 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/playbooks/post-check-metadata-injection.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 12:16:37.872141 glance-27.0.0.0b2/rally-jobs/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1048 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/rally-jobs/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 12:16:37.872141 glance-27.0.0.0b2/rally-jobs/extra/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      172 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/rally-jobs/extra/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/rally-jobs/extra/fake.img
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      979 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/rally-jobs/glance.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 12:16:37.872141 glance-27.0.0.0b2/rally-jobs/plugins/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      394 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/rally-jobs/plugins/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 12:16:37.784143 glance-27.0.0.0b2/releasenotes/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 12:16:37.892140 glance-27.0.0.0b2/releasenotes/notes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/notes/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      407 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/notes/Prevent-removing-last-image-location-d5ee3e00efe14f34.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3197 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/notes/Stein-reno-rc1-0a03f8394934a2e7.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      756 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/notes/Train-milestone3-be5520106a182fa0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      117 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/notes/add-all-visibility-image-filter-ea2f3948ff778fe3.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      180 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/notes/add-cli-and-cache-opts-902f28d65c8fb827.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3422 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/notes/add-compressed-format-185e537187a202bd.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      153 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/notes/add-cpu-thread-pinning-metadata-09b1866b875c4647.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      503 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/notes/add-description-common-image-property-95ab1139d41579d2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      489 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/notes/add-glance-download-method-be6d9e927b8b0a43.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      394 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/notes/add-ploop-format-fdd583849504ab15.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      511 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/notes/add-processlimits-to-qemu-img-c215f5d90f741d8a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      385 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/notes/add-vhdx-format-2be99354ad320cca.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       90 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/notes/add_capability_to_purge_all_deleted_rows-7b3b9b767669b1a5.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      530 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/notes/add_policy_enforcement_for_metadef_delete_apis-95d2b16cc444840a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      444 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/notes/added-quota-usage-api-f1914054132f2021.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      169 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/notes/added-store-detail-api-215810aa85dfbb99.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1947 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/notes/alembic-migrations-902b31edae7a5d7d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      632 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/notes/antelope-milestone-2-d89e39412f9c0334.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      954 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/notes/antelope-milestone-3-b9a4f7fdba31f628.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2905 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/notes/api-2-6-current-9eeb83b7ecc0a562.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      651 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/notes/api-2.16-8417b1e23322fedb.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1462 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/notes/api-minor-ver-bump-2-6-aa3591fc58f08055.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      926 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/notes/api-minor-version-bump-bbd69dc457fc731c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/notes/bobcat-milestone-1-releasenotes-2d109105530877d6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      291 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/notes/bobcat-milestone-2-releasenotes-085084b03f66d671.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2223 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/notes/bp-barbican-secret-deletion-support-40cffa5ffa33447e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1721 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/notes/bp-inject-image-metadata-0a08af539bcce7f2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      373 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/notes/bp-mitigate-ossn-0075-c0e74e60d86d8ea2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      450 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/notes/bp-upgrade-checks-b3272c3ddb4e8cf7.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      515 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/notes/bug-1537903-54b2822eac6cfc09.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      206 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/notes/bug-1593177-8ef35458d29ec93c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      400 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/notes/bug-1719252-name-validation-443a2e2a36be2cec.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      161 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/notes/bug-1861334-ebc2026b85675d47.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      197 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/notes/bug-1881958-d0e16538f3c0ffaa.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      212 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/notes/bug-1979699-70182ec2aead0383.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      539 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/notes/bug-1980049-623d2eb0fa074136.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      436 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/notes/bump-api-2-4-efa266aef0928e04.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      369 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/notes/cache-api-b806ccfb8c5d9bb6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      611 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/notes/cinder-store-migration-non-owner-80a2a8114d8602aa.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      447 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/notes/clean-up-acceptable-values-store_type_preference-39081e4045894731.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      437 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/notes/cleanout_registry_data-api-9d91368aed83497e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       95 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/notes/cleanup-enable_v2_api-9b9b467f4ae8c3b1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1450 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/notes/consistent-store-names-57374b9505d530d0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      706 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/notes/copy-existing-image-94fd0b8d24bc16a0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      434 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/notes/delete_from_store-a1d9b9bd5cf27546.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2952 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/notes/deprecate-admin_role-2f9d33ed0785d082.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      729 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/notes/deprecate-allow_additional_image_props-0e3b2f1ffa4e55e1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1160 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/notes/deprecate-checksum-a602853403e1c4a8.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      317 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/notes/deprecate-glance-api-opts-23bdbd1ad7625999.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1008 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/notes/deprecate-json-formatted-policy-file-5cb692fe889eb52b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      346 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/notes/deprecate-owner_is_tenant-ec8ea36a3f7e9268.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      569 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/notes/deprecate-registry-ff286df90df793f0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1456 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/notes/deprecate-show-multiple-location-9890a1e961def2f6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1146 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/notes/deprecate-show-multiple-location-continued-646f91b21cd771f7.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      929 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/notes/deprecate-show-multiple-location-continued-ussuri-16e8d9d8a59da1bc.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      887 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/notes/deprecate-v1-api-6c7dbefb90fd8772.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      571 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/notes/distributed-image-import-82cff4426731beac.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      211 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/notes/drop-py-2-7-863871c7bc047146.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      129 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/notes/drop-python-3-6-and-3-7-c6f051d5b2b40329.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      270 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/notes/drop-sheepdog-b55aae84807d31d9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      363 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/notes/drop-support-for-sqlalchemy-migrate-4bcbe7b200697586.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      465 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/notes/enable-enforce-scope-and-new-defaults-ef543183e6c2eabb.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      308 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/notes/exp-emc-mig-fix-a7e28d547ac38f9e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      304 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/notes/expanding-stores-details-d3aa8ebb76ad68d9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2050 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/notes/experimental-multi-store-d2c26f9dbb9c835b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      326 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/notes/fix-md-tag-create-multiple-c04756cf5155983d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      155 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/notes/fix_1889640-95d543629d7dadce.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      202 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/notes/fix_1889676-f8d302fd240c8a57.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      150 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/notes/fix_httpd_docs-3efff0395f96a94d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      367 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/notes/glance-unified-quotas-fba62fabb00379af.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2209 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/notes/glare-ectomy-72a1f80f306f2e3b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      500 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/notes/image-conversion-plugin-5aee45e1a1a5bb2b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      469 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/notes/image-not-found-policy-override-removed-52616c483a270bcf.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      578 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/notes/image-tasks-api-f21b42eab91c2079.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8505 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/notes/image-visibility-changes-fa5aa18dc67244c4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      249 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/notes/image_decompression_plugin-5f085666aae01f29.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      377 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/notes/immediate-caching-image-e38055575c361d32.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1048 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/notes/implement-lite-spec-db-sync-check-3e2e147aec0ae82b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      642 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/notes/import-locking-behavior-901c691f3839fe0a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1056 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/notes/import-multi-stores-3e781f2878b3134d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1321 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/notes/improved-config-options-221c58a8c37602ba.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1827 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/notes/location-add-status-checks-b70db66100bc96b7.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      212 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/notes/lock_path_config_option-2771feaa649e4563.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      730 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/notes/make-task-api-admin-only-by-default-7def996262e18f7a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      347 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/notes/metadef-api-admin-operations-b9a2d863913b0cae.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2867 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/notes/multihash-081466a98601da20.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      749 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/notes/mutistore-support-for-scrubber-6b360394ef32774a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      805 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/notes/new_image_filters-c888361e6ecf495c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      871 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/notes/newton-1-release-065334d464f78fc5.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2494 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/notes/newton-bugs-06ed3727b973c271.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      151 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/notes/no_plugins_for_copy-image-26c0e384a368bf6a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      432 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/notes/os-glance-injection-disallowed-5dad244dfb071938.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      303 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/notes/os-glance-namespace-reserved-1fcb8a5fddca4e0f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      796 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/notes/oslo-log-use-stderr-changes-07f5daf3e6abdcd6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      311 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/notes/pending-delete-rollback-444ff94c0056bbdb.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      586 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/notes/pike-metadefs-changes-95b54e0bf8bbefd6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2543 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/notes/pike-rc-1-a5d3f6e8877b52c6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3977 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/notes/pike-rc-2-acc173005045e16a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1224 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/notes/policy-in-code-7e0c6c070d32d136.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      732 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/notes/policy-in-code-implications-438449a73af2893c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      713 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/notes/policy-refactor-xena-0cddb7f2d492cb3a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      986 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/notes/queens-metadefs-changes-daf02bef18d049f4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1746 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/notes/queens-uwsgi-issues-4cee9e4fdf62c646.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      582 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/notes/range-header-request-83cf11eebf865fb1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1098 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/notes/rbac-updates-ba0fcb886fe4085c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      211 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/notes/remove-admin_role-f508754e98331fc4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      440 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/notes/remove-db-downgrade-0d1cc45b97605775.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      617 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/notes/remove-enforce-secure-rbac-ec9a0249870460c2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      711 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/notes/remove-osprofiler-paste-ini-options-c620dedc8f9728ff.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      489 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/notes/remove-owner_is_tenant-b30150def293effc.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      490 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/notes/remove-s3-driver-639c60b71761eb6f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      360 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/notes/remove_enable_image_import_option-ec4a859ac9a7ea7b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      796 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/notes/remove_native_ssl-c16d5a127b57583d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      329 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/notes/remove_secure_proxy_ssl_header-2a95ad48ffa471ad.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1346 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/notes/reordered-store-config-opts-newton-3a6575b5908c0e0f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      252 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/notes/replicator-token-cleanup-4a573c86f1acccc0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      863 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/notes/restrict_location_updates-05454bb765a8c92c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2735 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/notes/rethinking-filesystem-access-120bc46064b3d40a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      478 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/notes/rocky-metadefs-changes-cb00c006ff51b541.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1945 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/notes/rocky-rc-b0ea7628b7a74c96.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      394 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/notes/scrubber-exit-e5d77f6f1a38ffb7.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      475 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/notes/scrubber-refactor-73ddbd61ebbf1e86.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2674 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/notes/secure-rbac-project-personas-fb0d9792b9dc3783.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      368 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/notes/soft_delete-tasks-43ea983695faa565.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      380 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/notes/support-cinder-multiple-stores-eb4e6d912d549ee9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      805 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/notes/train-metadefs-changes-c4380754cdd13a19.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      386 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/notes/trust-support-registry-cfd17a6a9ab21d70.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      404 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/notes/update-show_multiple_locations-helptext-7fa692642b6b6d52.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      900 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/notes/use-cursive-c6b15d94845232da.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      547 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/notes/use-webob-1.8.1-5c3cd1b1382f063e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1315 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/notes/ussuri-final-b377a21508ada060.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1657 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/notes/victoria-m2-release-notes-8a6ae2fdb3d29dae.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1033 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/notes/victoria-m3-releasenotes-9209cea98a29abc4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      800 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/notes/victoria-rc1-release-notes-d928355cf90d608d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      325 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/notes/virtuozzo-hypervisor-fada477b64ae829d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      416 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/notes/wallaby-m3-releasenotes-bdc9fe6938aba8cc.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       64 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/notes/windows-support-f4aae61681dba569.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2369 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/notes/wsgi-containerization-369880238a5e793d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      411 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/notes/xena-m2-releasenotes-e68fd81ece1d514a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      944 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/notes/xena-m3-releasenotes-a92d55d29eecc8f6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      845 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/notes/xena-rc1-release-notes-12dbe0ac528ce483.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      755 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/notes/yoga-rc1-release-notes-153932161f52a038.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      757 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/notes/zed-milestone-1-592415040e67924e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      655 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/notes/zed-milestone-2-a782e75cdbd8fe13.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      633 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/notes/zed-milestone-3-3e38697ae4677a81.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 12:16:37.896140 glance-27.0.0.0b2/releasenotes/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/source/2023.1.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 12:16:37.896140 glance-27.0.0.0b2/releasenotes/source/_static/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/source/_static/.placeholder
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 12:16:37.896140 glance-27.0.0.0b2/releasenotes/source/_templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/source/_templates/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8927 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      264 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      146 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/source/liberty.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 12:16:37.784143 glance-27.0.0.0b2/releasenotes/source/locale/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 12:16:37.784143 glance-27.0.0.0b2/releasenotes/source/locale/en_GB/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 12:16:37.896140 glance-27.0.0.0b2/releasenotes/source/locale/en_GB/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   248044 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/source/locale/en_GB/LC_MESSAGES/releasenotes.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 12:16:37.784143 glance-27.0.0.0b2/releasenotes/source/locale/fr/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 12:16:37.896140 glance-27.0.0.0b2/releasenotes/source/locale/fr/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1540 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/source/locale/fr/LC_MESSAGES/releasenotes.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 12:16:37.784143 glance-27.0.0.0b2/releasenotes/source/locale/ja/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 12:16:37.896140 glance-27.0.0.0b2/releasenotes/source/locale/ja/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   123718 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/source/locale/ja/LC_MESSAGES/releasenotes.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 12:16:37.784143 glance-27.0.0.0b2/releasenotes/source/locale/ko_KR/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 12:16:37.896140 glance-27.0.0.0b2/releasenotes/source/locale/ko_KR/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12811 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/source/locale/ko_KR/LC_MESSAGES/releasenotes.po
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/source/mitaka.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      183 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/source/newton.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/source/ocata.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/source/pike.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      203 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/source/queens.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/source/rocky.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/source/stein.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/source/train.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      112 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/source/unreleased.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/source/ussuri.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/source/victoria.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/source/wallaby.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/source/xena.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/source/yoga.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/releasenotes/source/zed.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1654 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3115 2023-07-13 12:16:37.896140 glance-27.0.0.0b2/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      766 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/setup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1050 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/test-requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 12:16:37.896140 glance-27.0.0.0b2/tools/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     3184 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/tools/test-setup.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     4037 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/tools/test_format_inspector.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5764 2023-07-13 12:16:09.000000 glance-27.0.0.0b2/tox.ini
```

### Comparing `glance-27.0.0.0b1/.mailmap` & `glance-27.0.0.0b2/.mailmap`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/.zuul.yaml` & `glance-27.0.0.0b2/.zuul.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -241,14 +241,17 @@
       The regular import workflow job to test with multiple cinder stores
     vars:
       devstack_localrc:
         USE_CINDER_FOR_GLANCE: True
         GLANCE_ENABLE_MULTIPLE_STORES: True
         CINDER_ENABLED_BACKENDS: lvm:lvmdriver-1,lvm:lvmdriver-2
         GLANCE_CINDER_DEFAULT_BACKEND: lvmdriver-1
+        # Glance RBAC new defaults are tested by default so we need to test
+        # old defaults in some job.
+        GLANCE_ENFORCE_SCOPE: false
 
 - job:
     name: glance-multistore-cinder-import-fips
     parent: tempest-integrated-storage-import
     description: |
       The regular import workflow job to test with multiple cinder stores with
       fips enabled
@@ -295,17 +298,17 @@
     name: tempest-integrated-storage-enforce-scope-new-defaults
     parent: tempest-integrated-storage
     description: |
       This job runs the Tempest tests with scope and new defaults enabled
       Glance services.
     vars:
       devstack_localrc:
-        NOVA_ENFORCE_SCOPE: true
+        # Nova and glance scope and new defaults are enabled by default in
+        # Devstack so we do not need to explicitly set that to True.
         CINDER_ENFORCE_SCOPE: true
-        GLANCE_ENFORCE_SCOPE: true
 
 - project:
     templates:
       - check-requirements
       - integrated-gate-storage
       - openstack-python3-jobs
       - openstack-python3-jobs-arm64
@@ -327,15 +330,14 @@
               - ^glance/hacking/.*$
               - ^glance/locale/.*$
               - ^glance/tests/.*$
               - ^doc/.*$
               - ^releasenotes/.*$
               - ^tools/.*$
               - ^tox.ini$
-              - ^\.zuul\.yaml$
         - tempest-integrated-storage:
             irrelevant-files: *tempest-irrelevant-files
         - tempest-integrated-storage-enforce-scope-new-defaults:
             irrelevant-files: *tempest-irrelevant-files
         - tempest-integrated-storage-import:
             irrelevant-files: *tempest-irrelevant-files
         - tempest-integrated-storage-import-standalone:
```

### Comparing `glance-27.0.0.0b1/AUTHORS` & `glance-27.0.0.0b2/AUTHORS`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/CONTRIBUTING.rst` & `glance-27.0.0.0b2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/ChangeLog` & `glance-27.0.0.0b2/ChangeLog`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,31 @@
 CHANGES
 =======
 
+27.0.0.0b2
+----------
+
+* Release notes for Bobcat Milestone 2
+* Refresh Glance example configs for bobcat milestone 2
+* Remove the last occurrence of six.add\_metaclass
+* Imported Translations from Zanata
+* Handle case for multiple cirros images
+* Test glance RBAC old defaults
+* Run integrated test if zuul.yaml file is changed
+
 27.0.0.0b1
 ----------
 
+* Bump eventlet to a version that fixes #632[1]
+* Imported Translations from Zanata
+* Refactor pipeline definition
 * Release notes for Bobcat Milestone 1
 * Refresh Glance example configs for bobcat milestone 1
 * Add rocky linux to useful image properties os\_images list
+* Deploy healthcheck middleware as app instead of filter
 * Update functional jobs for 2023.2
 * Fix functional test failures with PasteDeploy 3.x
 * Remove duplicate value in compute-host-capabilities.json
 * Change DB migration constant to 2023\_2
 * Add a check on startup for staging directory
 * Imported Translations from Zanata
 * Update master for stable/2023.1
```

### Comparing `glance-27.0.0.0b1/HACKING.rst` & `glance-27.0.0.0b2/HACKING.rst`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/LICENSE` & `glance-27.0.0.0b2/LICENSE`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/PKG-INFO` & `glance-27.0.0.0b2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: glance
-Version: 27.0.0.0b1
+Version: 27.0.0.0b2
 Summary: OpenStack Image Service
 Home-page: https://docs.openstack.org/glance/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ================
         OpenStack Glance
```

### Comparing `glance-27.0.0.0b1/README.rst` & `glance-27.0.0.0b2/README.rst`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/api-ref/source/conf.py` & `glance-27.0.0.0b2/api-ref/source/conf.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/api-ref/source/heading-level-guide.txt` & `glance-27.0.0.0b2/api-ref/source/heading-level-guide.txt`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/api-ref/source/index.rst` & `glance-27.0.0.0b2/api-ref/source/index.rst`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/api-ref/source/v2/cache-manage-parameters.yaml` & `glance-27.0.0.0b2/api-ref/source/v2/cache-manage-parameters.yaml`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/api-ref/source/v2/cache-manage.inc` & `glance-27.0.0.0b2/api-ref/source/v2/cache-manage.inc`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/api-ref/source/v2/discovery-parameters.yaml` & `glance-27.0.0.0b2/api-ref/source/v2/discovery-parameters.yaml`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/api-ref/source/v2/discovery.inc` & `glance-27.0.0.0b2/api-ref/source/v2/discovery.inc`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/api-ref/source/v2/images-data.inc` & `glance-27.0.0.0b2/api-ref/source/v2/images-data.inc`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/api-ref/source/v2/images-images-v2.inc` & `glance-27.0.0.0b2/api-ref/source/v2/images-images-v2.inc`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/api-ref/source/v2/images-import.inc` & `glance-27.0.0.0b2/api-ref/source/v2/images-import.inc`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/api-ref/source/v2/images-parameters-descriptions.inc` & `glance-27.0.0.0b2/api-ref/source/v2/images-parameters-descriptions.inc`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/api-ref/source/v2/images-parameters.yaml` & `glance-27.0.0.0b2/api-ref/source/v2/images-parameters.yaml`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/api-ref/source/v2/images-schemas.inc` & `glance-27.0.0.0b2/api-ref/source/v2/images-schemas.inc`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/api-ref/source/v2/images-sharing-v2.inc` & `glance-27.0.0.0b2/api-ref/source/v2/images-sharing-v2.inc`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/api-ref/source/v2/images-tags.inc` & `glance-27.0.0.0b2/api-ref/source/v2/images-tags.inc`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/api-ref/source/v2/index.rst` & `glance-27.0.0.0b2/api-ref/source/v2/index.rst`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/api-ref/source/v2/metadefs-index.rst` & `glance-27.0.0.0b2/api-ref/source/v2/metadefs-index.rst`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/api-ref/source/v2/metadefs-namespaces-objects.inc` & `glance-27.0.0.0b2/api-ref/source/v2/metadefs-namespaces-objects.inc`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/api-ref/source/v2/metadefs-namespaces-properties.inc` & `glance-27.0.0.0b2/api-ref/source/v2/metadefs-namespaces-properties.inc`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/api-ref/source/v2/metadefs-namespaces-tags.inc` & `glance-27.0.0.0b2/api-ref/source/v2/metadefs-namespaces-tags.inc`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/api-ref/source/v2/metadefs-namespaces.inc` & `glance-27.0.0.0b2/api-ref/source/v2/metadefs-namespaces.inc`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/api-ref/source/v2/metadefs-parameters.yaml` & `glance-27.0.0.0b2/api-ref/source/v2/metadefs-parameters.yaml`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/api-ref/source/v2/metadefs-resourcetypes.inc` & `glance-27.0.0.0b2/api-ref/source/v2/metadefs-resourcetypes.inc`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/api-ref/source/v2/metadefs-schemas.inc` & `glance-27.0.0.0b2/api-ref/source/v2/metadefs-schemas.inc`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/api-ref/source/v2/samples/image-create-response.json` & `glance-27.0.0.0b2/api-ref/source/v2/samples/image-create-response.json`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/api-ref/source/v2/samples/image-details-deactivate-response.json` & `glance-27.0.0.0b2/api-ref/source/v2/samples/image-details-deactivate-response.json`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/api-ref/source/v2/samples/image-members-list-response.json` & `glance-27.0.0.0b2/api-ref/source/v2/samples/image-members-list-response.json`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/api-ref/source/v2/samples/image-show-response.json` & `glance-27.0.0.0b2/api-ref/source/v2/samples/image-show-response.json`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/api-ref/source/v2/samples/image-tasks-show-response.json` & `glance-27.0.0.0b2/api-ref/source/v2/samples/image-tasks-show-response.json`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/api-ref/source/v2/samples/image-update-response.json` & `glance-27.0.0.0b2/api-ref/source/v2/samples/image-update-response.json`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/api-ref/source/v2/samples/images-list-response.json` & `glance-27.0.0.0b2/api-ref/source/v2/samples/images-list-response.json`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/api-ref/source/v2/samples/metadef-namespace-create-request.json` & `glance-27.0.0.0b2/api-ref/source/v2/samples/metadef-namespace-create-request.json`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/api-ref/source/v2/samples/metadef-namespace-create-response.json` & `glance-27.0.0.0b2/api-ref/source/v2/samples/metadef-namespace-create-response.json`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/api-ref/source/v2/samples/metadef-namespace-details-response.json` & `glance-27.0.0.0b2/api-ref/source/v2/samples/metadef-namespace-details-response.json`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/api-ref/source/v2/samples/metadef-namespace-details-with-rt-response.json` & `glance-27.0.0.0b2/api-ref/source/v2/samples/metadef-namespace-details-with-rt-response.json`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/api-ref/source/v2/samples/metadef-namespace-update-response.json` & `glance-27.0.0.0b2/api-ref/source/v2/samples/metadef-namespace-update-response.json`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/api-ref/source/v2/samples/metadef-namespaces-list-response.json` & `glance-27.0.0.0b2/api-ref/source/v2/samples/metadef-namespaces-list-response.json`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/api-ref/source/v2/samples/metadef-object-create-request.json` & `glance-27.0.0.0b2/api-ref/source/v2/samples/metadef-object-create-request.json`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/api-ref/source/v2/samples/metadef-object-create-response.json` & `glance-27.0.0.0b2/api-ref/source/v2/samples/metadef-object-create-response.json`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/api-ref/source/v2/samples/metadef-object-details-response.json` & `glance-27.0.0.0b2/api-ref/source/v2/samples/metadef-object-details-response.json`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/api-ref/source/v2/samples/metadef-object-update-request.json` & `glance-27.0.0.0b2/api-ref/source/v2/samples/metadef-object-update-request.json`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/api-ref/source/v2/samples/metadef-object-update-response.json` & `glance-27.0.0.0b2/api-ref/source/v2/samples/metadef-object-update-response.json`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/api-ref/source/v2/samples/metadef-objects-list-response.json` & `glance-27.0.0.0b2/api-ref/source/v2/samples/metadef-objects-list-response.json`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/api-ref/source/v2/samples/metadef-properties-list-response.json` & `glance-27.0.0.0b2/api-ref/source/v2/samples/metadef-properties-list-response.json`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/api-ref/source/v2/samples/metadef-property-create-request.json` & `glance-27.0.0.0b2/api-ref/source/v2/samples/metadef-property-create-request.json`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/api-ref/source/v2/samples/metadef-property-create-response.json` & `glance-27.0.0.0b2/api-ref/source/v2/samples/metadef-property-create-response.json`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/api-ref/source/v2/samples/metadef-property-details-response.json` & `glance-27.0.0.0b2/api-ref/source/v2/samples/metadef-property-details-response.json`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/api-ref/source/v2/samples/metadef-property-update-request.json` & `glance-27.0.0.0b2/api-ref/source/v2/samples/metadef-property-update-request.json`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/api-ref/source/v2/samples/metadef-property-update-response.json` & `glance-27.0.0.0b2/api-ref/source/v2/samples/metadef-property-update-response.json`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/api-ref/source/v2/samples/metadef-resource-types-list-response.json` & `glance-27.0.0.0b2/api-ref/source/v2/samples/metadef-resource-types-list-response.json`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/api-ref/source/v2/samples/schemas-image-member-show-response.json` & `glance-27.0.0.0b2/api-ref/source/v2/samples/schemas-image-member-show-response.json`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/api-ref/source/v2/samples/schemas-image-members-list-response.json` & `glance-27.0.0.0b2/api-ref/source/v2/samples/schemas-image-members-list-response.json`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/api-ref/source/v2/samples/schemas-image-show-response.json` & `glance-27.0.0.0b2/api-ref/source/v2/samples/schemas-image-show-response.json`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/api-ref/source/v2/samples/schemas-images-list-response.json` & `glance-27.0.0.0b2/api-ref/source/v2/samples/schemas-images-list-response.json`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/api-ref/source/v2/samples/schemas-metadef-namespace-show-response.json` & `glance-27.0.0.0b2/api-ref/source/v2/samples/schemas-metadef-namespace-show-response.json`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/api-ref/source/v2/samples/schemas-metadef-namespaces-list-response.json` & `glance-27.0.0.0b2/api-ref/source/v2/samples/schemas-metadef-namespaces-list-response.json`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/api-ref/source/v2/samples/schemas-metadef-object-show-response.json` & `glance-27.0.0.0b2/api-ref/source/v2/samples/schemas-metadef-object-show-response.json`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/api-ref/source/v2/samples/schemas-metadef-objects-list-response.json` & `glance-27.0.0.0b2/api-ref/source/v2/samples/schemas-metadef-objects-list-response.json`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/api-ref/source/v2/samples/schemas-metadef-properties-list-response.json` & `glance-27.0.0.0b2/api-ref/source/v2/samples/schemas-metadef-properties-list-response.json`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/api-ref/source/v2/samples/schemas-metadef-property-show-response.json` & `glance-27.0.0.0b2/api-ref/source/v2/samples/schemas-metadef-property-show-response.json`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/api-ref/source/v2/samples/schemas-metadef-resource-type-association-show-response.json` & `glance-27.0.0.0b2/api-ref/source/v2/samples/schemas-metadef-resource-type-association-show-response.json`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/api-ref/source/v2/samples/schemas-metadef-resource-type-associations-list-response.json` & `glance-27.0.0.0b2/api-ref/source/v2/samples/schemas-metadef-resource-type-associations-list-response.json`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/api-ref/source/v2/samples/schemas-metadef-tag-show-response.json` & `glance-27.0.0.0b2/api-ref/source/v2/samples/schemas-metadef-tag-show-response.json`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/api-ref/source/v2/samples/schemas-metadef-tags-list-response.json` & `glance-27.0.0.0b2/api-ref/source/v2/samples/schemas-metadef-tags-list-response.json`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/api-ref/source/v2/samples/schemas-task-show-response.json` & `glance-27.0.0.0b2/api-ref/source/v2/samples/schemas-task-show-response.json`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/api-ref/source/v2/samples/schemas-tasks-list-response.json` & `glance-27.0.0.0b2/api-ref/source/v2/samples/schemas-tasks-list-response.json`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/api-ref/source/v2/samples/stores-list-detail-response.json` & `glance-27.0.0.0b2/api-ref/source/v2/samples/stores-list-detail-response.json`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/api-ref/source/v2/samples/stores-list-response.json` & `glance-27.0.0.0b2/api-ref/source/v2/samples/stores-list-response.json`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/api-ref/source/v2/samples/task-create-response.json` & `glance-27.0.0.0b2/api-ref/source/v2/samples/task-create-response.json`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/api-ref/source/v2/samples/task-show-failure-response.json` & `glance-27.0.0.0b2/api-ref/source/v2/samples/task-show-failure-response.json`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/api-ref/source/v2/samples/task-show-processing-response.json` & `glance-27.0.0.0b2/api-ref/source/v2/samples/task-show-processing-response.json`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/api-ref/source/v2/samples/task-show-success-response.json` & `glance-27.0.0.0b2/api-ref/source/v2/samples/task-show-success-response.json`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/api-ref/source/v2/samples/tasks-list-response.json` & `glance-27.0.0.0b2/api-ref/source/v2/samples/tasks-list-response.json`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/api-ref/source/v2/stores.inc` & `glance-27.0.0.0b2/api-ref/source/v2/stores.inc`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/api-ref/source/v2/tasks-parameters.yaml` & `glance-27.0.0.0b2/api-ref/source/v2/tasks-parameters.yaml`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/api-ref/source/v2/tasks-schemas.inc` & `glance-27.0.0.0b2/api-ref/source/v2/tasks-schemas.inc`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/api-ref/source/v2/tasks.inc` & `glance-27.0.0.0b2/api-ref/source/v2/tasks.inc`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/api-ref/source/versions/index.rst` & `glance-27.0.0.0b2/api-ref/source/versions/index.rst`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/api-ref/source/versions/samples/image-versions-response.json` & `glance-27.0.0.0b2/api-ref/source/versions/samples/image-versions-response.json`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/api-ref/source/versions/versions.inc` & `glance-27.0.0.0b2/api-ref/source/versions/versions.inc`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/bindep.txt` & `glance-27.0.0.0b2/bindep.txt`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/doc/source/_extra/.htaccess` & `glance-27.0.0.0b2/doc/source/_extra/.htaccess`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/doc/source/admin/apache-httpd.rst` & `glance-27.0.0.0b2/doc/source/admin/apache-httpd.rst`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/doc/source/admin/authentication.rst` & `glance-27.0.0.0b2/doc/source/admin/authentication.rst`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/doc/source/admin/cache.rst` & `glance-27.0.0.0b2/doc/source/admin/cache.rst`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/doc/source/admin/controllingservers.rst` & `glance-27.0.0.0b2/doc/source/admin/controllingservers.rst`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/doc/source/admin/db-sqlalchemy-migrate.rst` & `glance-27.0.0.0b2/doc/source/admin/db-sqlalchemy-migrate.rst`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/doc/source/admin/db.rst` & `glance-27.0.0.0b2/doc/source/admin/db.rst`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/doc/source/admin/flows.rst` & `glance-27.0.0.0b2/doc/source/admin/flows.rst`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/doc/source/admin/interoperable-image-import.rst` & `glance-27.0.0.0b2/doc/source/admin/interoperable-image-import.rst`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/doc/source/admin/manage-images.rst` & `glance-27.0.0.0b2/doc/source/admin/manage-images.rst`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/doc/source/admin/multistores.rst` & `glance-27.0.0.0b2/doc/source/admin/multistores.rst`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/doc/source/admin/notifications.rst` & `glance-27.0.0.0b2/doc/source/admin/notifications.rst`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/doc/source/admin/os_hash_algo.rst` & `glance-27.0.0.0b2/doc/source/admin/os_hash_algo.rst`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/doc/source/admin/policies.rst` & `glance-27.0.0.0b2/doc/source/admin/policies.rst`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/doc/source/admin/property-protections.rst` & `glance-27.0.0.0b2/doc/source/admin/property-protections.rst`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/doc/source/admin/quotas.rst` & `glance-27.0.0.0b2/doc/source/admin/quotas.rst`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/doc/source/admin/requirements.rst` & `glance-27.0.0.0b2/doc/source/admin/requirements.rst`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/doc/source/admin/rollingupgrades.rst` & `glance-27.0.0.0b2/doc/source/admin/rollingupgrades.rst`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/doc/source/admin/tasks.rst` & `glance-27.0.0.0b2/doc/source/admin/tasks.rst`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/doc/source/admin/troubleshooting.rst` & `glance-27.0.0.0b2/doc/source/admin/troubleshooting.rst`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/doc/source/admin/useful-image-properties.rst` & `glance-27.0.0.0b2/doc/source/admin/useful-image-properties.rst`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/doc/source/admin/zero-downtime-db-upgrade.rst` & `glance-27.0.0.0b2/doc/source/admin/zero-downtime-db-upgrade.rst`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/doc/source/cli/general_options.txt` & `glance-27.0.0.0b2/doc/source/cli/general_options.txt`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/doc/source/cli/glancecachecleaner.rst` & `glance-27.0.0.0b2/doc/source/cli/glancecachecleaner.rst`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/doc/source/cli/glancecachemanage.rst` & `glance-27.0.0.0b2/doc/source/cli/glancecachemanage.rst`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/doc/source/cli/glancecacheprefetcher.rst` & `glance-27.0.0.0b2/doc/source/cli/glancecacheprefetcher.rst`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/doc/source/cli/glancecachepruner.rst` & `glance-27.0.0.0b2/doc/source/cli/glancecachepruner.rst`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/doc/source/cli/glancecontrol.rst` & `glance-27.0.0.0b2/doc/source/cli/glancecontrol.rst`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/doc/source/cli/glancemanage.rst` & `glance-27.0.0.0b2/doc/source/cli/glancemanage.rst`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/doc/source/cli/glancereplicator.rst` & `glance-27.0.0.0b2/doc/source/cli/glancereplicator.rst`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/doc/source/cli/glancescrubber.rst` & `glance-27.0.0.0b2/doc/source/cli/glancescrubber.rst`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/doc/source/cli/glancestatus.rst` & `glance-27.0.0.0b2/doc/source/cli/glancestatus.rst`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/doc/source/cli/openstack_options.txt` & `glance-27.0.0.0b2/doc/source/cli/openstack_options.txt`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/doc/source/conf.py` & `glance-27.0.0.0b2/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/doc/source/configuration/configuring.rst` & `glance-27.0.0.0b2/doc/source/configuration/configuring.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1693,27 +1693,29 @@
 be available or not. Glance API server can be configured to expose a health
 check URL.
 
 To enable the health check middleware, it must occur in the beginning of the
 application pipeline.
 
 The health check middleware should be placed in your
-``glance-api-paste.ini`` in a section titled ``[filter:healthcheck]``.
+``glance-api-paste.ini`` in a section titled ``[app:healthcheck]``.
 It should look like this::
 
-  [filter:healthcheck]
-  paste.filter_factory = oslo_middleware:Healthcheck.factory
+  [app:healthcheck]
+  paste.app_factory = oslo_middleware:Healthcheck.app_factory
   backends = disable_by_file
   disable_by_file_path = /etc/glance/healthcheck_disable
 
-A ready-made application pipeline including this filter is defined e.g. in
+A ready-made composite including this application is defined e.g. in
 the ``glance-api-paste.ini`` file, looking like so::
 
-  [pipeline:glance-api]
-  pipeline = healthcheck versionnegotiation osprofiler unauthenticated-context rootapp
+  [composite:glance-api]
+  paste.composite_factory = glance.api:root_app_factory
+  /: apiv2app
+  /healthcheck: healthcheck
 
 For more information see
 `oslo.middleware <https://docs.openstack.org/oslo.middleware/latest/reference/api.html#oslo_middleware.Healthcheck>`_.
 
 Configuring supported disk formats
 ----------------------------------
```

### Comparing `glance-27.0.0.0b1/doc/source/configuration/sample-configuration.rst` & `glance-27.0.0.0b2/doc/source/configuration/sample-configuration.rst`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/doc/source/contributor/architecture.rst` & `glance-27.0.0.0b2/doc/source/contributor/architecture.rst`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/doc/source/contributor/blueprints.rst` & `glance-27.0.0.0b2/doc/source/contributor/blueprints.rst`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/doc/source/contributor/contributing.rst` & `glance-27.0.0.0b2/doc/source/contributor/contributing.rst`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/doc/source/contributor/core_reviewer_guidelines.rst` & `glance-27.0.0.0b2/doc/source/contributor/core_reviewer_guidelines.rst`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/doc/source/contributor/database_architecture.rst` & `glance-27.0.0.0b2/doc/source/contributor/database_architecture.rst`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/doc/source/contributor/database_migrations.rst` & `glance-27.0.0.0b2/doc/source/contributor/database_migrations.rst`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/doc/source/contributor/documentation.rst` & `glance-27.0.0.0b2/doc/source/contributor/documentation.rst`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/doc/source/contributor/domain_implementation.rst` & `glance-27.0.0.0b2/doc/source/contributor/domain_implementation.rst`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/doc/source/contributor/domain_model.rst` & `glance-27.0.0.0b2/doc/source/contributor/domain_model.rst`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/doc/source/contributor/gerrit.rst` & `glance-27.0.0.0b2/doc/source/contributor/gerrit.rst`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/doc/source/contributor/glance-groups.rst` & `glance-27.0.0.0b2/doc/source/contributor/glance-groups.rst`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/doc/source/contributor/index.rst` & `glance-27.0.0.0b2/doc/source/contributor/index.rst`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/doc/source/contributor/minor-code-changes.rst` & `glance-27.0.0.0b2/doc/source/contributor/minor-code-changes.rst`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/doc/source/contributor/refreshing-configs.rst` & `glance-27.0.0.0b2/doc/source/contributor/refreshing-configs.rst`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/doc/source/contributor/release-cpl.rst` & `glance-27.0.0.0b2/doc/source/contributor/release-cpl.rst`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/doc/source/contributor/release-notes.rst` & `glance-27.0.0.0b2/doc/source/contributor/release-notes.rst`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/doc/source/contributor/releasecycle.rst` & `glance-27.0.0.0b2/doc/source/contributor/releasecycle.rst`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/doc/source/glossary.rst` & `glance-27.0.0.0b2/doc/source/glossary.rst`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/doc/source/images/architecture.png` & `glance-27.0.0.0b2/doc/source/images/architecture.png`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/doc/source/images/glance_db.png` & `glance-27.0.0.0b2/doc/source/images/glance_db.png`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/doc/source/images/glance_layers.png` & `glance-27.0.0.0b2/doc/source/images/glance_layers.png`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/doc/source/images/image_status_transition.png` & `glance-27.0.0.0b2/doc/source/images/image_status_transition.png`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/doc/source/images/instance-life-1.png` & `glance-27.0.0.0b2/doc/source/images/instance-life-1.png`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/doc/source/images/instance-life-2.png` & `glance-27.0.0.0b2/doc/source/images/instance-life-2.png`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/doc/source/images/instance-life-3.png` & `glance-27.0.0.0b2/doc/source/images/instance-life-3.png`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/doc/source/images_src/architecture.graphml` & `glance-27.0.0.0b2/doc/source/images_src/architecture.graphml`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/doc/source/images_src/glance_db.graphml` & `glance-27.0.0.0b2/doc/source/images_src/glance_db.graphml`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/doc/source/images_src/glance_layers.graphml` & `glance-27.0.0.0b2/doc/source/images_src/glance_layers.graphml`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/doc/source/images_src/image_status_transition.dot` & `glance-27.0.0.0b2/doc/source/images_src/image_status_transition.dot`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/doc/source/index.rst` & `glance-27.0.0.0b2/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/doc/source/install/configure-quotas.rst` & `glance-27.0.0.0b2/doc/source/install/configure-quotas.rst`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/doc/source/install/get-started.rst` & `glance-27.0.0.0b2/doc/source/install/get-started.rst`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/doc/source/install/index.rst` & `glance-27.0.0.0b2/doc/source/install/index.rst`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/doc/source/install/install-debian.rst` & `glance-27.0.0.0b2/doc/source/install/install-debian.rst`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/doc/source/install/install-obs.rst` & `glance-27.0.0.0b2/doc/source/install/install-obs.rst`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/doc/source/install/install-rdo.rst` & `glance-27.0.0.0b2/doc/source/install/install-rdo.rst`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/doc/source/install/install-ubuntu.rst` & `glance-27.0.0.0b2/doc/source/install/install-ubuntu.rst`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/doc/source/install/register-quotas.rst` & `glance-27.0.0.0b2/doc/source/install/register-quotas.rst`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/doc/source/install/verify.rst` & `glance-27.0.0.0b2/doc/source/install/verify.rst`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/doc/source/user/common-image-properties.rst` & `glance-27.0.0.0b2/doc/source/user/common-image-properties.rst`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/doc/source/user/formats.rst` & `glance-27.0.0.0b2/doc/source/user/formats.rst`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/doc/source/user/glanceapi.rst` & `glance-27.0.0.0b2/doc/source/user/glanceapi.rst`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/doc/source/user/glanceclient.rst` & `glance-27.0.0.0b2/doc/source/user/glanceclient.rst`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/doc/source/user/glancemetadefcatalogapi.rst` & `glance-27.0.0.0b2/doc/source/user/glancemetadefcatalogapi.rst`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/doc/source/user/identifiers.rst` & `glance-27.0.0.0b2/doc/source/user/identifiers.rst`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/doc/source/user/metadefs-concepts.rst` & `glance-27.0.0.0b2/doc/source/user/metadefs-concepts.rst`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/doc/source/user/os_hash_algo.rst` & `glance-27.0.0.0b2/doc/source/user/os_hash_algo.rst`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/doc/source/user/signature.rst` & `glance-27.0.0.0b2/doc/source/user/signature.rst`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/doc/source/user/statuses.rst` & `glance-27.0.0.0b2/doc/source/user/statuses.rst`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/doc/test/redirect-tests.txt` & `glance-27.0.0.0b2/doc/test/redirect-tests.txt`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/etc/glance-api-paste.ini` & `glance-27.0.0.0b2/etc/glance-api-paste.ini`

 * *Files 25% similar despite different names*

```diff
@@ -1,44 +1,65 @@
-# Use this pipeline for no auth or image caching - DEFAULT
-[pipeline:glance-api]
-pipeline = cors healthcheck http_proxy_to_wsgi versionnegotiation osprofiler unauthenticated-context rootapp
-
-# Use this pipeline for image caching and no auth
-[pipeline:glance-api-caching]
-pipeline = cors healthcheck http_proxy_to_wsgi versionnegotiation osprofiler unauthenticated-context cache rootapp
-
-# Use this pipeline for caching w/ management interface but no auth
-[pipeline:glance-api-cachemanagement]
-pipeline = cors healthcheck http_proxy_to_wsgi versionnegotiation osprofiler unauthenticated-context cache cachemanage rootapp
-
-# Use this pipeline for keystone auth
-[pipeline:glance-api-keystone]
-pipeline = cors healthcheck http_proxy_to_wsgi versionnegotiation osprofiler authtoken context  rootapp
-
-# Use this pipeline for keystone auth with image caching
-[pipeline:glance-api-keystone+caching]
-pipeline = cors healthcheck http_proxy_to_wsgi versionnegotiation osprofiler authtoken context cache rootapp
-
-# Use this pipeline for keystone auth with caching and cache management
-[pipeline:glance-api-keystone+cachemanagement]
-pipeline = cors healthcheck http_proxy_to_wsgi versionnegotiation osprofiler authtoken context cache cachemanage rootapp
+# Use this composite for no auth or image caching - DEFAULT
+[composite:glance-api]
+paste.composite_factory = glance.api:root_app_factory
+/: api
+/healthcheck: healthcheck
+
+# Use this composite for image caching and no auth
+[composite:glance-api-caching]
+paste.composite_factory = glance.api:root_app_factory
+/: api
+/healthcheck: healthcheck
+
+# Use this composite for caching w/ management interface but no auth
+[composite:glance-api-cachemanagement]
+paste.composite_factory = glance.api:root_app_factory
+/: api
+/healthcheck: healthcheck
+
+# Use this composite for keystone auth
+[composite:glance-api-keystone]
+paste.composite_factory = glance.api:root_app_factory
+/: api
+/healthcheck: healthcheck
+
+# Use this composite for keystone auth with image caching
+[composite:glance-api-keystone+caching]
+paste.composite_factory = glance.api:root_app_factory
+/: api
+/healthcheck: healthcheck
+
+# Use this composite for keystone auth with caching and cache management
+[composite:glance-api-keystone+cachemanagement]
+paste.composite_factory = glance.api:root_app_factory
+/: api
+/healthchetck: healthcheck
+
+[composite:api]
+paste.composite_factory = glance.api:pipeline_factory
+default = cors http_proxy_to_wsgi versionnegotiation osprofiler unauthenticated-context rootapp
+caching = cors http_proxy_to_wsgi versionnegotiation osprofiler unauthenticated-context cache rootapp
+cachemanagement = cors http_proxy_to_wsgi versionnegotiation osprofiler unauthenticated-context cache cachemanage rootapp
+keystone = cors http_proxy_to_wsgi versionnegotiation osprofiler authtoken context rootapp
+keystone+caching = cors http_proxy_to_wsgi versionnegotiation osprofiler authtoken context cache rootapp
+keystone+cachemanagement = cors http_proxy_to_wsgi versionnegotiation osprofiler authtoken context cache cachemanage rootapp
 
 [composite:rootapp]
 paste.composite_factory = glance.api:root_app_factory
 /: apiversions
 /v2: apiv2app
 
 [app:apiversions]
 paste.app_factory = glance.api.versions:create_resource
 
 [app:apiv2app]
 paste.app_factory = glance.api.v2.router:API.factory
 
-[filter:healthcheck]
-paste.filter_factory = oslo_middleware:Healthcheck.factory
+[app:healthcheck]
+paste.app_factory = oslo_middleware:Healthcheck.app_factory
 backends = disable_by_file
 disable_by_file_path = /etc/glance/healthcheck_disable
 
 [filter:versionnegotiation]
 paste.filter_factory = glance.api.middleware.version_negotiation:VersionNegotiationFilter.factory
 
 [filter:cache]
```

### Comparing `glance-27.0.0.0b1/etc/glance-api.conf` & `glance-27.0.0.0b2/etc/glance-api.conf`

 * *Files 0% similar despite different names*

```diff
@@ -5682,16 +5682,18 @@
 # default. If this option is equal to False then the health check heartbeat will
 # inherit the execution model from the parent process. For example if the parent
 # process has monkey patched the stdlib by using eventlet/greenlet then the
 # heartbeat will be run through a green thread. This option should be set to
 # True only for the wsgi services. (boolean value)
 #heartbeat_in_pthread = false
 
-# How long to wait before reconnecting in response to an AMQP consumer cancel
-# notification. (floating point value)
+# How long to wait (in seconds) before reconnecting in response to an AMQP
+# consumer cancel notification. (floating point value)
+# Minimum value: 0.0
+# Maximum value: 4.5
 #kombu_reconnect_delay = 1.0
 
 # EXPERIMENTAL: Possible values are: gzip, bz2. If not set compression will not
 # be used. This option may not be available in future versions. (string value)
 #kombu_compression = <None>
 
 # How long to wait a missing client before abandoning to send it its replies.
@@ -5750,22 +5752,24 @@
 # (integer value)
 #rabbit_quorum_delivery_limit = 0
 
 # By default all messages are maintained in memory if a quorum queue grows in
 # length it can put memory pressure on a cluster. This option can limit the
 # number of messages in the quorum queue. Used only when rabbit_quorum_queue is
 # enabled, Default 0 which means dont set a limit. (integer value)
-#rabbit_quroum_max_memory_length = 0
+# Deprecated group/name - [oslo_messaging_rabbit]/rabbit_quroum_max_memory_length
+#rabbit_quorum_max_memory_length = 0
 
 # By default all messages are maintained in memory if a quorum queue grows in
 # length it can put memory pressure on a cluster. This option can limit the
 # number of memory bytes used by the quorum queue. Used only when
 # rabbit_quorum_queue is enabled, Default 0 which means dont set a limit.
 # (integer value)
-#rabbit_quroum_max_memory_bytes = 0
+# Deprecated group/name - [oslo_messaging_rabbit]/rabbit_quroum_max_memory_bytes
+#rabbit_quorum_max_memory_bytes = 0
 
 # Positive integer representing duration in seconds for queue TTL (x-expires).
 # Queues which are unused for the duration of the TTL are automatically deleted.
 # The parameter affects only reply and fanout queues. (integer value)
 # Minimum value: 1
 #rabbit_transient_queues_ttl = 1800
```

### Comparing `glance-27.0.0.0b1/etc/glance-cache.conf` & `glance-27.0.0.0b2/etc/glance-cache.conf`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/etc/glance-image-import.conf.sample` & `glance-27.0.0.0b2/etc/glance-image-import.conf.sample`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/etc/glance-manage.conf` & `glance-27.0.0.0b2/etc/glance-manage.conf`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/etc/glance-scrubber.conf` & `glance-27.0.0.0b2/etc/glance-scrubber.conf`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/etc/glance-swift.conf.sample` & `glance-27.0.0.0b2/etc/glance-swift.conf.sample`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/etc/metadefs/cim-processor-allocation-setting-data.json` & `glance-27.0.0.0b2/etc/metadefs/cim-processor-allocation-setting-data.json`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/etc/metadefs/cim-resource-allocation-setting-data.json` & `glance-27.0.0.0b2/etc/metadefs/cim-resource-allocation-setting-data.json`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/etc/metadefs/cim-storage-allocation-setting-data.json` & `glance-27.0.0.0b2/etc/metadefs/cim-storage-allocation-setting-data.json`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/etc/metadefs/cim-virtual-system-setting-data.json` & `glance-27.0.0.0b2/etc/metadefs/cim-virtual-system-setting-data.json`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/etc/metadefs/compute-aggr-disk-filter.json` & `glance-27.0.0.0b2/etc/metadefs/compute-aggr-disk-filter.json`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/etc/metadefs/compute-aggr-iops-filter.json` & `glance-27.0.0.0b2/etc/metadefs/compute-aggr-iops-filter.json`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/etc/metadefs/compute-aggr-num-instances.json` & `glance-27.0.0.0b2/etc/metadefs/compute-aggr-num-instances.json`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/etc/metadefs/compute-cpu-mode.json` & `glance-27.0.0.0b2/etc/metadefs/compute-cpu-mode.json`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/etc/metadefs/compute-cpu-pinning.json` & `glance-27.0.0.0b2/etc/metadefs/compute-cpu-pinning.json`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/etc/metadefs/compute-guest-memory-backing.json` & `glance-27.0.0.0b2/etc/metadefs/compute-guest-memory-backing.json`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/etc/metadefs/compute-guest-shutdown.json` & `glance-27.0.0.0b2/etc/metadefs/compute-guest-shutdown.json`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/etc/metadefs/compute-host-capabilities.json` & `glance-27.0.0.0b2/etc/metadefs/compute-host-capabilities.json`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/etc/metadefs/compute-hypervisor.json` & `glance-27.0.0.0b2/etc/metadefs/compute-hypervisor.json`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/etc/metadefs/compute-instance-data.json` & `glance-27.0.0.0b2/etc/metadefs/compute-instance-data.json`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/etc/metadefs/compute-libvirt-image.json` & `glance-27.0.0.0b2/etc/metadefs/compute-libvirt-image.json`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/etc/metadefs/compute-libvirt.json` & `glance-27.0.0.0b2/etc/metadefs/compute-libvirt.json`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/etc/metadefs/compute-quota.json` & `glance-27.0.0.0b2/etc/metadefs/compute-quota.json`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/etc/metadefs/compute-randomgen.json` & `glance-27.0.0.0b2/etc/metadefs/compute-randomgen.json`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/etc/metadefs/compute-vcputopology.json` & `glance-27.0.0.0b2/etc/metadefs/compute-vcputopology.json`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/etc/metadefs/compute-vmware-flavor.json` & `glance-27.0.0.0b2/etc/metadefs/compute-vmware-flavor.json`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/etc/metadefs/compute-vmware-quota-flavor.json` & `glance-27.0.0.0b2/etc/metadefs/compute-vmware-quota-flavor.json`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/etc/metadefs/compute-vmware.json` & `glance-27.0.0.0b2/etc/metadefs/compute-vmware.json`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/etc/metadefs/compute-vtpm-hw.json` & `glance-27.0.0.0b2/etc/metadefs/compute-vtpm-hw.json`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/etc/metadefs/compute-vtpm.json` & `glance-27.0.0.0b2/etc/metadefs/compute-vtpm.json`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/etc/metadefs/compute-watchdog.json` & `glance-27.0.0.0b2/etc/metadefs/compute-watchdog.json`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/etc/metadefs/compute-xenapi.json` & `glance-27.0.0.0b2/etc/metadefs/compute-xenapi.json`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/etc/metadefs/glance-common-image-props.json` & `glance-27.0.0.0b2/etc/metadefs/glance-common-image-props.json`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/etc/metadefs/image-signature-verification.json` & `glance-27.0.0.0b2/etc/metadefs/image-signature-verification.json`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/etc/metadefs/operating-system.json` & `glance-27.0.0.0b2/etc/metadefs/operating-system.json`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/etc/metadefs/software-databases.json` & `glance-27.0.0.0b2/etc/metadefs/software-databases.json`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/etc/metadefs/software-runtimes.json` & `glance-27.0.0.0b2/etc/metadefs/software-runtimes.json`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/etc/metadefs/software-webservers.json` & `glance-27.0.0.0b2/etc/metadefs/software-webservers.json`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/etc/metadefs/storage-volume-type.json` & `glance-27.0.0.0b2/etc/metadefs/storage-volume-type.json`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/etc/oslo-config-generator/glance-api.conf` & `glance-27.0.0.0b2/etc/oslo-config-generator/glance-api.conf`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/etc/property-protections-policies.conf.sample` & `glance-27.0.0.0b2/etc/property-protections-policies.conf.sample`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/etc/property-protections-roles.conf.sample` & `glance-27.0.0.0b2/etc/property-protections-roles.conf.sample`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/etc/schema-image.json` & `glance-27.0.0.0b2/etc/schema-image.json`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/api/__init__.py` & `glance-27.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/versions/rocky_contract02_empty.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,23 +1,25 @@
-# Copyright 2011-2012 OpenStack Foundation
+# Copyright (C) 2018 Verizon Wireless
 # All Rights Reserved.
 #
 #    Licensed under the Apache License, Version 2.0 (the "License"); you may
 #    not use this file except in compliance with the License. You may obtain
 #    a copy of the License at
 #
 #         http://www.apache.org/licenses/LICENSE-2.0
 #
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 #    WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 #    License for the specific language governing permissions and limitations
 #    under the License.
 
-from oslo_config import cfg
-import paste.urlmap
 
-CONF = cfg.CONF
+# revision identifiers, used by Alembic.
+revision = 'rocky_contract02'
+down_revision = 'rocky_contract01'
+branch_labels = None
+depends_on = 'rocky_expand02'
 
 
-def root_app_factory(loader, global_conf, **local_conf):
-    return paste.urlmap.urlmap_factory(loader, global_conf, **local_conf)
+def upgrade():
+    pass
```

### Comparing `glance-27.0.0.0b1/glance/api/common.py` & `glance-27.0.0.0b2/glance/api/common.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/api/middleware/cache.py` & `glance-27.0.0.0b2/glance/api/middleware/cache.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/api/middleware/cache_manage.py` & `glance-27.0.0.0b2/glance/api/middleware/cache_manage.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/api/middleware/context.py` & `glance-27.0.0.0b2/glance/api/middleware/context.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/api/middleware/gzip.py` & `glance-27.0.0.0b2/glance/api/middleware/gzip.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/api/middleware/version_negotiation.py` & `glance-27.0.0.0b2/glance/api/middleware/version_negotiation.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/api/policy.py` & `glance-27.0.0.0b2/glance/api/policy.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/api/property_protections.py` & `glance-27.0.0.0b2/glance/api/property_protections.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/api/v1/router.py` & `glance-27.0.0.0b2/glance/api/v1/router.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/api/v2/cached_images.py` & `glance-27.0.0.0b2/glance/api/v2/cached_images.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/api/v2/discovery.py` & `glance-27.0.0.0b2/glance/api/v2/discovery.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/api/v2/image_actions.py` & `glance-27.0.0.0b2/glance/api/v2/image_actions.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/api/v2/image_data.py` & `glance-27.0.0.0b2/glance/api/v2/image_data.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/api/v2/image_members.py` & `glance-27.0.0.0b2/glance/api/v2/image_members.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/api/v2/image_tags.py` & `glance-27.0.0.0b2/glance/api/v2/image_tags.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/api/v2/images.py` & `glance-27.0.0.0b2/glance/api/v2/images.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/api/v2/metadef_namespaces.py` & `glance-27.0.0.0b2/glance/api/v2/metadef_namespaces.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/api/v2/metadef_objects.py` & `glance-27.0.0.0b2/glance/api/v2/metadef_objects.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/api/v2/metadef_properties.py` & `glance-27.0.0.0b2/glance/api/v2/metadef_properties.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/api/v2/metadef_resource_types.py` & `glance-27.0.0.0b2/glance/api/v2/metadef_resource_types.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/api/v2/metadef_tags.py` & `glance-27.0.0.0b2/glance/api/v2/metadef_tags.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/api/v2/model/metadef_namespace.py` & `glance-27.0.0.0b2/glance/api/v2/model/metadef_namespace.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/api/v2/model/metadef_object.py` & `glance-27.0.0.0b2/glance/api/v2/model/metadef_object.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/api/v2/model/metadef_property_item_type.py` & `glance-27.0.0.0b2/glance/api/v2/model/metadef_property_item_type.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/api/v2/model/metadef_property_type.py` & `glance-27.0.0.0b2/glance/api/v2/model/metadef_property_type.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/api/v2/model/metadef_resource_type.py` & `glance-27.0.0.0b2/glance/api/v2/model/metadef_resource_type.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/api/v2/model/metadef_tag.py` & `glance-27.0.0.0b2/glance/api/v2/model/metadef_tag.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/api/v2/policy.py` & `glance-27.0.0.0b2/glance/api/v2/policy.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/api/v2/router.py` & `glance-27.0.0.0b2/glance/api/v2/router.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/api/v2/schemas.py` & `glance-27.0.0.0b2/glance/api/v2/schemas.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/api/v2/tasks.py` & `glance-27.0.0.0b2/glance/api/v2/tasks.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/api/versions.py` & `glance-27.0.0.0b2/glance/api/versions.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/async_/__init__.py` & `glance-27.0.0.0b2/glance/async_/__init__.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/async_/flows/_internal_plugins/__init__.py` & `glance-27.0.0.0b2/glance/async_/flows/_internal_plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/async_/flows/_internal_plugins/base_download.py` & `glance-27.0.0.0b2/glance/async_/flows/_internal_plugins/base_download.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,27 +16,25 @@
 
 import abc
 
 import glance_store as store_api
 from glance_store import backend
 from oslo_config import cfg
 from oslo_log import log as logging
-import six
 from taskflow import task
 
 from glance.common import exception
 from glance.i18n import _, _LE
 
 LOG = logging.getLogger(__name__)
 
 CONF = cfg.CONF
 
 
-@six.add_metaclass(abc.ABCMeta)
-class BaseDownload(task.Task):
+class BaseDownload(task.Task, metaclass=abc.ABCMeta):
 
     default_provides = 'file_uri'
 
     def __init__(self, task_id, task_type, action_wrapper, stores,
                  plugin_name):
         self.task_id = task_id
         self.task_type = task_type
```

### Comparing `glance-27.0.0.0b1/glance/async_/flows/_internal_plugins/copy_image.py` & `glance-27.0.0.0b2/glance/async_/flows/_internal_plugins/copy_image.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/async_/flows/_internal_plugins/glance_download.py` & `glance-27.0.0.0b2/glance/async_/flows/_internal_plugins/glance_download.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/async_/flows/_internal_plugins/web_download.py` & `glance-27.0.0.0b2/glance/async_/flows/_internal_plugins/web_download.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/async_/flows/api_image_import.py` & `glance-27.0.0.0b2/glance/async_/flows/api_image_import.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/async_/flows/base_import.py` & `glance-27.0.0.0b2/glance/async_/flows/base_import.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/async_/flows/convert.py` & `glance-27.0.0.0b2/glance/async_/flows/convert.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/async_/flows/introspect.py` & `glance-27.0.0.0b2/glance/async_/flows/introspect.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/async_/flows/ovf_process.py` & `glance-27.0.0.0b2/glance/async_/flows/ovf_process.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/async_/flows/plugins/__init__.py` & `glance-27.0.0.0b2/glance/async_/flows/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/async_/flows/plugins/image_conversion.py` & `glance-27.0.0.0b2/glance/async_/flows/plugins/image_conversion.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/async_/flows/plugins/image_decompression.py` & `glance-27.0.0.0b2/glance/async_/flows/plugins/image_decompression.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/async_/flows/plugins/inject_image_metadata.py` & `glance-27.0.0.0b2/glance/async_/flows/plugins/inject_image_metadata.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/async_/flows/plugins/no_op.py` & `glance-27.0.0.0b2/glance/async_/flows/plugins/no_op.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/async_/flows/plugins/plugin_opts.py` & `glance-27.0.0.0b2/glance/async_/flows/plugins/plugin_opts.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/async_/taskflow_executor.py` & `glance-27.0.0.0b2/glance/async_/taskflow_executor.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/async_/utils.py` & `glance-27.0.0.0b2/glance/async_/utils.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/cmd/api.py` & `glance-27.0.0.0b2/glance/cmd/api.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/cmd/cache_cleaner.py` & `glance-27.0.0.0b2/glance/cmd/cache_cleaner.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/cmd/cache_manage.py` & `glance-27.0.0.0b2/glance/cmd/cache_manage.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/cmd/cache_prefetcher.py` & `glance-27.0.0.0b2/glance/cmd/cache_prefetcher.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/cmd/cache_pruner.py` & `glance-27.0.0.0b2/glance/cmd/cache_pruner.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/cmd/control.py` & `glance-27.0.0.0b2/glance/cmd/control.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/cmd/manage.py` & `glance-27.0.0.0b2/glance/cmd/manage.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/cmd/replicator.py` & `glance-27.0.0.0b2/glance/cmd/replicator.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/cmd/scrubber.py` & `glance-27.0.0.0b2/glance/cmd/scrubber.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/cmd/status.py` & `glance-27.0.0.0b2/glance/cmd/status.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/common/auth.py` & `glance-27.0.0.0b2/glance/common/auth.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/common/client.py` & `glance-27.0.0.0b2/glance/common/client.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/common/config.py` & `glance-27.0.0.0b2/glance/common/config.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/common/crypt.py` & `glance-27.0.0.0b2/glance/common/crypt.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/common/exception.py` & `glance-27.0.0.0b2/glance/common/exception.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/common/format_inspector.py` & `glance-27.0.0.0b2/glance/common/format_inspector.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/common/location_strategy/__init__.py` & `glance-27.0.0.0b2/glance/common/location_strategy/__init__.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/common/location_strategy/location_order.py` & `glance-27.0.0.0b2/glance/common/location_strategy/location_order.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/common/location_strategy/store_type.py` & `glance-27.0.0.0b2/glance/common/location_strategy/store_type.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/common/property_utils.py` & `glance-27.0.0.0b2/glance/common/property_utils.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/common/removed_config.py` & `glance-27.0.0.0b2/glance/common/removed_config.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/common/scripts/__init__.py` & `glance-27.0.0.0b2/glance/common/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/common/scripts/api_image_import/main.py` & `glance-27.0.0.0b2/glance/common/scripts/api_image_import/main.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/common/scripts/image_import/main.py` & `glance-27.0.0.0b2/glance/common/scripts/image_import/main.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/common/scripts/utils.py` & `glance-27.0.0.0b2/glance/common/scripts/utils.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/common/store_utils.py` & `glance-27.0.0.0b2/glance/common/store_utils.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/common/swift_store_utils.py` & `glance-27.0.0.0b2/glance/common/swift_store_utils.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/common/timeutils.py` & `glance-27.0.0.0b2/glance/common/timeutils.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/common/trust_auth.py` & `glance-27.0.0.0b2/glance/common/trust_auth.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/common/utils.py` & `glance-27.0.0.0b2/glance/common/utils.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/common/wsgi.py` & `glance-27.0.0.0b2/glance/common/wsgi.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/common/wsgi_app.py` & `glance-27.0.0.0b2/glance/common/wsgi_app.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/common/wsme_utils.py` & `glance-27.0.0.0b2/glance/common/wsme_utils.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/context.py` & `glance-27.0.0.0b2/glance/context.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/db/__init__.py` & `glance-27.0.0.0b2/glance/db/__init__.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/db/metadata.py` & `glance-27.0.0.0b2/glance/db/metadata.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/db/migration.py` & `glance-27.0.0.0b2/glance/db/migration.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/db/simple/api.py` & `glance-27.0.0.0b2/glance/db/simple/api.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/db/sqlalchemy/alembic_migrations/__init__.py` & `glance-27.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/__init__.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/db/sqlalchemy/alembic_migrations/add_artifacts_tables.py` & `glance-27.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/add_artifacts_tables.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/db/sqlalchemy/alembic_migrations/add_images_tables.py` & `glance-27.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/add_images_tables.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/db/sqlalchemy/alembic_migrations/add_metadefs_tables.py` & `glance-27.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/add_metadefs_tables.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/db/sqlalchemy/alembic_migrations/add_tasks_tables.py` & `glance-27.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/add_tasks_tables.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/db/sqlalchemy/alembic_migrations/alembic.ini` & `glance-27.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/alembic.ini`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/db/sqlalchemy/alembic_migrations/data_migrations/2023_1_migrate01_empty.py` & `glance-27.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/data_migrations/2023_1_migrate01_empty.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/db/sqlalchemy/alembic_migrations/data_migrations/__init__.py` & `glance-27.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/data_migrations/__init__.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/db/sqlalchemy/alembic_migrations/data_migrations/ocata_migrate01_community_images.py` & `glance-27.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/data_migrations/ocata_migrate01_community_images.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/db/sqlalchemy/alembic_migrations/data_migrations/pike_migrate01_empty.py` & `glance-27.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/data_migrations/pike_migrate01_empty.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/db/sqlalchemy/alembic_migrations/data_migrations/queens_migrate01_empty.py` & `glance-27.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/data_migrations/queens_migrate01_empty.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/db/sqlalchemy/alembic_migrations/data_migrations/rocky_migrate01_empty.py` & `glance-27.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/data_migrations/rocky_migrate01_empty.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/db/sqlalchemy/alembic_migrations/data_migrations/rocky_migrate02_empty.py` & `glance-27.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/data_migrations/rocky_migrate02_empty.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/db/sqlalchemy/alembic_migrations/data_migrations/train_migrate01_backend_to_store.py` & `glance-27.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/data_migrations/train_migrate01_backend_to_store.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/db/sqlalchemy/alembic_migrations/data_migrations/ussuri_migrate01_empty.py` & `glance-27.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/data_migrations/ussuri_migrate01_empty.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/db/sqlalchemy/alembic_migrations/data_migrations/wallaby_migrate01_empty.py` & `glance-27.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/data_migrations/wallaby_migrate01_empty.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/db/sqlalchemy/alembic_migrations/data_migrations/xena_migrate01_empty.py` & `glance-27.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/data_migrations/xena_migrate01_empty.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/db/sqlalchemy/alembic_migrations/data_migrations/yoga_migrate01_empty.py` & `glance-27.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/data_migrations/yoga_migrate01_empty.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/db/sqlalchemy/alembic_migrations/data_migrations/zed_migrate01_empty.py` & `glance-27.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/data_migrations/zed_migrate01_empty.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/db/sqlalchemy/alembic_migrations/env.py` & `glance-27.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/env.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/db/sqlalchemy/alembic_migrations/migrate.cfg` & `glance-27.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/migrate.cfg`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/db/sqlalchemy/alembic_migrations/versions/2023_1_contract01_empty.py` & `glance-27.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/versions/2023_1_contract01_empty.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/db/sqlalchemy/alembic_migrations/versions/2023_1_expand01_empty.py` & `glance-27.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/versions/2023_1_expand01_empty.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/db/sqlalchemy/alembic_migrations/versions/liberty_initial.py` & `glance-27.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/versions/liberty_initial.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/db/sqlalchemy/alembic_migrations/versions/mitaka01_add_image_created_updated_idx.py` & `glance-27.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/versions/mitaka01_add_image_created_updated_idx.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/db/sqlalchemy/alembic_migrations/versions/mitaka02_update_metadef_os_nova_server.py` & `glance-27.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/versions/mitaka02_update_metadef_os_nova_server.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/db/sqlalchemy/alembic_migrations/versions/ocata_contract01_drop_is_public.py` & `glance-27.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/versions/ocata_contract01_drop_is_public.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/db/sqlalchemy/alembic_migrations/versions/ocata_expand01_add_visibility.py` & `glance-27.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/versions/ocata_expand01_add_visibility.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/db/sqlalchemy/alembic_migrations/versions/pike_contract01_drop_artifacts_tables.py` & `glance-27.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/versions/pike_contract01_drop_artifacts_tables.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/db/sqlalchemy/alembic_migrations/versions/pike_expand01_empty.py` & `glance-27.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/versions/pike_expand01_empty.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/db/sqlalchemy/alembic_migrations/versions/queens_contract01_empty.py` & `glance-27.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/versions/queens_contract01_empty.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/db/sqlalchemy/alembic_migrations/versions/queens_expand01_empty.py` & `glance-27.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/versions/queens_expand01_empty.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/db/sqlalchemy/alembic_migrations/versions/rocky_contract01_empty.py` & `glance-27.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/versions/rocky_contract01_empty.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/db/sqlalchemy/alembic_migrations/versions/rocky_contract02_empty.py` & `glance-27.0.0.0b2/glance/version.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,19 @@
-# Copyright (C) 2018 Verizon Wireless
-# All Rights Reserved.
+#    Copyright 2012 OpenStack Foundation
 #
 #    Licensed under the Apache License, Version 2.0 (the "License"); you may
 #    not use this file except in compliance with the License. You may obtain
 #    a copy of the License at
 #
 #         http://www.apache.org/licenses/LICENSE-2.0
 #
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 #    WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 #    License for the specific language governing permissions and limitations
 #    under the License.
 
 
-# revision identifiers, used by Alembic.
-revision = 'rocky_contract02'
-down_revision = 'rocky_contract01'
-branch_labels = None
-depends_on = 'rocky_expand02'
+import pbr.version
 
-
-def upgrade():
-    pass
+version_info = pbr.version.VersionInfo('glance')
+version_string = version_info.version_string
```

### Comparing `glance-27.0.0.0b1/glance/db/sqlalchemy/alembic_migrations/versions/rocky_expand01_add_os_hidden.py` & `glance-27.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/versions/rocky_expand01_add_os_hidden.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/db/sqlalchemy/alembic_migrations/versions/rocky_expand02_add_os_hash_.py` & `glance-27.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/versions/rocky_expand02_add_os_hash_.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/db/sqlalchemy/alembic_migrations/versions/train_contract01_empty.py` & `glance-27.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/versions/train_contract01_empty.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/db/sqlalchemy/alembic_migrations/versions/train_expand01_empty.py` & `glance-27.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/versions/train_expand01_empty.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/db/sqlalchemy/alembic_migrations/versions/ussuri_contract01_empty.py` & `glance-27.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/versions/ussuri_contract01_empty.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/db/sqlalchemy/alembic_migrations/versions/ussuri_expand01_empty.py` & `glance-27.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/versions/ussuri_expand01_empty.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/db/sqlalchemy/alembic_migrations/versions/wallaby_contract01_empty.py` & `glance-27.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/versions/wallaby_contract01_empty.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/db/sqlalchemy/alembic_migrations/versions/wallaby_expand01_add_user_imageid_requestid_to_tasks.py` & `glance-27.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/versions/wallaby_expand01_add_user_imageid_requestid_to_tasks.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/db/sqlalchemy/alembic_migrations/versions/xena_contract01_empty.py` & `glance-27.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/versions/xena_contract01_empty.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/db/sqlalchemy/alembic_migrations/versions/xena_expand01_empty.py` & `glance-27.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/versions/xena_expand01_empty.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/db/sqlalchemy/alembic_migrations/versions/yoga_contract01_empty.py` & `glance-27.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/versions/yoga_contract01_empty.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/db/sqlalchemy/alembic_migrations/versions/yoga_expand01_empty.py` & `glance-27.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/versions/yoga_expand01_empty.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/db/sqlalchemy/alembic_migrations/versions/zed_contract01_empty.py` & `glance-27.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/versions/zed_contract01_empty.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/db/sqlalchemy/alembic_migrations/versions/zed_expand01_empty.py` & `glance-27.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/versions/zed_expand01_empty.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/db/sqlalchemy/api.py` & `glance-27.0.0.0b2/glance/db/sqlalchemy/api.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/db/sqlalchemy/metadata.py` & `glance-27.0.0.0b2/glance/db/sqlalchemy/metadata.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/db/sqlalchemy/metadef_api/namespace.py` & `glance-27.0.0.0b2/glance/db/sqlalchemy/metadef_api/namespace.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/db/sqlalchemy/metadef_api/object.py` & `glance-27.0.0.0b2/glance/db/sqlalchemy/metadef_api/object.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/db/sqlalchemy/metadef_api/property.py` & `glance-27.0.0.0b2/glance/db/sqlalchemy/metadef_api/property.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/db/sqlalchemy/metadef_api/resource_type.py` & `glance-27.0.0.0b2/glance/db/sqlalchemy/metadef_api/resource_type.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/db/sqlalchemy/metadef_api/resource_type_association.py` & `glance-27.0.0.0b2/glance/db/sqlalchemy/metadef_api/resource_type_association.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/db/sqlalchemy/metadef_api/tag.py` & `glance-27.0.0.0b2/glance/db/sqlalchemy/metadef_api/tag.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/db/sqlalchemy/metadef_api/utils.py` & `glance-27.0.0.0b2/glance/db/sqlalchemy/metadef_api/utils.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/db/sqlalchemy/models.py` & `glance-27.0.0.0b2/glance/db/sqlalchemy/models.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/db/sqlalchemy/models_metadef.py` & `glance-27.0.0.0b2/glance/db/sqlalchemy/models_metadef.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/db/sqlalchemy/schema.py` & `glance-27.0.0.0b2/glance/db/sqlalchemy/schema.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/db/utils.py` & `glance-27.0.0.0b2/glance/db/utils.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/domain/__init__.py` & `glance-27.0.0.0b2/glance/domain/__init__.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/domain/proxy.py` & `glance-27.0.0.0b2/glance/domain/proxy.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/gateway.py` & `glance-27.0.0.0b2/glance/gateway.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/hacking/checks.py` & `glance-27.0.0.0b2/glance/hacking/checks.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/housekeeping.py` & `glance-27.0.0.0b2/glance/housekeeping.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/i18n.py` & `glance-27.0.0.0b2/glance/i18n.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/image_cache/__init__.py` & `glance-27.0.0.0b2/glance/image_cache/__init__.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/image_cache/base.py` & `glance-27.0.0.0b2/glance/image_cache/base.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/image_cache/cleaner.py` & `glance-27.0.0.0b2/glance/image_cache/cleaner.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/image_cache/client.py` & `glance-27.0.0.0b2/glance/image_cache/client.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/image_cache/drivers/base.py` & `glance-27.0.0.0b2/glance/image_cache/drivers/base.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/image_cache/drivers/sqlite.py` & `glance-27.0.0.0b2/glance/image_cache/drivers/sqlite.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/image_cache/drivers/xattr.py` & `glance-27.0.0.0b2/glance/image_cache/drivers/xattr.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/image_cache/prefetcher.py` & `glance-27.0.0.0b2/glance/image_cache/prefetcher.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/image_cache/pruner.py` & `glance-27.0.0.0b2/glance/image_cache/pruner.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/locale/de/LC_MESSAGES/glance.po` & `glance-27.0.0.0b2/glance/locale/de/LC_MESSAGES/glance.po`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/locale/en_GB/LC_MESSAGES/glance.po` & `glance-27.0.0.0b2/glance/locale/en_GB/LC_MESSAGES/glance.po`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/locale/es/LC_MESSAGES/glance.po` & `glance-27.0.0.0b2/glance/locale/es/LC_MESSAGES/glance.po`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/locale/fr/LC_MESSAGES/glance.po` & `glance-27.0.0.0b2/glance/locale/fr/LC_MESSAGES/glance.po`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/locale/it/LC_MESSAGES/glance.po` & `glance-27.0.0.0b2/glance/locale/it/LC_MESSAGES/glance.po`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/locale/ja/LC_MESSAGES/glance.po` & `glance-27.0.0.0b2/glance/locale/ja/LC_MESSAGES/glance.po`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/locale/ko_KR/LC_MESSAGES/glance.po` & `glance-27.0.0.0b2/glance/locale/ko_KR/LC_MESSAGES/glance.po`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/locale/pt_BR/LC_MESSAGES/glance.po` & `glance-27.0.0.0b2/glance/locale/pt_BR/LC_MESSAGES/glance.po`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/locale/ru/LC_MESSAGES/glance.po` & `glance-27.0.0.0b2/glance/locale/ru/LC_MESSAGES/glance.po`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/locale/tr_TR/LC_MESSAGES/glance.po` & `glance-27.0.0.0b2/glance/locale/tr_TR/LC_MESSAGES/glance.po`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/locale/zh_CN/LC_MESSAGES/glance.po` & `glance-27.0.0.0b2/glance/locale/zh_CN/LC_MESSAGES/glance.po`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/locale/zh_TW/LC_MESSAGES/glance.po` & `glance-27.0.0.0b2/glance/locale/zh_TW/LC_MESSAGES/glance.po`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/location.py` & `glance-27.0.0.0b2/glance/location.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/notifier.py` & `glance-27.0.0.0b2/glance/notifier.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/opts.py` & `glance-27.0.0.0b2/glance/opts.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/policies/__init__.py` & `glance-27.0.0.0b2/glance/policies/__init__.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/policies/base.py` & `glance-27.0.0.0b2/glance/policies/base.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/policies/cache.py` & `glance-27.0.0.0b2/glance/policies/cache.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/policies/discovery.py` & `glance-27.0.0.0b2/glance/policies/discovery.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/policies/image.py` & `glance-27.0.0.0b2/glance/policies/image.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/policies/metadef.py` & `glance-27.0.0.0b2/glance/policies/metadef.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/policies/tasks.py` & `glance-27.0.0.0b2/glance/policies/tasks.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/quota/__init__.py` & `glance-27.0.0.0b2/glance/quota/__init__.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/quota/keystone.py` & `glance-27.0.0.0b2/glance/quota/keystone.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/schema.py` & `glance-27.0.0.0b2/glance/schema.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/scrubber.py` & `glance-27.0.0.0b2/glance/scrubber.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/tests/__init__.py` & `glance-27.0.0.0b2/glance/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/tests/etc/glance-swift.conf` & `glance-27.0.0.0b2/glance/tests/etc/glance-swift.conf`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/tests/etc/property-protections-policies.conf` & `glance-27.0.0.0b2/glance/tests/etc/property-protections-policies.conf`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/tests/etc/property-protections.conf` & `glance-27.0.0.0b2/glance/tests/etc/property-protections.conf`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/tests/functional/__init__.py` & `glance-27.0.0.0b2/glance/tests/functional/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -464,57 +464,79 @@
 store_type_preference = %(store_type_location_strategy_preference)s
 [glance_store]
 filesystem_store_datadir=%(image_dir)s
 default_store = %(default_store)s
 [import_filtering_opts]
 allowed_ports = []
 """
-        self.paste_conf_base = """[pipeline:glance-api]
+        self.paste_conf_base = """[composite:glance-api]
+paste.composite_factory = glance.api:root_app_factory
+/: api
+/healthcheck: healthcheck
+
+[pipeline:api]
 pipeline =
     cors
-    healthcheck
     versionnegotiation
     gzip
     unauthenticated-context
     rootapp
 
-[pipeline:glance-api-caching]
-pipeline = cors healthcheck versionnegotiation gzip context
- cache rootapp
+[composite:glance-api-caching]
+paste.composite_factory = glance.api:root_app_factory
+/: api-caching
+/healthcheck: healthcheck
+
+[pipeline:api-caching]
+pipeline = cors versionnegotiation gzip context cache rootapp
+
+[composite:glance-api-cachemanagement]
+paste.composite_factory = glance.api:root_app_factory
+/: api-cachemanagement
+/healthcheck: healthcheck
 
-[pipeline:glance-api-cachemanagement]
+[pipeline:api-cachemanagement]
 pipeline =
     cors
-    healthcheck
     versionnegotiation
     gzip
     unauthenticated-context
     cache
     cache_manage
     rootapp
 
-[pipeline:glance-api-fakeauth]
-pipeline = cors healthcheck versionnegotiation gzip fakeauth context rootapp
+[composite:glance-api-fakeauth]
+paste.composite_factory = glance.api:root_app_factory
+/: api-fakeauth
+/healthcheck: healthcheck
+
+[pipeline:api-fakeauth]
+pipeline = cors versionnegotiation gzip fakeauth context rootapp
+
+[composite:glance-api-noauth]
+paste.composite_factory = glance.api:root_app_factory
+/: api-noauth
+/healthcheck: healthcheck
 
-[pipeline:glance-api-noauth]
-pipeline = cors healthcheck versionnegotiation gzip context rootapp
+[pipeline:api-noauth]
+pipeline = cors versionnegotiation gzip context rootapp
 
 [composite:rootapp]
 paste.composite_factory = glance.api:root_app_factory
 /: apiversions
 /v2: apiv2app
 
 [app:apiversions]
 paste.app_factory = glance.api.versions:create_resource
 
 [app:apiv2app]
 paste.app_factory = glance.api.v2.router:API.factory
 
-[filter:healthcheck]
-paste.filter_factory = oslo_middleware:Healthcheck.factory
+[app:healthcheck]
+paste.app_factory = oslo_middleware:Healthcheck.app_factory
 backends = disable_by_file
 disable_by_file_path = %(disable_path)s
 
 [filter:versionnegotiation]
 paste.filter_factory = glance.api.middleware.version_negotiation:VersionNegotiationFilter.factory
 
 [filter:gzip]
@@ -639,57 +661,79 @@
 [file3]
 filesystem_store_datadir=%(image_dir_backend_3)s
 [import_filtering_opts]
 allowed_ports = []
 [os_glance_staging_store]
 filesystem_store_datadir=%(staging_dir)s
 """
-        self.paste_conf_base = """[pipeline:glance-api]
+        self.paste_conf_base = """[composite:glance-api]
+paste.composite_factory = glance.api:root_app_factory
+/: api
+/healthcheck: healthcheck
+
+[pipeline:api]
 pipeline =
     cors
-    healthcheck
     versionnegotiation
     gzip
     unauthenticated-context
     rootapp
 
-[pipeline:glance-api-caching]
-pipeline = cors healthcheck versionnegotiation gzip unauthenticated-context
- cache rootapp
+[composite:glance-api-caching]
+paste.composite_factory = glance.api:root_app_factory
+/: api-caching
+/healthcheck: healthcheck
+
+[pipeline:api-caching]
+pipeline = cors versionnegotiation gzip unauthenticated-context cache rootapp
+
+[composite:glance-api-cachemanagement]
+paste.composite_factory = glance.api:root_app_factory
+/: api-cachemanagement
+/healthcheck: healthcheck
 
-[pipeline:glance-api-cachemanagement]
+[pipeline:api-cachemanagement]
 pipeline =
     cors
-    healthcheck
     versionnegotiation
     gzip
     unauthenticated-context
     cache
     cache_manage
     rootapp
 
-[pipeline:glance-api-fakeauth]
-pipeline = cors healthcheck versionnegotiation gzip fakeauth context rootapp
+[composite:glance-api-fakeauth]
+paste.composite_factory = glance.api:root_app_factory
+/: api-fakeauth
+/healthcheck: healthcheck
+
+[pipeline:api-fakeauth]
+pipeline = cors versionnegotiation gzip fakeauth context rootapp
+
+[composite:glance-api-noauth]
+paste.composite_factory = glance.api:root_app_factory
+/: api-noauth
+/healthcheck: healthcheck
 
-[pipeline:glance-api-noauth]
-pipeline = cors healthcheck versionnegotiation gzip context rootapp
+[pipeline:api-noauth]
+pipeline = cors versionnegotiation gzip context rootapp
 
 [composite:rootapp]
 paste.composite_factory = glance.api:root_app_factory
 /: apiversions
 /v2: apiv2app
 
 [app:apiversions]
 paste.app_factory = glance.api.versions:create_resource
 
 [app:apiv2app]
 paste.app_factory = glance.api.v2.router:API.factory
 
-[filter:healthcheck]
-paste.filter_factory = oslo_middleware:Healthcheck.factory
+[app:healthcheck]
+paste.app_factory = oslo_middleware:Healthcheck.app_factory
 backends = disable_by_file
 disable_by_file_path = %(disable_path)s
 
 [filter:versionnegotiation]
 paste.filter_factory = glance.api.middleware.version_negotiation:VersionNegotiationFilter.factory
 
 [filter:gzip]
```

### Comparing `glance-27.0.0.0b1/glance/tests/functional/db/__init__.py` & `glance-27.0.0.0b2/glance/tests/functional/db/__init__.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/tests/functional/db/base.py` & `glance-27.0.0.0b2/glance/tests/functional/db/base.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/tests/functional/db/base_metadef.py` & `glance-27.0.0.0b2/glance/tests/functional/db/base_metadef.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/tests/functional/db/migrations/test_mitaka01.py` & `glance-27.0.0.0b2/glance/tests/functional/db/migrations/test_mitaka01.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/tests/functional/db/migrations/test_mitaka02.py` & `glance-27.0.0.0b2/glance/tests/functional/db/migrations/test_mitaka02.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/tests/functional/db/migrations/test_ocata_contract01.py` & `glance-27.0.0.0b2/glance/tests/functional/db/migrations/test_ocata_contract01.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/tests/functional/db/migrations/test_ocata_expand01.py` & `glance-27.0.0.0b2/glance/tests/functional/db/migrations/test_ocata_expand01.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/tests/functional/db/migrations/test_ocata_migrate01.py` & `glance-27.0.0.0b2/glance/tests/functional/db/migrations/test_ocata_migrate01.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/tests/functional/db/migrations/test_pike_contract01.py` & `glance-27.0.0.0b2/glance/tests/functional/db/migrations/test_pike_contract01.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/tests/functional/db/migrations/test_pike_expand01.py` & `glance-27.0.0.0b2/glance/tests/functional/db/migrations/test_pike_expand01.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/tests/functional/db/migrations/test_pike_migrate01.py` & `glance-27.0.0.0b2/glance/tests/functional/db/migrations/test_pike_migrate01.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/tests/functional/db/migrations/test_rocky_expand01.py` & `glance-27.0.0.0b2/glance/tests/functional/db/migrations/test_rocky_expand01.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/tests/functional/db/migrations/test_rocky_expand02.py` & `glance-27.0.0.0b2/glance/tests/functional/db/migrations/test_rocky_expand02.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/tests/functional/db/migrations/test_train_migrate01.py` & `glance-27.0.0.0b2/glance/tests/functional/db/migrations/test_train_migrate01.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/tests/functional/db/migrations/test_wallaby_expand01.py` & `glance-27.0.0.0b2/glance/tests/functional/db/migrations/test_wallaby_expand01.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/tests/functional/db/test_migrations.py` & `glance-27.0.0.0b2/glance/tests/functional/db/test_migrations.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/tests/functional/db/test_sqlalchemy.py` & `glance-27.0.0.0b2/glance/tests/functional/db/test_sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/tests/functional/ft_utils.py` & `glance-27.0.0.0b2/glance/tests/functional/ft_utils.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/tests/functional/serial/test_scrubber.py` & `glance-27.0.0.0b2/glance/tests/functional/serial/test_scrubber.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/tests/functional/store_utils.py` & `glance-27.0.0.0b2/glance/tests/functional/store_utils.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/tests/functional/test_api.py` & `glance-27.0.0.0b2/glance/tests/functional/test_api.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/tests/functional/test_cache_middleware.py` & `glance-27.0.0.0b2/glance/tests/functional/test_cache_middleware.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/tests/functional/test_client_exceptions.py` & `glance-27.0.0.0b2/glance/tests/functional/test_client_exceptions.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/tests/functional/test_client_redirects.py` & `glance-27.0.0.0b2/glance/tests/functional/test_client_redirects.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/tests/functional/test_cors_middleware.py` & `glance-27.0.0.0b2/glance/tests/functional/test_cors_middleware.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/tests/functional/test_glance_manage.py` & `glance-27.0.0.0b2/glance/tests/functional/test_glance_manage.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/tests/functional/test_gzip_middleware.py` & `glance-27.0.0.0b2/glance/tests/functional/test_gzip_middleware.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/tests/functional/test_healthcheck_middleware.py` & `glance-27.0.0.0b2/glance/tests/functional/test_healthcheck_middleware.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/tests/functional/test_logging.py` & `glance-27.0.0.0b2/glance/tests/functional/test_logging.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/tests/functional/test_reload.py` & `glance-27.0.0.0b2/glance/tests/functional/test_reload.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/tests/functional/test_sqlite.py` & `glance-27.0.0.0b2/glance/tests/functional/test_sqlite.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/tests/functional/test_wsgi.py` & `glance-27.0.0.0b2/glance/tests/functional/test_wsgi.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/tests/functional/v2/metadef_base.py` & `glance-27.0.0.0b2/glance/tests/functional/v2/metadef_base.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/tests/functional/v2/test_cache_api.py` & `glance-27.0.0.0b2/glance/tests/functional/v2/test_cache_api.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/tests/functional/v2/test_cache_api_policy.py` & `glance-27.0.0.0b2/glance/tests/functional/v2/test_cache_api_policy.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/tests/functional/v2/test_discovery.py` & `glance-27.0.0.0b2/glance/tests/functional/v2/test_discovery.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/tests/functional/v2/test_images.py` & `glance-27.0.0.0b2/glance/tests/functional/v2/test_images.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/tests/functional/v2/test_images_api_policy.py` & `glance-27.0.0.0b2/glance/tests/functional/v2/test_images_api_policy.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/tests/functional/v2/test_images_import_locking.py` & `glance-27.0.0.0b2/glance/tests/functional/v2/test_images_import_locking.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/tests/functional/v2/test_legacy_update_cinder_store.py` & `glance-27.0.0.0b2/glance/tests/functional/v2/test_legacy_update_cinder_store.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/tests/functional/v2/test_member_api_policy.py` & `glance-27.0.0.0b2/glance/tests/functional/v2/test_member_api_policy.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/tests/functional/v2/test_metadef_namespace_api_policy.py` & `glance-27.0.0.0b2/glance/tests/functional/v2/test_metadef_namespace_api_policy.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/tests/functional/v2/test_metadef_namespaces.py` & `glance-27.0.0.0b2/glance/tests/functional/v2/test_metadef_namespaces.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/tests/functional/v2/test_metadef_object_api_policy.py` & `glance-27.0.0.0b2/glance/tests/functional/v2/test_metadef_object_api_policy.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/tests/functional/v2/test_metadef_objects.py` & `glance-27.0.0.0b2/glance/tests/functional/v2/test_metadef_objects.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/tests/functional/v2/test_metadef_properties.py` & `glance-27.0.0.0b2/glance/tests/functional/v2/test_metadef_properties.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/tests/functional/v2/test_metadef_property_api_policy.py` & `glance-27.0.0.0b2/glance/tests/functional/v2/test_metadef_property_api_policy.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/tests/functional/v2/test_metadef_resourcetype_api_policy.py` & `glance-27.0.0.0b2/glance/tests/functional/v2/test_metadef_resourcetype_api_policy.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/tests/functional/v2/test_metadef_resourcetypes.py` & `glance-27.0.0.0b2/glance/tests/functional/v2/test_metadef_resourcetypes.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/tests/functional/v2/test_metadef_tag_api_policy.py` & `glance-27.0.0.0b2/glance/tests/functional/v2/test_metadef_tag_api_policy.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/tests/functional/v2/test_metadef_tags.py` & `glance-27.0.0.0b2/glance/tests/functional/v2/test_metadef_tags.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/tests/functional/v2/test_schemas.py` & `glance-27.0.0.0b2/glance/tests/functional/v2/test_schemas.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/tests/functional/v2/test_tasks.py` & `glance-27.0.0.0b2/glance/tests/functional/v2/test_tasks.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/tests/functional/v2/test_tasks_api_policy.py` & `glance-27.0.0.0b2/glance/tests/functional/v2/test_tasks_api_policy.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/tests/integration/v2/base.py` & `glance-27.0.0.0b2/glance/tests/integration/v2/base.py`

 * *Files 9% similar despite different names*

```diff
@@ -27,33 +27,53 @@
 from glance.common import config
 import glance.db.sqlalchemy.api
 from glance import tests as glance_tests
 from glance.tests import utils as test_utils
 
 
 TESTING_API_PASTE_CONF = """
-[pipeline:glance-api]
+[composite:glance-api]
+paste.composite_factory = glance.api:root_app_factory
+/: api
+
+[pipeline: api]
 pipeline = versionnegotiation gzip unauthenticated-context rootapp
 
-[pipeline:glance-api-caching]
+[composite:glance-api-caching]
+paste.composite_factory = glance.api:root_app_factory
+/: api-caching
+
+[pipeline: api-caching]
 pipeline = versionnegotiation gzip unauthenticated-context cache rootapp
 
-[pipeline:glance-api-cachemanagement]
+[composite:glance-api-cachemanagement]
+paste.composite_factory = glance.api:root_app_factory
+/: api-cachemanagement
+
+[pipeline: api-cachemanagement]
 pipeline =
     versionnegotiation
     gzip
     unauthenticated-context
     cache
     cache_manage
     rootapp
 
-[pipeline:glance-api-fakeauth]
+[composite:glance-api-fakeauth]
+paste.composite_factory = glance.api:root_app_factory
+/: api-fakeauth
+
+[pipeline: api-fakeauth]
 pipeline = versionnegotiation gzip fakeauth context rootapp
 
-[pipeline:glance-api-noauth]
+[composite:glance-api-noauth]
+paste.composite_factory = glance.api:root_app_factory
+/: api-noauth
+
+[pipeline: api-noauth]
 pipeline = versionnegotiation gzip context rootapp
 
 [composite:rootapp]
 paste.composite_factory = glance.api:root_app_factory
 /: apiversions
 /v2: apiv2app
```

### Comparing `glance-27.0.0.0b1/glance/tests/integration/v2/test_property_quota_violations.py` & `glance-27.0.0.0b2/glance/tests/integration/v2/test_property_quota_violations.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/tests/integration/v2/test_tasks_api.py` & `glance-27.0.0.0b2/glance/tests/integration/v2/test_tasks_api.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/tests/stubs.py` & `glance-27.0.0.0b2/glance/tests/stubs.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/tests/test_hacking.py` & `glance-27.0.0.0b2/glance/tests/test_hacking.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/tests/unit/api/middleware/test_cache_manage.py` & `glance-27.0.0.0b2/glance/tests/unit/api/middleware/test_cache_manage.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/tests/unit/api/test_cmd.py` & `glance-27.0.0.0b2/glance/tests/unit/api/test_cmd.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/tests/unit/api/test_common.py` & `glance-27.0.0.0b2/glance/tests/unit/api/test_common.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/tests/unit/api/test_property_protections.py` & `glance-27.0.0.0b2/glance/tests/unit/api/test_property_protections.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/tests/unit/async_/flows/plugins/test_image_conversion.py` & `glance-27.0.0.0b2/glance/tests/unit/async_/flows/plugins/test_image_conversion.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/tests/unit/async_/flows/plugins/test_inject_image_metadata.py` & `glance-27.0.0.0b2/glance/tests/unit/async_/flows/plugins/test_inject_image_metadata.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/tests/unit/async_/flows/test_api_image_import.py` & `glance-27.0.0.0b2/glance/tests/unit/async_/flows/test_api_image_import.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/tests/unit/async_/flows/test_base_download.py` & `glance-27.0.0.0b2/glance/tests/unit/async_/flows/test_base_download.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/tests/unit/async_/flows/test_convert.py` & `glance-27.0.0.0b2/glance/tests/unit/async_/flows/test_convert.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/tests/unit/async_/flows/test_copy_image.py` & `glance-27.0.0.0b2/glance/tests/unit/async_/flows/test_copy_image.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/tests/unit/async_/flows/test_glance_download.py` & `glance-27.0.0.0b2/glance/tests/unit/async_/flows/test_glance_download.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/tests/unit/async_/flows/test_import.py` & `glance-27.0.0.0b2/glance/tests/unit/async_/flows/test_import.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/tests/unit/async_/flows/test_introspect.py` & `glance-27.0.0.0b2/glance/tests/unit/async_/flows/test_introspect.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/tests/unit/async_/flows/test_ovf_process.py` & `glance-27.0.0.0b2/glance/tests/unit/async_/flows/test_ovf_process.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/tests/unit/async_/flows/test_web_download.py` & `glance-27.0.0.0b2/glance/tests/unit/async_/flows/test_web_download.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/tests/unit/async_/test_async.py` & `glance-27.0.0.0b2/glance/tests/unit/async_/test_async.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/tests/unit/async_/test_taskflow_executor.py` & `glance-27.0.0.0b2/glance/tests/unit/async_/test_taskflow_executor.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/tests/unit/async_/test_utils.py` & `glance-27.0.0.0b2/glance/tests/unit/async_/test_utils.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/tests/unit/base.py` & `glance-27.0.0.0b2/glance/tests/unit/base.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/tests/unit/cmd/test_status.py` & `glance-27.0.0.0b2/glance/tests/unit/cmd/test_status.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/tests/unit/common/scripts/image_import/test_main.py` & `glance-27.0.0.0b2/glance/tests/unit/common/scripts/image_import/test_main.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/tests/unit/common/scripts/test_scripts_utils.py` & `glance-27.0.0.0b2/glance/tests/unit/common/scripts/test_scripts_utils.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/tests/unit/common/test_client.py` & `glance-27.0.0.0b2/glance/tests/unit/common/test_client.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/tests/unit/common/test_config.py` & `glance-27.0.0.0b2/glance/tests/unit/common/test_config.py`

 * *Files 6% similar despite different names*

```diff
@@ -62,27 +62,31 @@
         if not paste_config_file and make_paste_file:
             paste_from = os.path.join(os.getcwd(),
                                       'etc/glance-api-paste.ini')
             _appendto(paste_from, paste_to, paste_append)
 
         app = config.load_paste_app('glance-api')
 
-        self.assertIsInstance(app, expected_app_type)
+        self.assertIsInstance(app['/'], expected_app_type)
 
     def test_load_paste_app(self):
         expected_middleware = oslo_middleware.CORS
         self._do_test_load_paste_app(expected_middleware)
 
     def test_load_paste_app_paste_config_not_found(self):
         expected_middleware = context.UnauthenticatedContextMiddleware
         self.assertRaises(RuntimeError, self._do_test_load_paste_app,
                           expected_middleware, make_paste_file=False)
 
     def test_load_paste_app_with_paste_flavor(self):
-        pipeline = ('[pipeline:glance-api-incomplete]\n'
+        pipeline = ('[composite:glance-api-incomplete]\n'
+                    'paste.composite_factory = glance.api:root_app_factory\n'
+                    '/: api-incomplete\n'
+                    '/healthcheck: healthcheck\n'
+                    '[pipeline:api-incomplete]\n'
                     'pipeline = context rootapp')
         expected_middleware = context.ContextMiddleware
         self._do_test_load_paste_app(expected_middleware,
                                      paste_flavor='incomplete',
                                      paste_append=pipeline)
 
     def test_load_paste_app_with_paste_config_file(self):
```

### Comparing `glance-27.0.0.0b1/glance/tests/unit/common/test_exception.py` & `glance-27.0.0.0b2/glance/tests/unit/common/test_exception.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/tests/unit/common/test_format_inspector.py` & `glance-27.0.0.0b2/glance/tests/unit/common/test_format_inspector.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/tests/unit/common/test_location_strategy.py` & `glance-27.0.0.0b2/glance/tests/unit/common/test_location_strategy.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/tests/unit/common/test_property_utils.py` & `glance-27.0.0.0b2/glance/tests/unit/common/test_property_utils.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/tests/unit/common/test_scripts.py` & `glance-27.0.0.0b2/glance/tests/unit/common/test_scripts.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/tests/unit/common/test_swift_store_utils.py` & `glance-27.0.0.0b2/glance/tests/unit/common/test_swift_store_utils.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/tests/unit/common/test_timeutils.py` & `glance-27.0.0.0b2/glance/tests/unit/common/test_timeutils.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/tests/unit/common/test_utils.py` & `glance-27.0.0.0b2/glance/tests/unit/common/test_utils.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/tests/unit/common/test_wsgi.py` & `glance-27.0.0.0b2/glance/tests/unit/common/test_wsgi.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/tests/unit/common/test_wsgi_app.py` & `glance-27.0.0.0b2/glance/tests/unit/common/test_wsgi_app.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/tests/unit/fake_rados.py` & `glance-27.0.0.0b2/glance/tests/unit/fake_rados.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/tests/unit/fixtures.py` & `glance-27.0.0.0b2/glance/tests/unit/fixtures.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/tests/unit/image_cache/drivers/test_sqlite.py` & `glance-27.0.0.0b2/glance/tests/unit/image_cache/drivers/test_sqlite.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/tests/unit/keymgr/fake.py` & `glance-27.0.0.0b2/glance/tests/unit/keymgr/fake.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/tests/unit/test_auth.py` & `glance-27.0.0.0b2/glance/tests/unit/test_auth.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/tests/unit/test_cache_manage.py` & `glance-27.0.0.0b2/glance/tests/unit/test_cache_manage.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/tests/unit/test_cache_middleware.py` & `glance-27.0.0.0b2/glance/tests/unit/test_cache_middleware.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/tests/unit/test_cached_images.py` & `glance-27.0.0.0b2/glance/tests/unit/test_cached_images.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/tests/unit/test_context.py` & `glance-27.0.0.0b2/glance/tests/unit/test_context.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/tests/unit/test_context_middleware.py` & `glance-27.0.0.0b2/glance/tests/unit/test_context_middleware.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/tests/unit/test_data_migration_framework.py` & `glance-27.0.0.0b2/glance/tests/unit/test_data_migration_framework.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/tests/unit/test_db.py` & `glance-27.0.0.0b2/glance/tests/unit/test_db.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/tests/unit/test_db_metadef.py` & `glance-27.0.0.0b2/glance/tests/unit/test_db_metadef.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/tests/unit/test_domain.py` & `glance-27.0.0.0b2/glance/tests/unit/test_domain.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/tests/unit/test_domain_proxy.py` & `glance-27.0.0.0b2/glance/tests/unit/test_domain_proxy.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/tests/unit/test_gateway.py` & `glance-27.0.0.0b2/glance/tests/unit/test_gateway.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/tests/unit/test_glance_manage.py` & `glance-27.0.0.0b2/glance/tests/unit/test_glance_manage.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/tests/unit/test_glance_replicator.py` & `glance-27.0.0.0b2/glance/tests/unit/test_glance_replicator.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/tests/unit/test_housekeeping.py` & `glance-27.0.0.0b2/glance/tests/unit/test_housekeeping.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/tests/unit/test_image_cache.py` & `glance-27.0.0.0b2/glance/tests/unit/test_image_cache.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/tests/unit/test_manage.py` & `glance-27.0.0.0b2/glance/tests/unit/test_manage.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/tests/unit/test_misc.py` & `glance-27.0.0.0b2/glance/tests/unit/test_misc.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/tests/unit/test_notifier.py` & `glance-27.0.0.0b2/glance/tests/unit/test_notifier.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/tests/unit/test_policy.py` & `glance-27.0.0.0b2/glance/tests/unit/test_policy.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/tests/unit/test_quota.py` & `glance-27.0.0.0b2/glance/tests/unit/test_quota.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/tests/unit/test_schema.py` & `glance-27.0.0.0b2/glance/tests/unit/test_schema.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/tests/unit/test_scrubber.py` & `glance-27.0.0.0b2/glance/tests/unit/test_scrubber.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/tests/unit/test_store_image.py` & `glance-27.0.0.0b2/glance/tests/unit/test_store_image.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/tests/unit/test_store_location.py` & `glance-27.0.0.0b2/glance/tests/unit/test_store_location.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/tests/unit/test_test_utils.py` & `glance-27.0.0.0b2/glance/tests/unit/test_test_utils.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/tests/unit/test_versions.py` & `glance-27.0.0.0b2/glance/tests/unit/test_versions.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/tests/unit/utils.py` & `glance-27.0.0.0b2/glance/tests/unit/utils.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/tests/unit/v2/test_cache_management_api.py` & `glance-27.0.0.0b2/glance/tests/unit/v2/test_cache_management_api.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/tests/unit/v2/test_discovery_image_import.py` & `glance-27.0.0.0b2/glance/tests/unit/v2/test_discovery_image_import.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/tests/unit/v2/test_discovery_stores.py` & `glance-27.0.0.0b2/glance/tests/unit/v2/test_discovery_stores.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/tests/unit/v2/test_image_actions_resource.py` & `glance-27.0.0.0b2/glance/tests/unit/v2/test_image_actions_resource.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/tests/unit/v2/test_image_data_resource.py` & `glance-27.0.0.0b2/glance/tests/unit/v2/test_image_data_resource.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/tests/unit/v2/test_image_members_resource.py` & `glance-27.0.0.0b2/glance/tests/unit/v2/test_image_members_resource.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/tests/unit/v2/test_image_tags_resource.py` & `glance-27.0.0.0b2/glance/tests/unit/v2/test_image_tags_resource.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/tests/unit/v2/test_images_resource.py` & `glance-27.0.0.0b2/glance/tests/unit/v2/test_images_resource.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/tests/unit/v2/test_metadef_resources.py` & `glance-27.0.0.0b2/glance/tests/unit/v2/test_metadef_resources.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/tests/unit/v2/test_schemas_resource.py` & `glance-27.0.0.0b2/glance/tests/unit/v2/test_schemas_resource.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/tests/unit/v2/test_tasks_resource.py` & `glance-27.0.0.0b2/glance/tests/unit/v2/test_tasks_resource.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/tests/unit/v2/test_v2_policy.py` & `glance-27.0.0.0b2/glance/tests/unit/v2/test_v2_policy.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/tests/utils.py` & `glance-27.0.0.0b2/glance/tests/utils.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/tests/var/ca.crt` & `glance-27.0.0.0b2/glance/tests/var/ca.crt`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/tests/var/ca.key` & `glance-27.0.0.0b2/glance/tests/var/ca.key`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/tests/var/certificate.crt` & `glance-27.0.0.0b2/glance/tests/var/certificate.crt`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/tests/var/privatekey.key` & `glance-27.0.0.0b2/glance/tests/var/privatekey.key`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/tests/var/testserver-bad-ovf.ova` & `glance-27.0.0.0b2/glance/tests/var/testserver-bad-ovf.ova`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/tests/var/testserver-no-disk.ova` & `glance-27.0.0.0b2/glance/tests/var/testserver-no-disk.ova`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/tests/var/testserver-no-ovf.ova` & `glance-27.0.0.0b2/glance/tests/var/testserver-no-ovf.ova`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/tests/var/testserver-not-tar.ova` & `glance-27.0.0.0b2/glance/tests/var/testserver-not-tar.ova`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance/tests/var/testserver.ova` & `glance-27.0.0.0b2/glance/tests/var/testserver.ova`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance.egg-info/PKG-INFO` & `glance-27.0.0.0b2/glance.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: glance
-Version: 27.0.0.0b1
+Version: 27.0.0.0b2
 Summary: OpenStack Image Service
 Home-page: https://docs.openstack.org/glance/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ================
         OpenStack Glance
```

### Comparing `glance-27.0.0.0b1/glance.egg-info/SOURCES.txt` & `glance-27.0.0.0b2/glance.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -699,14 +699,15 @@
 releasenotes/notes/antelope-milestone-2-d89e39412f9c0334.yaml
 releasenotes/notes/antelope-milestone-3-b9a4f7fdba31f628.yaml
 releasenotes/notes/api-2-6-current-9eeb83b7ecc0a562.yaml
 releasenotes/notes/api-2.16-8417b1e23322fedb.yaml
 releasenotes/notes/api-minor-ver-bump-2-6-aa3591fc58f08055.yaml
 releasenotes/notes/api-minor-version-bump-bbd69dc457fc731c.yaml
 releasenotes/notes/bobcat-milestone-1-releasenotes-2d109105530877d6.yaml
+releasenotes/notes/bobcat-milestone-2-releasenotes-085084b03f66d671.yaml
 releasenotes/notes/bp-barbican-secret-deletion-support-40cffa5ffa33447e.yaml
 releasenotes/notes/bp-inject-image-metadata-0a08af539bcce7f2.yaml
 releasenotes/notes/bp-mitigate-ossn-0075-c0e74e60d86d8ea2.yaml
 releasenotes/notes/bp-upgrade-checks-b3272c3ddb4e8cf7.yaml
 releasenotes/notes/bug-1537903-54b2822eac6cfc09.yaml
 releasenotes/notes/bug-1593177-8ef35458d29ec93c.yaml
 releasenotes/notes/bug-1719252-name-validation-443a2e2a36be2cec.yaml
```

### Comparing `glance-27.0.0.0b1/glance.egg-info/entry_points.txt` & `glance-27.0.0.0b2/glance.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/glance.egg-info/requires.txt` & `glance-27.0.0.0b2/glance.egg-info/requires.txt`

 * *Files 12% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 WebOb>=1.8.1
 alembic>=0.9.6
 castellan>=0.17.0
 cryptography>=2.6.1
 cursive>=0.2.1
 debtcollector>=1.19.0
 defusedxml>=0.6.0
-eventlet>=0.25.1
+eventlet>=0.33.3
 futurist>=1.2.0
 glance-store>=2.3.0
 httplib2>=0.9.1
 iso8601>=0.1.11
 jsonschema>=3.2.0
 keystoneauth1>=3.4.0
 keystonemiddleware>=5.1.0
```

### Comparing `glance-27.0.0.0b1/playbooks/post-check-metadata-injection.yaml` & `glance-27.0.0.0b2/playbooks/post-check-metadata-injection.yaml`

 * *Files 20% similar despite different names*

```diff
@@ -5,16 +5,20 @@
       shell:
         executable: /bin/bash
         cmd: |
           source /opt/stack/devstack/openrc
           set -xe
           cirrosimg=$(glance image-list | grep cirros | cut -d" " -f 2)
 
-          echo "Dumping the cirros image for debugging..."
-          glance image-show $cirrosimg
+          # There could be more than one cirros image so traverse through the list
+          for image in $cirrosimg
+          do
+              echo "Dumping the cirros image for debugging..."
+              glance image-show $image
 
-          echo "Checking that the cirros image was decorated with metdata on import..."
-          glance image-list --property-filter 'glance_devstack_test=doyouseeme?' | grep cirros
+              echo "Checking that the cirros image was decorated with metdata on import..."
+              glance image-list --property-filter 'glance_devstack_test=doyouseeme?' | grep $image
 
-          echo "Checking that the cirros image was converted to raw on import..."
-          glance image-show $cirrosimg | egrep -e 'disk_format.*raw'
+              echo "Checking that the cirros image was converted to raw on import..."
+              glance image-show $image | egrep -e 'disk_format.*raw'
+          done
       environment: '{{ zuul | zuul_legacy_vars }}'
```

### Comparing `glance-27.0.0.0b1/rally-jobs/README.rst` & `glance-27.0.0.0b2/rally-jobs/README.rst`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/rally-jobs/glance.yaml` & `glance-27.0.0.0b2/rally-jobs/glance.yaml`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/releasenotes/notes/Stein-reno-rc1-0a03f8394934a2e7.yaml` & `glance-27.0.0.0b2/releasenotes/notes/Stein-reno-rc1-0a03f8394934a2e7.yaml`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/releasenotes/notes/Train-milestone3-be5520106a182fa0.yaml` & `glance-27.0.0.0b2/releasenotes/notes/Train-milestone3-be5520106a182fa0.yaml`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/releasenotes/notes/add-compressed-format-185e537187a202bd.yaml` & `glance-27.0.0.0b2/releasenotes/notes/add-compressed-format-185e537187a202bd.yaml`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/releasenotes/notes/add_policy_enforcement_for_metadef_delete_apis-95d2b16cc444840a.yaml` & `glance-27.0.0.0b2/releasenotes/notes/add_policy_enforcement_for_metadef_delete_apis-95d2b16cc444840a.yaml`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/releasenotes/notes/alembic-migrations-902b31edae7a5d7d.yaml` & `glance-27.0.0.0b2/releasenotes/notes/alembic-migrations-902b31edae7a5d7d.yaml`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/releasenotes/notes/antelope-milestone-2-d89e39412f9c0334.yaml` & `glance-27.0.0.0b2/releasenotes/notes/antelope-milestone-2-d89e39412f9c0334.yaml`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/releasenotes/notes/antelope-milestone-3-b9a4f7fdba31f628.yaml` & `glance-27.0.0.0b2/releasenotes/notes/antelope-milestone-3-b9a4f7fdba31f628.yaml`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/releasenotes/notes/api-2-6-current-9eeb83b7ecc0a562.yaml` & `glance-27.0.0.0b2/releasenotes/notes/api-2-6-current-9eeb83b7ecc0a562.yaml`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/releasenotes/notes/api-2.16-8417b1e23322fedb.yaml` & `glance-27.0.0.0b2/releasenotes/notes/api-2.16-8417b1e23322fedb.yaml`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/releasenotes/notes/api-minor-ver-bump-2-6-aa3591fc58f08055.yaml` & `glance-27.0.0.0b2/releasenotes/notes/api-minor-ver-bump-2-6-aa3591fc58f08055.yaml`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/releasenotes/notes/api-minor-version-bump-bbd69dc457fc731c.yaml` & `glance-27.0.0.0b2/releasenotes/notes/api-minor-version-bump-bbd69dc457fc731c.yaml`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/releasenotes/notes/bp-barbican-secret-deletion-support-40cffa5ffa33447e.yaml` & `glance-27.0.0.0b2/releasenotes/notes/bp-barbican-secret-deletion-support-40cffa5ffa33447e.yaml`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/releasenotes/notes/bp-inject-image-metadata-0a08af539bcce7f2.yaml` & `glance-27.0.0.0b2/releasenotes/notes/bp-inject-image-metadata-0a08af539bcce7f2.yaml`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/releasenotes/notes/bug-1537903-54b2822eac6cfc09.yaml` & `glance-27.0.0.0b2/releasenotes/notes/bug-1537903-54b2822eac6cfc09.yaml`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/releasenotes/notes/bug-1980049-623d2eb0fa074136.yaml` & `glance-27.0.0.0b2/releasenotes/notes/bug-1980049-623d2eb0fa074136.yaml`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/releasenotes/notes/cinder-store-migration-non-owner-80a2a8114d8602aa.yaml` & `glance-27.0.0.0b2/releasenotes/notes/cinder-store-migration-non-owner-80a2a8114d8602aa.yaml`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/releasenotes/notes/consistent-store-names-57374b9505d530d0.yaml` & `glance-27.0.0.0b2/releasenotes/notes/consistent-store-names-57374b9505d530d0.yaml`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/releasenotes/notes/copy-existing-image-94fd0b8d24bc16a0.yaml` & `glance-27.0.0.0b2/releasenotes/notes/copy-existing-image-94fd0b8d24bc16a0.yaml`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/releasenotes/notes/deprecate-admin_role-2f9d33ed0785d082.yaml` & `glance-27.0.0.0b2/releasenotes/notes/deprecate-admin_role-2f9d33ed0785d082.yaml`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/releasenotes/notes/deprecate-allow_additional_image_props-0e3b2f1ffa4e55e1.yaml` & `glance-27.0.0.0b2/releasenotes/notes/deprecate-allow_additional_image_props-0e3b2f1ffa4e55e1.yaml`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/releasenotes/notes/deprecate-checksum-a602853403e1c4a8.yaml` & `glance-27.0.0.0b2/releasenotes/notes/deprecate-checksum-a602853403e1c4a8.yaml`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/releasenotes/notes/deprecate-json-formatted-policy-file-5cb692fe889eb52b.yaml` & `glance-27.0.0.0b2/releasenotes/notes/deprecate-json-formatted-policy-file-5cb692fe889eb52b.yaml`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/releasenotes/notes/deprecate-registry-ff286df90df793f0.yaml` & `glance-27.0.0.0b2/releasenotes/notes/deprecate-registry-ff286df90df793f0.yaml`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/releasenotes/notes/deprecate-show-multiple-location-9890a1e961def2f6.yaml` & `glance-27.0.0.0b2/releasenotes/notes/deprecate-show-multiple-location-9890a1e961def2f6.yaml`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/releasenotes/notes/deprecate-show-multiple-location-continued-646f91b21cd771f7.yaml` & `glance-27.0.0.0b2/releasenotes/notes/deprecate-show-multiple-location-continued-646f91b21cd771f7.yaml`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/releasenotes/notes/deprecate-show-multiple-location-continued-ussuri-16e8d9d8a59da1bc.yaml` & `glance-27.0.0.0b2/releasenotes/notes/deprecate-show-multiple-location-continued-ussuri-16e8d9d8a59da1bc.yaml`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/releasenotes/notes/deprecate-v1-api-6c7dbefb90fd8772.yaml` & `glance-27.0.0.0b2/releasenotes/notes/deprecate-v1-api-6c7dbefb90fd8772.yaml`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/releasenotes/notes/distributed-image-import-82cff4426731beac.yaml` & `glance-27.0.0.0b2/releasenotes/notes/distributed-image-import-82cff4426731beac.yaml`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/releasenotes/notes/experimental-multi-store-d2c26f9dbb9c835b.yaml` & `glance-27.0.0.0b2/releasenotes/notes/experimental-multi-store-d2c26f9dbb9c835b.yaml`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/releasenotes/notes/glare-ectomy-72a1f80f306f2e3b.yaml` & `glance-27.0.0.0b2/releasenotes/notes/glare-ectomy-72a1f80f306f2e3b.yaml`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/releasenotes/notes/image-tasks-api-f21b42eab91c2079.yaml` & `glance-27.0.0.0b2/releasenotes/notes/image-tasks-api-f21b42eab91c2079.yaml`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/releasenotes/notes/image-visibility-changes-fa5aa18dc67244c4.yaml` & `glance-27.0.0.0b2/releasenotes/notes/image-visibility-changes-fa5aa18dc67244c4.yaml`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/releasenotes/notes/implement-lite-spec-db-sync-check-3e2e147aec0ae82b.yaml` & `glance-27.0.0.0b2/releasenotes/notes/implement-lite-spec-db-sync-check-3e2e147aec0ae82b.yaml`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/releasenotes/notes/import-locking-behavior-901c691f3839fe0a.yaml` & `glance-27.0.0.0b2/releasenotes/notes/import-locking-behavior-901c691f3839fe0a.yaml`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/releasenotes/notes/import-multi-stores-3e781f2878b3134d.yaml` & `glance-27.0.0.0b2/releasenotes/notes/import-multi-stores-3e781f2878b3134d.yaml`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/releasenotes/notes/improved-config-options-221c58a8c37602ba.yaml` & `glance-27.0.0.0b2/releasenotes/notes/improved-config-options-221c58a8c37602ba.yaml`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/releasenotes/notes/location-add-status-checks-b70db66100bc96b7.yaml` & `glance-27.0.0.0b2/releasenotes/notes/location-add-status-checks-b70db66100bc96b7.yaml`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/releasenotes/notes/make-task-api-admin-only-by-default-7def996262e18f7a.yaml` & `glance-27.0.0.0b2/releasenotes/notes/make-task-api-admin-only-by-default-7def996262e18f7a.yaml`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/releasenotes/notes/multihash-081466a98601da20.yaml` & `glance-27.0.0.0b2/releasenotes/notes/multihash-081466a98601da20.yaml`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/releasenotes/notes/mutistore-support-for-scrubber-6b360394ef32774a.yaml` & `glance-27.0.0.0b2/releasenotes/notes/mutistore-support-for-scrubber-6b360394ef32774a.yaml`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/releasenotes/notes/new_image_filters-c888361e6ecf495c.yaml` & `glance-27.0.0.0b2/releasenotes/notes/new_image_filters-c888361e6ecf495c.yaml`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/releasenotes/notes/newton-1-release-065334d464f78fc5.yaml` & `glance-27.0.0.0b2/releasenotes/notes/newton-1-release-065334d464f78fc5.yaml`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/releasenotes/notes/newton-bugs-06ed3727b973c271.yaml` & `glance-27.0.0.0b2/releasenotes/notes/newton-bugs-06ed3727b973c271.yaml`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/releasenotes/notes/oslo-log-use-stderr-changes-07f5daf3e6abdcd6.yaml` & `glance-27.0.0.0b2/releasenotes/notes/oslo-log-use-stderr-changes-07f5daf3e6abdcd6.yaml`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/releasenotes/notes/pike-metadefs-changes-95b54e0bf8bbefd6.yaml` & `glance-27.0.0.0b2/releasenotes/notes/pike-metadefs-changes-95b54e0bf8bbefd6.yaml`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/releasenotes/notes/pike-rc-1-a5d3f6e8877b52c6.yaml` & `glance-27.0.0.0b2/releasenotes/notes/pike-rc-1-a5d3f6e8877b52c6.yaml`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/releasenotes/notes/pike-rc-2-acc173005045e16a.yaml` & `glance-27.0.0.0b2/releasenotes/notes/pike-rc-2-acc173005045e16a.yaml`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/releasenotes/notes/policy-in-code-7e0c6c070d32d136.yaml` & `glance-27.0.0.0b2/releasenotes/notes/policy-in-code-7e0c6c070d32d136.yaml`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/releasenotes/notes/policy-in-code-implications-438449a73af2893c.yaml` & `glance-27.0.0.0b2/releasenotes/notes/policy-in-code-implications-438449a73af2893c.yaml`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/releasenotes/notes/policy-refactor-xena-0cddb7f2d492cb3a.yaml` & `glance-27.0.0.0b2/releasenotes/notes/policy-refactor-xena-0cddb7f2d492cb3a.yaml`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/releasenotes/notes/queens-metadefs-changes-daf02bef18d049f4.yaml` & `glance-27.0.0.0b2/releasenotes/notes/queens-metadefs-changes-daf02bef18d049f4.yaml`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/releasenotes/notes/queens-uwsgi-issues-4cee9e4fdf62c646.yaml` & `glance-27.0.0.0b2/releasenotes/notes/queens-uwsgi-issues-4cee9e4fdf62c646.yaml`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/releasenotes/notes/range-header-request-83cf11eebf865fb1.yaml` & `glance-27.0.0.0b2/releasenotes/notes/range-header-request-83cf11eebf865fb1.yaml`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/releasenotes/notes/rbac-updates-ba0fcb886fe4085c.yaml` & `glance-27.0.0.0b2/releasenotes/notes/rbac-updates-ba0fcb886fe4085c.yaml`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/releasenotes/notes/remove-enforce-secure-rbac-ec9a0249870460c2.yaml` & `glance-27.0.0.0b2/releasenotes/notes/remove-enforce-secure-rbac-ec9a0249870460c2.yaml`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/releasenotes/notes/remove-osprofiler-paste-ini-options-c620dedc8f9728ff.yaml` & `glance-27.0.0.0b2/releasenotes/notes/remove-osprofiler-paste-ini-options-c620dedc8f9728ff.yaml`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/releasenotes/notes/remove_native_ssl-c16d5a127b57583d.yaml` & `glance-27.0.0.0b2/releasenotes/notes/remove_native_ssl-c16d5a127b57583d.yaml`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/releasenotes/notes/reordered-store-config-opts-newton-3a6575b5908c0e0f.yaml` & `glance-27.0.0.0b2/releasenotes/notes/reordered-store-config-opts-newton-3a6575b5908c0e0f.yaml`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/releasenotes/notes/restrict_location_updates-05454bb765a8c92c.yaml` & `glance-27.0.0.0b2/releasenotes/notes/restrict_location_updates-05454bb765a8c92c.yaml`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/releasenotes/notes/rethinking-filesystem-access-120bc46064b3d40a.yaml` & `glance-27.0.0.0b2/releasenotes/notes/rethinking-filesystem-access-120bc46064b3d40a.yaml`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/releasenotes/notes/rocky-rc-b0ea7628b7a74c96.yaml` & `glance-27.0.0.0b2/releasenotes/notes/rocky-rc-b0ea7628b7a74c96.yaml`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/releasenotes/notes/secure-rbac-project-personas-fb0d9792b9dc3783.yaml` & `glance-27.0.0.0b2/releasenotes/notes/secure-rbac-project-personas-fb0d9792b9dc3783.yaml`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/releasenotes/notes/train-metadefs-changes-c4380754cdd13a19.yaml` & `glance-27.0.0.0b2/releasenotes/notes/train-metadefs-changes-c4380754cdd13a19.yaml`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/releasenotes/notes/use-cursive-c6b15d94845232da.yaml` & `glance-27.0.0.0b2/releasenotes/notes/use-cursive-c6b15d94845232da.yaml`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/releasenotes/notes/use-webob-1.8.1-5c3cd1b1382f063e.yaml` & `glance-27.0.0.0b2/releasenotes/notes/use-webob-1.8.1-5c3cd1b1382f063e.yaml`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/releasenotes/notes/ussuri-final-b377a21508ada060.yaml` & `glance-27.0.0.0b2/releasenotes/notes/ussuri-final-b377a21508ada060.yaml`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/releasenotes/notes/victoria-m2-release-notes-8a6ae2fdb3d29dae.yaml` & `glance-27.0.0.0b2/releasenotes/notes/victoria-m2-release-notes-8a6ae2fdb3d29dae.yaml`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/releasenotes/notes/victoria-m3-releasenotes-9209cea98a29abc4.yaml` & `glance-27.0.0.0b2/releasenotes/notes/victoria-m3-releasenotes-9209cea98a29abc4.yaml`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/releasenotes/notes/victoria-rc1-release-notes-d928355cf90d608d.yaml` & `glance-27.0.0.0b2/releasenotes/notes/victoria-rc1-release-notes-d928355cf90d608d.yaml`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/releasenotes/notes/wsgi-containerization-369880238a5e793d.yaml` & `glance-27.0.0.0b2/releasenotes/notes/wsgi-containerization-369880238a5e793d.yaml`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/releasenotes/notes/xena-m3-releasenotes-a92d55d29eecc8f6.yaml` & `glance-27.0.0.0b2/releasenotes/notes/xena-m3-releasenotes-a92d55d29eecc8f6.yaml`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/releasenotes/notes/xena-rc1-release-notes-12dbe0ac528ce483.yaml` & `glance-27.0.0.0b2/releasenotes/notes/xena-rc1-release-notes-12dbe0ac528ce483.yaml`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/releasenotes/notes/yoga-rc1-release-notes-153932161f52a038.yaml` & `glance-27.0.0.0b2/releasenotes/notes/yoga-rc1-release-notes-153932161f52a038.yaml`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/releasenotes/notes/zed-milestone-1-592415040e67924e.yaml` & `glance-27.0.0.0b2/releasenotes/notes/zed-milestone-1-592415040e67924e.yaml`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/releasenotes/notes/zed-milestone-2-a782e75cdbd8fe13.yaml` & `glance-27.0.0.0b2/releasenotes/notes/zed-milestone-2-a782e75cdbd8fe13.yaml`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/releasenotes/notes/zed-milestone-3-3e38697ae4677a81.yaml` & `glance-27.0.0.0b2/releasenotes/notes/zed-milestone-3-3e38697ae4677a81.yaml`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/releasenotes/source/conf.py` & `glance-27.0.0.0b2/releasenotes/source/conf.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/releasenotes/source/locale/en_GB/LC_MESSAGES/releasenotes.po` & `glance-27.0.0.0b2/releasenotes/source/locale/en_GB/LC_MESSAGES/releasenotes.po`

 * *Files 1% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 # Andi Chandler <andi@gowling.com>, 2020. #zanata
 # Andi Chandler <andi@gowling.com>, 2022. #zanata
 # Andi Chandler <andi@gowling.com>, 2023. #zanata
 msgid ""
 msgstr ""
 "Project-Id-Version: Glance Release Notes\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-03-04 12:01+0000\n"
+"POT-Creation-Date: 2023-06-16 12:05+0000\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"PO-Revision-Date: 2023-02-03 04:34+0000\n"
+"PO-Revision-Date: 2023-06-17 02:38+0000\n"
 "Last-Translator: Andi Chandler <andi@gowling.com>\n"
 "Language-Team: English (United Kingdom)\n"
 "Language: en_GB\n"
 "X-Generator: Zanata 4.3.3\n"
 "Plural-Forms: nplurals=2; plural=(n != 1)\n"
 
 msgid "\"glance-manage\" purges all deleted rows if \"--max_rows\" equals -1"
@@ -147,14 +147,17 @@
 
 msgid "20.1.0"
 msgstr "20.1.0"
 
 msgid "20.2.0"
 msgstr "20.2.0"
 
+msgid "2023.1 Series Release Notes"
+msgstr "2023.1 Series Release Notes"
+
 msgid "21.0.0"
 msgstr "21.0.0"
 
 msgid "21.1.0"
 msgstr "21.1.0"
 
 msgid "22.0.0"
@@ -177,16 +180,19 @@
 
 msgid "24.2.0"
 msgstr "24.2.0"
 
 msgid "25.0.0"
 msgstr "25.0.0"
 
-msgid "26.0.0.0b2"
-msgstr "26.0.0.0b2"
+msgid "26.0.0"
+msgstr "26.0.0"
+
+msgid "27.0.0.0b1"
+msgstr "27.0.0.0b1"
 
 msgid ""
 "A change was added to the import API which provides time-based locking of an "
 "image to exclude other import operations from starting until the lock-"
 "holding task completes (see Bug 1884596_). The lock is based on the task "
 "that we start to do the work, and the UUID of that task is stored in the "
 "``os_glance_import_task`` image property, which indicates who owns the lock. "
@@ -797,14 +803,29 @@
 "single store. Through new '/v2/stores' endpoint the API user can request "
 "image to be deleted from single store instead of deleting the whole image. "
 "This feature can be used to clean up store metadata in cases where the image "
 "data has for some reason disappeared from the store already, except 410 Gone "
 "HTTP response."
 
 msgid ""
+"As per the revised SRBAC community goals, glance service is switching to new "
+"defaults by default in Antelope cycle, hence removing the deprecated "
+"``enforce_secure_rbac`` option which is no longer needed. The "
+"``enforce_secure_rbac`` option was introduced EXPERIMENTAL in Wallaby "
+"release for operators to opt into enforcing authorization based on common "
+"RBAC personas."
+msgstr ""
+"As per the revised SRBAC community goals, the Glance service is switching to "
+"new defaults by default in the Antelope cycle, hence removing the deprecated "
+"``enforce_secure_rbac`` option which is no longer needed. The "
+"``enforce_secure_rbac`` option was introduced EXPERIMENTAL in the Wallaby "
+"release for operators to opt into enforcing authorisation based on common "
+"RBAC personas."
+
+msgid ""
 "As with all container formats, Glance does not verify that the data payload "
 "of an image is actually in that format.  Further, you should not expect "
 "other OpenStack services to be able to handle arbitrary compressed file "
 "formats.  Consult the documentation of any services that will consume your "
 "image for details."
 msgstr ""
 "As with all container formats, Glance does not verify that the data payload "
@@ -1261,14 +1282,21 @@
 msgstr "Bug 1939169_: glance md-tag-create-multiple overwrites existing tags"
 
 msgid "Bug 1939307_: glance-uwsgi - Add missing cache prefetching periodic job"
 msgstr ""
 "Bug 1939307_: glance-uwsgi - Add missing cache prefetching periodic job"
 
 msgid ""
+"Bug 1939690_: The api-ref response and the actual response returned from the "
+"Create Tags API does not match"
+msgstr ""
+"Bug 1939690_: The api-ref response and the actual response returned from the "
+"Create Tags API does not match"
+
+msgid ""
 "Bug 1939922_: Internal server error if shared member tries to stage data to "
 "image"
 msgstr ""
 "Bug 1939922_: Internal server error if shared member tries to stage data to "
 "image"
 
 msgid ""
@@ -1335,14 +1363,24 @@
 
 msgid "Bug 1989268_: Wrong assertion method"
 msgstr "Bug 1989268_: Wrong assertion method"
 
 msgid "Bug 1990854_: oslo_limit section not clear"
 msgstr "Bug 1990854_: oslo_limit section not clear"
 
+msgid ""
+"Bug 1996188_: [OSSA-2023-002] Arbitrary file access through custom VMDK flat "
+"descriptor (CVE-2022-47951)"
+msgstr ""
+"Bug 1996188_: [OSSA-2023-002] Arbitrary file access through custom VMDK flat "
+"descriptor (CVE-2022-47951)"
+
+msgid "Bug 2007354_: duplicate values in compute-host-capabilities.json"
+msgstr "Bug 2007354_: duplicate values in compute-host-capabilities.json"
+
 msgid "Bug Fixes"
 msgstr "Bug Fixes"
 
 msgid ""
 "Bug `1971521 <https://bugs.launchpad.net/glance/+bug/1971521>`_: Fixed the "
 "success response code of the REST API call ``PUT /v2/cache/{image_id}`` to "
 "be 202 (Accepted), following the original design of the feature."
@@ -2015,14 +2053,21 @@
 "basis in Rocky and now fully supported in the Train release, then you *must* "
 "use backing stores instead of ``work_dir`` and ``node_staging_uri`` for "
 "Glance's temporary storage **beginning right now with the current "
 "release**.  See the \"Reserved Stores\" section of the \"Multi Store Support"
 "\" chapter of the Glance Administration Guide for more information."
 
 msgid ""
+"If you want to disable them then modify the below config options value in "
+"``glance-api.conf`` file::"
+msgstr ""
+"If you want to disable them then modify the below config options value in "
+"``glance-api.conf`` file::"
+
+msgid ""
 "If you were previously aware of this option and were actually using it, we "
 "apologize for the inconvenience its removal will cause, but overall it will "
 "be better for everyone if policy configuration is confined to the policy "
 "configuration file and this backdoor is eliminated.  The migration path is "
 "to explictly mention the role you configured for this option in appropriate "
 "places in your policy configuration file."
 msgstr ""
@@ -2226,14 +2271,29 @@
 "In the v1 API, images have an ``is_public`` field (but no ``visibility`` "
 "field).  Images for which ``is_public`` is True are the equivalent of images "
 "with 'public' visibility in the v2 API.  Images for which ``is_public`` is "
 "false are the equivalent of v2 'shared' images if they have members, or the "
 "equivalent of v2 'private' images if they have no members."
 
 msgid ""
+"In this cycle Glance enabled the API policies (RBAC) new defaults and scope "
+"by default and removed the deprecated ``enforce_secure_rbac`` option which "
+"is no longer needed after switching to new defaults. The Default value of "
+"config options ``[oslo_policy] enforce_scope`` and ``[oslo_policy] "
+"oslo_policy.enforce_new_defaults`` have been changed to ``True``. Old "
+"policies are still there but they are disabled by default."
+msgstr ""
+"In this cycle Glance enabled the API policies (RBAC) new defaults and scope "
+"by default and removed the deprecated ``enforce_secure_rbac`` option which "
+"is no longer needed after switching to new defaults. The Default value of "
+"config options ``[oslo_policy] enforce_scope`` and ``[oslo_policy] "
+"oslo_policy.enforce_new_defaults`` have been changed to ``True``. Old "
+"policies are still there but they are disabled by default."
+
+msgid ""
 "In this release, the default value of ``admin_role`` has been defined as "
 "``__NOT_A_ROLE_07697c71e6174332989d3d5f2a7d2e7c_NOT_A_ROLE__``. This "
 "effectively makes it inoperable (unless your Keystone administrator has "
 "actually created such a role and assigned it to someone, which is unlikely "
 "but possible, so you should check).  If your local policy tests (you have "
 "some, right?) indicate that your Glance policies no longer function as "
 "expected, then you have been relying on the ``admin_role`` configuration "
@@ -2469,14 +2529,21 @@
 msgid "Note the ordering of the options within a store is not alphabetical."
 msgstr "Note the ordering of the options within a store is not alphabetical."
 
 msgid "Note: This is not a change.  It's simply mentioned for completeness."
 msgstr "Note: This is not a change.  It's simply mentioned for completeness."
 
 msgid ""
+"Now operator can control the scope and new defaults flag with the below "
+"config options in ``glance-api.conf`` file::"
+msgstr ""
+"Now operator can control the scope and new defaults flag with the below "
+"config options in ``glance-api.conf`` file::"
+
+msgid ""
 "OSprofiler support requires passing of trace information between various "
 "OpenStack services. This information is signed by one of HMAC keys, which we "
 "historically defined in glance-api-paste.ini and glance-registry-paste.ini "
 "files (together with enabled option, that in fact was duplicated in the "
 "corresponding configuration files). OSprofiler 0.3.1 and higher supports "
 "passing this information via configuration files, therefore it's recommended "
 "to modify the ``[filter:osprofiler]`` section in  \\*-paste.ini to look like "
@@ -3091,14 +3158,25 @@
 "OpenStack, we are committed to `The Four Opens`_.  If the ability to run "
 "Glance under uWSGI is important to you, feel free to participate in the "
 "Glance community to help coordinate and drive such an effort.  (We gently "
 "remind you that \"participation\" includes providing testing and development "
 "resources.)"
 
 msgid ""
+"The Glance service enables the API policies (RBAC) new defaults and scope by "
+"default. The Default value of config options ``[oslo_policy] enforce_scope`` "
+"and ``[oslo_policy] oslo_policy.enforce_new_defaults`` have been changed to "
+"``True``."
+msgstr ""
+"The Glance service enables the API policies (RBAC) new defaults and scope by "
+"default. The Default value of config options ``[oslo_policy] enforce_scope`` "
+"and ``[oslo_policy] oslo_policy.enforce_new_defaults`` have been changed to "
+"``True``."
+
+msgid ""
 "The Image Service API Reference has been updated with a section on the "
 "`Interoperable image import`_ process (also known as \"image import "
 "refactored\") and the API calls that are exposed to implement it in the "
 "EXPERIMENTAL v2.6 of the API."
 msgstr ""
 "The Image Service API Reference has been updated with a section on the "
 "`Interoperable image import`_ process (also known as \"image import "
```

### Comparing `glance-27.0.0.0b1/releasenotes/source/locale/fr/LC_MESSAGES/releasenotes.po` & `glance-27.0.0.0b2/releasenotes/source/locale/fr/LC_MESSAGES/releasenotes.po`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/releasenotes/source/locale/ja/LC_MESSAGES/releasenotes.po` & `glance-27.0.0.0b2/releasenotes/source/locale/ja/LC_MESSAGES/releasenotes.po`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/releasenotes/source/locale/ko_KR/LC_MESSAGES/releasenotes.po` & `glance-27.0.0.0b2/releasenotes/source/locale/ko_KR/LC_MESSAGES/releasenotes.po`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/requirements.txt` & `glance-27.0.0.0b2/requirements.txt`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # process, which may cause wedges in the gate later.
 
 pbr>=3.1.1 # Apache-2.0
 defusedxml>=0.6.0 # PSF
 
 # < 0.8.0/0.8 does not work, see https://bugs.launchpad.net/bugs/1153983
 SQLAlchemy>=1.3.14 # MIT
-eventlet>=0.25.1 # MIT
+eventlet>=0.33.3 # MIT
 PasteDeploy>=1.5.0 # MIT
 Routes>=2.3.1 # MIT
 WebOb>=1.8.1 # MIT
 sqlparse>=0.2.2 # BSD
 alembic>=0.9.6 # MIT
 httplib2>=0.9.1 # MIT
 oslo.config>=8.1.0 # Apache-2.0
```

### Comparing `glance-27.0.0.0b1/setup.cfg` & `glance-27.0.0.0b2/setup.cfg`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/setup.py` & `glance-27.0.0.0b2/setup.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/test-requirements.txt` & `glance-27.0.0.0b2/test-requirements.txt`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/tools/test-setup.sh` & `glance-27.0.0.0b2/tools/test-setup.sh`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/tools/test_format_inspector.py` & `glance-27.0.0.0b2/tools/test_format_inspector.py`

 * *Files identical despite different names*

### Comparing `glance-27.0.0.0b1/tox.ini` & `glance-27.0.0.0b2/tox.ini`

 * *Files identical despite different names*

