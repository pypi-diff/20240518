# Comparing `tmp/create_fastapi_project-0.2.4.tar.gz` & `tmp/create_fastapi_project-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "create_fastapi_project-0.2.4.tar", max compression
+gzip compressed data, was "create_fastapi_project-0.2.5.tar", max compression
```

## Comparing `create_fastapi_project-0.2.4.tar` & `create_fastapi_project-0.2.5.tar`

### file list

```diff
@@ -1,186 +1,184 @@
--rw-r--r--   0        0        0     1064 2023-11-02 20:11:29.226034 create_fastapi_project-0.2.4/LICENSE
--rw-r--r--   0        0        0    11309 2023-11-02 20:11:29.226034 create_fastapi_project-0.2.4/README.md
--rw-r--r--   0        0        0     6148 2023-11-02 20:11:29.226034 create_fastapi_project-0.2.4/create_fastapi_project/.DS_Store
--rw-r--r--   0        0        0       63 2023-11-02 20:11:29.226034 create_fastapi_project-0.2.4/create_fastapi_project/__main__.py
--rw-r--r--   0        0        0     1977 2023-11-02 20:11:29.226034 create_fastapi_project-0.2.4/create_fastapi_project/create_app.py
--rw-r--r--   0        0        0        0 2023-11-02 20:11:29.226034 create_fastapi_project-0.2.4/create_fastapi_project/helpers/__init__.py
--rw-r--r--   0        0        0     1975 2023-11-02 20:11:29.226034 create_fastapi_project-0.2.4/create_fastapi_project/helpers/git.py
--rw-r--r--   0        0        0     4029 2023-11-02 20:11:29.226034 create_fastapi_project-0.2.4/create_fastapi_project/helpers/install.py
--rw-r--r--   0        0        0     4052 2023-11-02 20:11:29.226034 create_fastapi_project-0.2.4/create_fastapi_project/main.py
--rw-r--r--   0        0        0     4947 2023-11-02 20:11:29.226034 create_fastapi_project-0.2.4/create_fastapi_project/templates/__init__.py
--rw-r--r--   0        0        0      214 2023-11-02 20:11:29.226034 create_fastapi_project-0.2.4/create_fastapi_project/templates/basic/.env.example
--rw-r--r--   0        0        0     1858 2023-11-02 20:11:29.226034 create_fastapi_project-0.2.4/create_fastapi_project/templates/basic/.gitignore
--rw-r--r--   0        0        0     1686 2023-11-02 20:11:29.226034 create_fastapi_project-0.2.4/create_fastapi_project/templates/basic/Makefile
--rw-r--r--   0        0        0     3334 2023-11-02 20:11:29.226034 create_fastapi_project-0.2.4/create_fastapi_project/templates/basic/README.md
--rw-r--r--   0        0        0      683 2023-11-02 20:11:29.226034 create_fastapi_project-0.2.4/create_fastapi_project/templates/basic/backend/Dockerfile
--rw-r--r--   0        0        0        0 2023-11-02 20:11:29.226034 create_fastapi_project-0.2.4/create_fastapi_project/templates/basic/backend/app/README.md
--rw-r--r--   0        0        0        0 2023-11-02 20:11:29.226034 create_fastapi_project-0.2.4/create_fastapi_project/templates/basic/backend/app/app/__init__.py
--rw-r--r--   0        0        0        0 2023-11-02 20:11:29.226034 create_fastapi_project-0.2.4/create_fastapi_project/templates/basic/backend/app/app/api/__init__.py
--rw-r--r--   0        0        0        0 2023-11-02 20:11:29.230035 create_fastapi_project-0.2.4/create_fastapi_project/templates/basic/backend/app/app/api/v1/__init__.py
--rw-r--r--   0        0        0      189 2023-11-02 20:11:29.230035 create_fastapi_project-0.2.4/create_fastapi_project/templates/basic/backend/app/app/api/v1/api.py
--rw-r--r--   0        0        0        0 2023-11-02 20:11:29.230035 create_fastapi_project-0.2.4/create_fastapi_project/templates/basic/backend/app/app/api/v1/endpoints/__init__.py
--rw-r--r--   0        0        0     3520 2023-11-02 20:11:29.230035 create_fastapi_project-0.2.4/create_fastapi_project/templates/basic/backend/app/app/api/v1/endpoints/weather.py
--rw-r--r--   0        0        0        0 2023-11-02 20:11:29.230035 create_fastapi_project-0.2.4/create_fastapi_project/templates/basic/backend/app/app/core/__init__.py
--rw-r--r--   0        0        0      620 2023-11-02 20:11:29.230035 create_fastapi_project-0.2.4/create_fastapi_project/templates/basic/backend/app/app/core/config.py
--rw-r--r--   0        0        0     1125 2023-11-02 20:11:29.230035 create_fastapi_project-0.2.4/create_fastapi_project/templates/basic/backend/app/app/main.py
--rw-r--r--   0        0        0     2666 2023-11-02 20:11:29.230035 create_fastapi_project-0.2.4/create_fastapi_project/templates/basic/backend/app/app/schemas/response_schema.py
--rw-r--r--   0        0        0        0 2023-11-02 20:11:29.230035 create_fastapi_project-0.2.4/create_fastapi_project/templates/basic/backend/app/app/utils/__init__.py
--rw-r--r--   0        0        0      317 2023-11-02 20:11:29.230035 create_fastapi_project-0.2.4/create_fastapi_project/templates/basic/backend/app/app/utils/exceptions/__init__.py
--rw-r--r--   0        0        0     2477 2023-11-02 20:11:29.230035 create_fastapi_project-0.2.4/create_fastapi_project/templates/basic/backend/app/app/utils/exceptions/common_exception.py
--rw-r--r--   0        0        0      398 2023-11-02 20:11:29.230035 create_fastapi_project-0.2.4/create_fastapi_project/templates/basic/backend/app/app/utils/exceptions/user_exceptions.py
--rw-r--r--   0        0        0     1895 2023-11-02 20:11:29.230035 create_fastapi_project-0.2.4/create_fastapi_project/templates/basic/backend/app/app/utils/exceptions/user_follow_exceptions.py
--rw-r--r--   0        0        0      608 2023-11-02 20:11:29.230035 create_fastapi_project-0.2.4/create_fastapi_project/templates/basic/backend/app/app/utils/partial.py
--rw-r--r--   0        0        0     4562 2023-11-02 20:11:29.230035 create_fastapi_project-0.2.4/create_fastapi_project/templates/basic/backend/app/app/utils/uuid6.py
--rw-r--r--   0        0        0        0 2023-11-02 20:11:29.230035 create_fastapi_project-0.2.4/create_fastapi_project/templates/basic/backend/app/test/__init__.py
--rw-r--r--   0        0        0      146 2023-11-02 20:11:29.230035 create_fastapi_project-0.2.4/create_fastapi_project/templates/basic/caddy/Caddyfile
--rw-r--r--   0        0        0      749 2023-11-02 20:11:29.230035 create_fastapi_project-0.2.4/create_fastapi_project/templates/basic/docker-compose-dev.yml
--rw-r--r--   0        0        0      797 2023-11-02 20:11:29.230035 create_fastapi_project-0.2.4/create_fastapi_project/templates/basic/docker-compose.yml
--rw-r--r--   0        0        0     1497 2023-11-02 20:11:29.230035 create_fastapi_project-0.2.4/create_fastapi_project/templates/full/.env.example
--rw-r--r--   0        0        0     1858 2023-11-02 20:11:29.230035 create_fastapi_project-0.2.4/create_fastapi_project/templates/full/.gitignore
--rw-r--r--   0        0        0     1072 2023-11-02 20:11:29.230035 create_fastapi_project-0.2.4/create_fastapi_project/templates/full/LICENSE
--rw-r--r--   0        0        0     3767 2023-11-02 20:11:29.230035 create_fastapi_project-0.2.4/create_fastapi_project/templates/full/Makefile
--rw-r--r--   0        0        0    20374 2023-11-02 20:11:29.230035 create_fastapi_project-0.2.4/create_fastapi_project/templates/full/README.md
--rw-r--r--   0        0        0        0 2023-11-02 20:11:29.230035 create_fastapi_project-0.2.4/create_fastapi_project/templates/full/__init__.py
--rw-r--r--   0        0        0      699 2023-11-02 20:11:29.230035 create_fastapi_project-0.2.4/create_fastapi_project/templates/full/backend/Dockerfile
--rw-r--r--   0        0        0        0 2023-11-02 20:11:29.230035 create_fastapi_project-0.2.4/create_fastapi_project/templates/full/backend/app/README.md
--rw-r--r--   0        0        0       38 2023-11-02 20:11:29.230035 create_fastapi_project-0.2.4/create_fastapi_project/templates/full/backend/app/alembic/README
--rw-r--r--   0        0        0     2285 2023-11-02 20:11:29.230035 create_fastapi_project-0.2.4/create_fastapi_project/templates/full/backend/app/alembic/env.py
--rw-r--r--   0        0        0      600 2023-11-02 20:11:29.230035 create_fastapi_project-0.2.4/create_fastapi_project/templates/full/backend/app/alembic/script.py.mako
--rw-r--r--   0        0        0     6644 2023-11-02 20:11:29.230035 create_fastapi_project-0.2.4/create_fastapi_project/templates/full/backend/app/alembic/versions/2022-09-25-19-46_60d49bf413b8.py
--rw-r--r--   0        0        0     2384 2023-11-02 20:11:29.230035 create_fastapi_project-0.2.4/create_fastapi_project/templates/full/backend/app/alembic/versions/2022-10-03-18-32_3223652d21bd.py
--rw-r--r--   0        0        0     1666 2023-11-02 20:11:29.230035 create_fastapi_project-0.2.4/create_fastapi_project/templates/full/backend/app/alembic/versions/2022-10-23-04-07_cc36a024e8ed.py
--rw-r--r--   0        0        0      892 2023-11-02 20:11:29.230035 create_fastapi_project-0.2.4/create_fastapi_project/templates/full/backend/app/alembic/versions/2022-11-03-14-16_3293815eb23c.py
--rw-r--r--   0        0        0      854 2023-11-02 20:11:29.230035 create_fastapi_project-0.2.4/create_fastapi_project/templates/full/backend/app/alembic/versions/2023-03-04-23-15_5591a516fc47.py
--rw-r--r--   0        0        0      659 2023-11-02 20:11:29.230035 create_fastapi_project-0.2.4/create_fastapi_project/templates/full/backend/app/alembic/versions/2023-03-17-17-34_13d2068684ab.py
--rw-r--r--   0        0        0     1676 2023-11-02 20:11:29.230035 create_fastapi_project-0.2.4/create_fastapi_project/templates/full/backend/app/alembic.ini
--rw-r--r--   0        0        0        0 2023-11-02 20:11:29.230035 create_fastapi_project-0.2.4/create_fastapi_project/templates/full/backend/app/app/__init__.py
--rw-r--r--   0        0        0        0 2023-11-02 20:11:29.230035 create_fastapi_project-0.2.4/create_fastapi_project/templates/full/backend/app/app/api/__init__.py
--rw-r--r--   0        0        0      727 2023-11-02 20:11:29.230035 create_fastapi_project-0.2.4/create_fastapi_project/templates/full/backend/app/app/api/celery_task.py
--rw-r--r--   0        0        0     3376 2023-11-02 20:11:29.230035 create_fastapi_project-0.2.4/create_fastapi_project/templates/full/backend/app/app/api/deps.py
--rw-r--r--   0        0        0        0 2023-11-02 20:11:29.230035 create_fastapi_project-0.2.4/create_fastapi_project/templates/full/backend/app/app/api/v1/__init__.py
--rw-r--r--   0        0        0      971 2023-11-02 20:11:29.230035 create_fastapi_project-0.2.4/create_fastapi_project/templates/full/backend/app/app/api/v1/api.py
--rw-r--r--   0        0        0        0 2023-11-02 20:11:29.230035 create_fastapi_project-0.2.4/create_fastapi_project/templates/full/backend/app/app/api/v1/endpoints/__init__.py
--rw-r--r--   0        0        0     2054 2023-11-02 20:11:29.230035 create_fastapi_project-0.2.4/create_fastapi_project/templates/full/backend/app/app/api/v1/endpoints/cache.py
--rw-r--r--   0        0        0     3122 2023-11-02 20:11:29.230035 create_fastapi_project-0.2.4/create_fastapi_project/templates/full/backend/app/app/api/v1/endpoints/group.py
--rw-r--r--   0        0        0     4336 2023-11-02 20:11:29.230035 create_fastapi_project-0.2.4/create_fastapi_project/templates/full/backend/app/app/api/v1/endpoints/hero.py
--rw-r--r--   0        0        0     7902 2023-11-02 20:11:29.230035 create_fastapi_project-0.2.4/create_fastapi_project/templates/full/backend/app/app/api/v1/endpoints/login.py
--rw-r--r--   0        0        0     3884 2023-11-02 20:11:29.230035 create_fastapi_project-0.2.4/create_fastapi_project/templates/full/backend/app/app/api/v1/endpoints/periodic_tasks.py
--rw-r--r--   0        0        0     3376 2023-11-02 20:11:29.230035 create_fastapi_project-0.2.4/create_fastapi_project/templates/full/backend/app/app/api/v1/endpoints/report.py
--rw-r--r--   0        0        0     2515 2023-11-02 20:11:29.230035 create_fastapi_project-0.2.4/create_fastapi_project/templates/full/backend/app/app/api/v1/endpoints/role.py
--rw-r--r--   0        0        0     3466 2023-11-02 20:11:29.230035 create_fastapi_project-0.2.4/create_fastapi_project/templates/full/backend/app/app/api/v1/endpoints/team.py
--rw-r--r--   0        0        0    14433 2023-11-02 20:11:29.230035 create_fastapi_project-0.2.4/create_fastapi_project/templates/full/backend/app/app/api/v1/endpoints/user.py
--rw-r--r--   0        0        0     3622 2023-11-02 20:11:29.230035 create_fastapi_project-0.2.4/create_fastapi_project/templates/full/backend/app/app/api/v1/endpoints/weather.py
--rw-r--r--   0        0        0        0 2023-11-02 20:11:29.230035 create_fastapi_project-0.2.4/create_fastapi_project/templates/full/backend/app/app/core/__init__.py
--rw-r--r--   0        0        0     1095 2023-11-02 20:11:29.230035 create_fastapi_project-0.2.4/create_fastapi_project/templates/full/backend/app/app/core/authz.polar
--rw-r--r--   0        0        0      385 2023-11-02 20:11:29.230035 create_fastapi_project-0.2.4/create_fastapi_project/templates/full/backend/app/app/core/authz.py
--rw-r--r--   0        0        0      627 2023-11-02 20:11:29.230035 create_fastapi_project-0.2.4/create_fastapi_project/templates/full/backend/app/app/core/celery.py
--rw-r--r--   0        0        0     4088 2023-11-02 20:11:29.230035 create_fastapi_project-0.2.4/create_fastapi_project/templates/full/backend/app/app/core/config.py
--rw-r--r--   0        0        0     1676 2023-11-02 20:11:29.230035 create_fastapi_project-0.2.4/create_fastapi_project/templates/full/backend/app/app/core/security.py
--rw-r--r--   0        0        0      220 2023-11-02 20:11:29.230035 create_fastapi_project-0.2.4/create_fastapi_project/templates/full/backend/app/app/crud/__init__.py
--rw-r--r--   0        0        0     6856 2023-11-02 20:11:29.230035 create_fastapi_project-0.2.4/create_fastapi_project/templates/full/backend/app/app/crud/base_crud.py
--rw-r--r--   0        0        0     1474 2023-11-02 20:11:29.230035 create_fastapi_project-0.2.4/create_fastapi_project/templates/full/backend/app/app/crud/group_crud.py
--rw-r--r--   0        0        0     1347 2023-11-02 20:11:29.230035 create_fastapi_project-0.2.4/create_fastapi_project/templates/full/backend/app/app/crud/hero_crud.py
--rw-r--r--   0        0        0      302 2023-11-02 20:11:29.230035 create_fastapi_project-0.2.4/create_fastapi_project/templates/full/backend/app/app/crud/image_media_crud.py
--rw-r--r--   0        0        0      983 2023-11-02 20:11:29.230035 create_fastapi_project-0.2.4/create_fastapi_project/templates/full/backend/app/app/crud/role_crud.py
--rw-r--r--   0        0        0      600 2023-11-02 20:11:29.230035 create_fastapi_project-0.2.4/create_fastapi_project/templates/full/backend/app/app/crud/team_crud.py
--rw-r--r--   0        0        0     3981 2023-11-02 20:11:29.230035 create_fastapi_project-0.2.4/create_fastapi_project/templates/full/backend/app/app/crud/user_crud.py
--rw-r--r--   0        0        0     3752 2023-11-02 20:11:29.230035 create_fastapi_project-0.2.4/create_fastapi_project/templates/full/backend/app/app/crud/user_follow_crud.py
--rw-r--r--   0        0        0     6148 2023-11-02 20:11:29.230035 create_fastapi_project-0.2.4/create_fastapi_project/templates/full/backend/app/app/db/.DS_Store
--rw-r--r--   0        0        0        0 2023-11-02 20:11:29.230035 create_fastapi_project-0.2.4/create_fastapi_project/templates/full/backend/app/app/db/__init__.py
--rw-r--r--   0        0        0     4681 2023-11-02 20:11:29.230035 create_fastapi_project-0.2.4/create_fastapi_project/templates/full/backend/app/app/db/init_db.py
--rw-r--r--   0        0        0     1247 2023-11-02 20:11:29.230035 create_fastapi_project-0.2.4/create_fastapi_project/templates/full/backend/app/app/db/session.py
--rw-r--r--   0        0        0      364 2023-11-02 20:11:29.230035 create_fastapi_project-0.2.4/create_fastapi_project/templates/full/backend/app/app/deps/celery_deps.py
--rw-r--r--   0        0        0      824 2023-11-02 20:11:29.230035 create_fastapi_project-0.2.4/create_fastapi_project/templates/full/backend/app/app/deps/group_deps.py
--rw-r--r--   0        0        0      790 2023-11-02 20:11:29.230035 create_fastapi_project-0.2.4/create_fastapi_project/templates/full/backend/app/app/deps/role_deps.py
--rw-r--r--   0        0        0     1299 2023-11-02 20:11:29.230035 create_fastapi_project-0.2.4/create_fastapi_project/templates/full/backend/app/app/deps/user_deps.py
--rw-r--r--   0        0        0      313 2023-11-02 20:11:29.230035 create_fastapi_project-0.2.4/create_fastapi_project/templates/full/backend/app/app/initial_data.py
--rw-r--r--   0        0        0     7181 2023-11-02 20:11:29.230035 create_fastapi_project-0.2.4/create_fastapi_project/templates/full/backend/app/app/main.py
--rw-r--r--   0        0        0      262 2023-11-02 20:11:29.230035 create_fastapi_project-0.2.4/create_fastapi_project/templates/full/backend/app/app/models/__init__.py
--rw-r--r--   0        0        0      698 2023-11-02 20:11:29.230035 create_fastapi_project-0.2.4/create_fastapi_project/templates/full/backend/app/app/models/base_uuid_model.py
--rw-r--r--   0        0        0      740 2023-11-02 20:11:29.230035 create_fastapi_project-0.2.4/create_fastapi_project/templates/full/backend/app/app/models/group_model.py
--rw-r--r--   0        0        0      778 2023-11-02 20:11:29.230035 create_fastapi_project-0.2.4/create_fastapi_project/templates/full/backend/app/app/models/hero_model.py
--rw-r--r--   0        0        0      571 2023-11-02 20:11:29.230035 create_fastapi_project-0.2.4/create_fastapi_project/templates/full/backend/app/app/models/image_media_model.py
--rw-r--r--   0        0        0      390 2023-11-02 20:11:29.230035 create_fastapi_project-0.2.4/create_fastapi_project/templates/full/backend/app/app/models/links_model.py
--rw-r--r--   0        0        0      631 2023-11-02 20:11:29.230035 create_fastapi_project-0.2.4/create_fastapi_project/templates/full/backend/app/app/models/media_model.py
--rw-r--r--   0        0        0      346 2023-11-02 20:11:29.230035 create_fastapi_project-0.2.4/create_fastapi_project/templates/full/backend/app/app/models/role_model.py
--rw-r--r--   0        0        0      663 2023-11-02 20:11:29.230035 create_fastapi_project-0.2.4/create_fastapi_project/templates/full/backend/app/app/models/team_model.py
--rw-r--r--   0        0        0      402 2023-11-02 20:11:29.230035 create_fastapi_project-0.2.4/create_fastapi_project/templates/full/backend/app/app/models/user_follow_model.py
--rw-r--r--   0        0        0     2049 2023-11-02 20:11:29.230035 create_fastapi_project-0.2.4/create_fastapi_project/templates/full/backend/app/app/models/user_model.py
--rw-r--r--   0        0        0     1312 2023-11-02 20:11:29.230035 create_fastapi_project-0.2.4/create_fastapi_project/templates/full/backend/app/app/schemas/common_schema.py
--rw-r--r--   0        0        0      429 2023-11-02 20:11:29.230035 create_fastapi_project-0.2.4/create_fastapi_project/templates/full/backend/app/app/schemas/group_schema.py
--rw-r--r--   0        0        0      606 2023-11-02 20:11:29.230035 create_fastapi_project-0.2.4/create_fastapi_project/templates/full/backend/app/app/schemas/hero_schema.py
--rw-r--r--   0        0        0     1022 2023-11-02 20:11:29.230035 create_fastapi_project-0.2.4/create_fastapi_project/templates/full/backend/app/app/schemas/image_media_schema.py
--rw-r--r--   0        0        0      303 2023-11-02 20:11:29.230035 create_fastapi_project-0.2.4/create_fastapi_project/templates/full/backend/app/app/schemas/media_schema.py
--rw-r--r--   0        0        0     2666 2023-11-02 20:11:29.230035 create_fastapi_project-0.2.4/create_fastapi_project/templates/full/backend/app/app/schemas/response_schema.py
--rw-r--r--   0        0        0      382 2023-11-02 20:11:29.230035 create_fastapi_project-0.2.4/create_fastapi_project/templates/full/backend/app/app/schemas/role_schema.py
--rw-r--r--   0        0        0      463 2023-11-02 20:11:29.230035 create_fastapi_project-0.2.4/create_fastapi_project/templates/full/backend/app/app/schemas/team_schema.py
--rw-r--r--   0        0        0      305 2023-11-02 20:11:29.230035 create_fastapi_project-0.2.4/create_fastapi_project/templates/full/backend/app/app/schemas/token_schema.py
--rw-r--r--   0        0        0      518 2023-11-02 20:11:29.230035 create_fastapi_project-0.2.4/create_fastapi_project/templates/full/backend/app/app/schemas/user_follow_schema.py
--rw-r--r--   0        0        0     1181 2023-11-02 20:11:29.230035 create_fastapi_project-0.2.4/create_fastapi_project/templates/full/backend/app/app/schemas/user_schema.py
--rw-r--r--   0        0        0        0 2023-11-02 20:11:29.230035 create_fastapi_project-0.2.4/create_fastapi_project/templates/full/backend/app/app/utils/__init__.py
--rw-r--r--   0        0        0      317 2023-11-02 20:11:29.230035 create_fastapi_project-0.2.4/create_fastapi_project/templates/full/backend/app/app/utils/exceptions/__init__.py
--rw-r--r--   0        0        0     2477 2023-11-02 20:11:29.230035 create_fastapi_project-0.2.4/create_fastapi_project/templates/full/backend/app/app/utils/exceptions/common_exception.py
--rw-r--r--   0        0        0      398 2023-11-02 20:11:29.234035 create_fastapi_project-0.2.4/create_fastapi_project/templates/full/backend/app/app/utils/exceptions/user_exceptions.py
--rw-r--r--   0        0        0     1895 2023-11-02 20:11:29.234035 create_fastapi_project-0.2.4/create_fastapi_project/templates/full/backend/app/app/utils/exceptions/user_follow_exceptions.py
--rw-r--r--   0        0        0     4018 2023-11-02 20:11:29.234035 create_fastapi_project-0.2.4/create_fastapi_project/templates/full/backend/app/app/utils/fastapi_globals.py
--rw-r--r--   0        0        0      317 2023-11-02 20:11:29.234035 create_fastapi_project-0.2.4/create_fastapi_project/templates/full/backend/app/app/utils/map_schema.py
--rw-r--r--   0        0        0     2210 2023-11-02 20:11:29.234035 create_fastapi_project-0.2.4/create_fastapi_project/templates/full/backend/app/app/utils/minio_client.py
--rw-r--r--   0        0        0      608 2023-11-02 20:11:29.234035 create_fastapi_project-0.2.4/create_fastapi_project/templates/full/backend/app/app/utils/partial.py
--rw-r--r--   0        0        0      341 2023-11-02 20:11:29.234035 create_fastapi_project-0.2.4/create_fastapi_project/templates/full/backend/app/app/utils/print_model.py
--rw-r--r--   0        0        0      279 2023-11-02 20:11:29.234035 create_fastapi_project-0.2.4/create_fastapi_project/templates/full/backend/app/app/utils/requestvars.py
--rw-r--r--   0        0        0      751 2023-11-02 20:11:29.234035 create_fastapi_project-0.2.4/create_fastapi_project/templates/full/backend/app/app/utils/resize_image.py
--rw-r--r--   0        0        0     1475 2023-11-02 20:11:29.234035 create_fastapi_project-0.2.4/create_fastapi_project/templates/full/backend/app/app/utils/snowflake.py
--rw-r--r--   0        0        0     1083 2023-11-02 20:11:29.234035 create_fastapi_project-0.2.4/create_fastapi_project/templates/full/backend/app/app/utils/token.py
--rw-r--r--   0        0        0     4562 2023-11-02 20:11:29.234035 create_fastapi_project-0.2.4/create_fastapi_project/templates/full/backend/app/app/utils/uuid6.py
--rw-r--r--   0        0        0        0 2023-11-02 20:11:29.234035 create_fastapi_project-0.2.4/create_fastapi_project/templates/full/backend/app/test/__init__.py
--rw-r--r--   0        0        0        0 2023-11-02 20:11:29.234035 create_fastapi_project-0.2.4/create_fastapi_project/templates/full/backend/app/test/api/__init__.py
--rw-r--r--   0        0        0     2018 2023-11-02 20:11:29.234035 create_fastapi_project-0.2.4/create_fastapi_project/templates/full/backend/app/test/api/test_login.py
--rw-r--r--   0        0        0     2271 2023-11-02 20:11:29.234035 create_fastapi_project-0.2.4/create_fastapi_project/templates/full/backend/app/test/api/test_user.py
--rw-r--r--   0        0        0      653 2023-11-02 20:11:29.234035 create_fastapi_project-0.2.4/create_fastapi_project/templates/full/backend/app/test/test_main.py
--rw-r--r--   0        0        0      652 2023-11-02 20:11:29.234035 create_fastapi_project-0.2.4/create_fastapi_project/templates/full/backend/sonar-project.properties
--rw-r--r--   0        0        0      971 2023-11-02 20:11:29.234035 create_fastapi_project-0.2.4/create_fastapi_project/templates/full/caddy/Caddyfile
--rw-r--r--   0        0        0       65 2023-11-02 20:11:29.234035 create_fastapi_project-0.2.4/create_fastapi_project/templates/full/create-dbs.sql
--rw-r--r--   0        0        0     3109 2023-11-02 20:11:29.234035 create_fastapi_project-0.2.4/create_fastapi_project/templates/full/docker-compose-dev.yml
--rw-r--r--   0        0        0      346 2023-11-02 20:11:29.234035 create_fastapi_project-0.2.4/create_fastapi_project/templates/full/docker-compose-sonarqube.yml
--rw-r--r--   0        0        0     3121 2023-11-02 20:11:29.234035 create_fastapi_project-0.2.4/create_fastapi_project/templates/full/docker-compose-test.yml
--rw-r--r--   0        0        0     3138 2023-11-02 20:11:29.234035 create_fastapi_project-0.2.4/create_fastapi_project/templates/full/docker-compose.yml
--rw-r--r--   0        0        0        0 2023-11-02 20:11:29.234035 create_fastapi_project-0.2.4/create_fastapi_project/templates/full/eslintrc.json
--rw-r--r--   0        0        0      243 2023-11-02 20:11:29.234035 create_fastapi_project-0.2.4/create_fastapi_project/templates/full/pgadmin/servers.json
--rw-r--r--   0        0        0      895 2023-11-02 20:11:29.234035 create_fastapi_project-0.2.4/create_fastapi_project/templates/full/pgadmin.yml
--rw-r--r--   0        0        0      263 2023-11-02 20:11:29.234035 create_fastapi_project-0.2.4/create_fastapi_project/templates/langchain_basic/.env.example
--rw-r--r--   0        0        0     1858 2023-11-02 20:11:29.234035 create_fastapi_project-0.2.4/create_fastapi_project/templates/langchain_basic/.gitignore
--rw-r--r--   0        0        0     1686 2023-11-02 20:11:29.234035 create_fastapi_project-0.2.4/create_fastapi_project/templates/langchain_basic/Makefile
--rw-r--r--   0        0        0     6060 2023-11-02 20:11:29.234035 create_fastapi_project-0.2.4/create_fastapi_project/templates/langchain_basic/README.md
--rw-r--r--   0        0        0      683 2023-11-02 20:11:29.234035 create_fastapi_project-0.2.4/create_fastapi_project/templates/langchain_basic/backend/Dockerfile
--rw-r--r--   0        0        0        0 2023-11-02 20:11:29.234035 create_fastapi_project-0.2.4/create_fastapi_project/templates/langchain_basic/backend/app/README.md
--rw-r--r--   0        0        0        0 2023-11-02 20:11:29.234035 create_fastapi_project-0.2.4/create_fastapi_project/templates/langchain_basic/backend/app/app/__init__.py
--rw-r--r--   0        0        0        0 2023-11-02 20:11:29.234035 create_fastapi_project-0.2.4/create_fastapi_project/templates/langchain_basic/backend/app/app/api/__init__.py
--rw-r--r--   0        0        0        0 2023-11-02 20:11:29.234035 create_fastapi_project-0.2.4/create_fastapi_project/templates/langchain_basic/backend/app/app/api/v1/__init__.py
--rw-r--r--   0        0        0      173 2023-11-02 20:11:29.234035 create_fastapi_project-0.2.4/create_fastapi_project/templates/langchain_basic/backend/app/app/api/v1/api.py
--rw-r--r--   0        0        0        0 2023-11-02 20:11:29.234035 create_fastapi_project-0.2.4/create_fastapi_project/templates/langchain_basic/backend/app/app/api/v1/endpoints/__init__.py
--rw-r--r--   0        0        0     4890 2023-11-02 20:11:29.234035 create_fastapi_project-0.2.4/create_fastapi_project/templates/langchain_basic/backend/app/app/api/v1/endpoints/chat.py
--rw-r--r--   0        0        0        0 2023-11-02 20:11:29.234035 create_fastapi_project-0.2.4/create_fastapi_project/templates/langchain_basic/backend/app/app/core/__init__.py
--rw-r--r--   0        0        0      617 2023-11-02 20:11:29.234035 create_fastapi_project-0.2.4/create_fastapi_project/templates/langchain_basic/backend/app/app/core/config.py
--rw-r--r--   0        0        0     1478 2023-11-02 20:11:29.234035 create_fastapi_project-0.2.4/create_fastapi_project/templates/langchain_basic/backend/app/app/main.py
--rw-r--r--   0        0        0      144 2023-11-02 20:11:29.234035 create_fastapi_project-0.2.4/create_fastapi_project/templates/langchain_basic/backend/app/app/schemas/adaptive_cards_schema.py
--rw-r--r--   0        0        0      931 2023-11-02 20:11:29.234035 create_fastapi_project-0.2.4/create_fastapi_project/templates/langchain_basic/backend/app/app/schemas/message_schema.py
--rw-r--r--   0        0        0     2666 2023-11-02 20:11:29.234035 create_fastapi_project-0.2.4/create_fastapi_project/templates/langchain_basic/backend/app/app/schemas/response_schema.py
--rw-r--r--   0        0        0      702 2023-11-02 20:11:29.234035 create_fastapi_project-0.2.4/create_fastapi_project/templates/langchain_basic/backend/app/app/templates/chat.py
--rw-r--r--   0        0        0        0 2023-11-02 20:11:29.234035 create_fastapi_project-0.2.4/create_fastapi_project/templates/langchain_basic/backend/app/app/utils/__init__.py
--rw-r--r--   0        0        0     4959 2023-11-02 20:11:29.234035 create_fastapi_project-0.2.4/create_fastapi_project/templates/langchain_basic/backend/app/app/utils/adaptive_cards/cards.py
--rw-r--r--   0        0        0    10084 2023-11-02 20:11:29.234035 create_fastapi_project-0.2.4/create_fastapi_project/templates/langchain_basic/backend/app/app/utils/callback.py
--rw-r--r--   0        0        0     1179 2023-11-02 20:11:29.234035 create_fastapi_project-0.2.4/create_fastapi_project/templates/langchain_basic/backend/app/app/utils/chains.py
--rw-r--r--   0        0        0      317 2023-11-02 20:11:29.234035 create_fastapi_project-0.2.4/create_fastapi_project/templates/langchain_basic/backend/app/app/utils/exceptions/__init__.py
--rw-r--r--   0        0        0     2477 2023-11-02 20:11:29.234035 create_fastapi_project-0.2.4/create_fastapi_project/templates/langchain_basic/backend/app/app/utils/exceptions/common_exception.py
--rw-r--r--   0        0        0      608 2023-11-02 20:11:29.234035 create_fastapi_project-0.2.4/create_fastapi_project/templates/langchain_basic/backend/app/app/utils/partial.py
--rw-r--r--   0        0        0     1502 2023-11-02 20:11:29.234035 create_fastapi_project-0.2.4/create_fastapi_project/templates/langchain_basic/backend/app/app/utils/prompt_zero.py
--rw-r--r--   0        0        0     6275 2023-11-02 20:11:29.234035 create_fastapi_project-0.2.4/create_fastapi_project/templates/langchain_basic/backend/app/app/utils/tools.py
--rw-r--r--   0        0        0     4562 2023-11-02 20:11:29.234035 create_fastapi_project-0.2.4/create_fastapi_project/templates/langchain_basic/backend/app/app/utils/uuid6.py
--rw-r--r--   0        0        0      270 2023-11-02 20:11:29.234035 create_fastapi_project-0.2.4/create_fastapi_project/templates/langchain_basic/caddy/Caddyfile
--rw-r--r--   0        0        0      983 2023-11-02 20:11:29.234035 create_fastapi_project-0.2.4/create_fastapi_project/templates/langchain_basic/docker-compose-dev.yml
--rw-r--r--   0        0        0     1066 2023-11-02 20:11:29.234035 create_fastapi_project-0.2.4/create_fastapi_project/templates/langchain_basic/docker-compose.yml
--rw-r--r--   0        0        0      701 2023-11-02 20:11:29.234035 create_fastapi_project-0.2.4/create_fastapi_project/templates/langchain_basic/frontend/Dockerfile
--rw-r--r--   0        0        0     2345 2023-11-02 20:11:29.234035 create_fastapi_project-0.2.4/create_fastapi_project/templates/langchain_basic/frontend/app/main.py
--rw-r--r--   0        0        0      307 2023-11-02 20:11:29.234035 create_fastapi_project-0.2.4/create_fastapi_project/templates/langchain_basic/streamlit.yml
--rw-r--r--   0        0        0     1456 2023-11-02 20:11:40.618399 create_fastapi_project-0.2.4/pyproject.toml
--rw-r--r--   0        0        0    11830 1970-01-01 00:00:00.000000 create_fastapi_project-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-05-18 16:03:12.200227 create_fastapi_project-0.2.5/LICENSE
+-rw-r--r--   0        0        0    11309 2024-05-18 16:03:12.200227 create_fastapi_project-0.2.5/README.md
+-rw-r--r--   0        0        0     6148 2024-05-18 16:03:12.200227 create_fastapi_project-0.2.5/create_fastapi_project/.DS_Store
+-rw-r--r--   0        0        0       63 2024-05-18 16:03:12.200227 create_fastapi_project-0.2.5/create_fastapi_project/__main__.py
+-rw-r--r--   0        0        0     1977 2024-05-18 16:03:12.200227 create_fastapi_project-0.2.5/create_fastapi_project/create_app.py
+-rw-r--r--   0        0        0        0 2024-05-18 16:03:12.200227 create_fastapi_project-0.2.5/create_fastapi_project/helpers/__init__.py
+-rw-r--r--   0        0        0     1975 2024-05-18 16:03:12.200227 create_fastapi_project-0.2.5/create_fastapi_project/helpers/git.py
+-rw-r--r--   0        0        0     4029 2024-05-18 16:03:12.200227 create_fastapi_project-0.2.5/create_fastapi_project/helpers/install.py
+-rw-r--r--   0        0        0     4052 2024-05-18 16:03:12.200227 create_fastapi_project-0.2.5/create_fastapi_project/main.py
+-rw-r--r--   0        0        0     4516 2024-05-18 16:03:12.200227 create_fastapi_project-0.2.5/create_fastapi_project/templates/__init__.py
+-rw-r--r--   0        0        0      214 2024-05-18 16:03:12.200227 create_fastapi_project-0.2.5/create_fastapi_project/templates/basic/.env.example
+-rw-r--r--   0        0        0     1858 2024-05-18 16:03:12.200227 create_fastapi_project-0.2.5/create_fastapi_project/templates/basic/.gitignore
+-rw-r--r--   0        0        0     1686 2024-05-18 16:03:12.200227 create_fastapi_project-0.2.5/create_fastapi_project/templates/basic/Makefile
+-rw-r--r--   0        0        0     3334 2024-05-18 16:03:12.200227 create_fastapi_project-0.2.5/create_fastapi_project/templates/basic/README.md
+-rw-r--r--   0        0        0      719 2024-05-18 16:03:12.200227 create_fastapi_project-0.2.5/create_fastapi_project/templates/basic/backend/Dockerfile
+-rw-r--r--   0        0        0        0 2024-05-18 16:03:12.200227 create_fastapi_project-0.2.5/create_fastapi_project/templates/basic/backend/app/README.md
+-rw-r--r--   0        0        0        0 2024-05-18 16:03:12.200227 create_fastapi_project-0.2.5/create_fastapi_project/templates/basic/backend/app/app/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-18 16:03:12.200227 create_fastapi_project-0.2.5/create_fastapi_project/templates/basic/backend/app/app/api/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-18 16:03:12.200227 create_fastapi_project-0.2.5/create_fastapi_project/templates/basic/backend/app/app/api/v1/__init__.py
+-rw-r--r--   0        0        0      189 2024-05-18 16:03:12.200227 create_fastapi_project-0.2.5/create_fastapi_project/templates/basic/backend/app/app/api/v1/api.py
+-rw-r--r--   0        0        0        0 2024-05-18 16:03:12.200227 create_fastapi_project-0.2.5/create_fastapi_project/templates/basic/backend/app/app/api/v1/endpoints/__init__.py
+-rw-r--r--   0        0        0     3520 2024-05-18 16:03:12.200227 create_fastapi_project-0.2.5/create_fastapi_project/templates/basic/backend/app/app/api/v1/endpoints/weather.py
+-rw-r--r--   0        0        0        0 2024-05-18 16:03:12.200227 create_fastapi_project-0.2.5/create_fastapi_project/templates/basic/backend/app/app/core/__init__.py
+-rw-r--r--   0        0        0      640 2024-05-18 16:03:12.200227 create_fastapi_project-0.2.5/create_fastapi_project/templates/basic/backend/app/app/core/config.py
+-rw-r--r--   0        0        0     1125 2024-05-18 16:03:12.200227 create_fastapi_project-0.2.5/create_fastapi_project/templates/basic/backend/app/app/main.py
+-rw-r--r--   0        0        0     2666 2024-05-18 16:03:12.200227 create_fastapi_project-0.2.5/create_fastapi_project/templates/basic/backend/app/app/schemas/response_schema.py
+-rw-r--r--   0        0        0        0 2024-05-18 16:03:12.200227 create_fastapi_project-0.2.5/create_fastapi_project/templates/basic/backend/app/app/utils/__init__.py
+-rw-r--r--   0        0        0      317 2024-05-18 16:03:12.200227 create_fastapi_project-0.2.5/create_fastapi_project/templates/basic/backend/app/app/utils/exceptions/__init__.py
+-rw-r--r--   0        0        0     2477 2024-05-18 16:03:12.200227 create_fastapi_project-0.2.5/create_fastapi_project/templates/basic/backend/app/app/utils/exceptions/common_exception.py
+-rw-r--r--   0        0        0      398 2024-05-18 16:03:12.200227 create_fastapi_project-0.2.5/create_fastapi_project/templates/basic/backend/app/app/utils/exceptions/user_exceptions.py
+-rw-r--r--   0        0        0     1895 2024-05-18 16:03:12.200227 create_fastapi_project-0.2.5/create_fastapi_project/templates/basic/backend/app/app/utils/exceptions/user_follow_exceptions.py
+-rw-r--r--   0        0        0      608 2024-05-18 16:03:12.200227 create_fastapi_project-0.2.5/create_fastapi_project/templates/basic/backend/app/app/utils/partial.py
+-rw-r--r--   0        0        0     4562 2024-05-18 16:03:12.200227 create_fastapi_project-0.2.5/create_fastapi_project/templates/basic/backend/app/app/utils/uuid6.py
+-rw-r--r--   0        0        0        0 2024-05-18 16:03:12.200227 create_fastapi_project-0.2.5/create_fastapi_project/templates/basic/backend/app/test/__init__.py
+-rw-r--r--   0        0        0      146 2024-05-18 16:03:12.200227 create_fastapi_project-0.2.5/create_fastapi_project/templates/basic/caddy/Caddyfile
+-rw-r--r--   0        0        0      749 2024-05-18 16:03:12.200227 create_fastapi_project-0.2.5/create_fastapi_project/templates/basic/docker-compose-dev.yml
+-rw-r--r--   0        0        0      797 2024-05-18 16:03:12.200227 create_fastapi_project-0.2.5/create_fastapi_project/templates/basic/docker-compose.yml
+-rw-r--r--   0        0        0     1497 2024-05-18 16:03:12.200227 create_fastapi_project-0.2.5/create_fastapi_project/templates/full/.env.example
+-rw-r--r--   0        0        0     1858 2024-05-18 16:03:12.200227 create_fastapi_project-0.2.5/create_fastapi_project/templates/full/.gitignore
+-rw-r--r--   0        0        0     1072 2024-05-18 16:03:12.200227 create_fastapi_project-0.2.5/create_fastapi_project/templates/full/LICENSE
+-rw-r--r--   0        0        0     3767 2024-05-18 16:03:12.200227 create_fastapi_project-0.2.5/create_fastapi_project/templates/full/Makefile
+-rw-r--r--   0        0        0    20374 2024-05-18 16:03:12.200227 create_fastapi_project-0.2.5/create_fastapi_project/templates/full/README.md
+-rw-r--r--   0        0        0        0 2024-05-18 16:03:12.200227 create_fastapi_project-0.2.5/create_fastapi_project/templates/full/__init__.py
+-rw-r--r--   0        0        0      719 2024-05-18 16:03:12.200227 create_fastapi_project-0.2.5/create_fastapi_project/templates/full/backend/Dockerfile
+-rw-r--r--   0        0        0        0 2024-05-18 16:03:12.200227 create_fastapi_project-0.2.5/create_fastapi_project/templates/full/backend/app/README.md
+-rw-r--r--   0        0        0       38 2024-05-18 16:03:12.200227 create_fastapi_project-0.2.5/create_fastapi_project/templates/full/backend/app/alembic/README
+-rw-r--r--   0        0        0     2285 2024-05-18 16:03:12.200227 create_fastapi_project-0.2.5/create_fastapi_project/templates/full/backend/app/alembic/env.py
+-rw-r--r--   0        0        0      600 2024-05-18 16:03:12.200227 create_fastapi_project-0.2.5/create_fastapi_project/templates/full/backend/app/alembic/script.py.mako
+-rw-r--r--   0        0        0     6644 2024-05-18 16:03:12.200227 create_fastapi_project-0.2.5/create_fastapi_project/templates/full/backend/app/alembic/versions/2022-09-25-19-46_60d49bf413b8.py
+-rw-r--r--   0        0        0     2384 2024-05-18 16:03:12.200227 create_fastapi_project-0.2.5/create_fastapi_project/templates/full/backend/app/alembic/versions/2022-10-03-18-32_3223652d21bd.py
+-rw-r--r--   0        0        0     1666 2024-05-18 16:03:12.200227 create_fastapi_project-0.2.5/create_fastapi_project/templates/full/backend/app/alembic/versions/2022-10-23-04-07_cc36a024e8ed.py
+-rw-r--r--   0        0        0      892 2024-05-18 16:03:12.204227 create_fastapi_project-0.2.5/create_fastapi_project/templates/full/backend/app/alembic/versions/2022-11-03-14-16_3293815eb23c.py
+-rw-r--r--   0        0        0      854 2024-05-18 16:03:12.204227 create_fastapi_project-0.2.5/create_fastapi_project/templates/full/backend/app/alembic/versions/2023-03-04-23-15_5591a516fc47.py
+-rw-r--r--   0        0        0      659 2024-05-18 16:03:12.204227 create_fastapi_project-0.2.5/create_fastapi_project/templates/full/backend/app/alembic/versions/2023-03-17-17-34_13d2068684ab.py
+-rw-r--r--   0        0        0     1676 2024-05-18 16:03:12.200227 create_fastapi_project-0.2.5/create_fastapi_project/templates/full/backend/app/alembic.ini
+-rw-r--r--   0        0        0        0 2024-05-18 16:03:12.204227 create_fastapi_project-0.2.5/create_fastapi_project/templates/full/backend/app/app/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-18 16:03:12.204227 create_fastapi_project-0.2.5/create_fastapi_project/templates/full/backend/app/app/api/__init__.py
+-rw-r--r--   0        0        0      727 2024-05-18 16:03:12.204227 create_fastapi_project-0.2.5/create_fastapi_project/templates/full/backend/app/app/api/celery_task.py
+-rw-r--r--   0        0        0     3376 2024-05-18 16:03:12.204227 create_fastapi_project-0.2.5/create_fastapi_project/templates/full/backend/app/app/api/deps.py
+-rw-r--r--   0        0        0        0 2024-05-18 16:03:12.204227 create_fastapi_project-0.2.5/create_fastapi_project/templates/full/backend/app/app/api/v1/__init__.py
+-rw-r--r--   0        0        0      971 2024-05-18 16:03:12.204227 create_fastapi_project-0.2.5/create_fastapi_project/templates/full/backend/app/app/api/v1/api.py
+-rw-r--r--   0        0        0        0 2024-05-18 16:03:12.204227 create_fastapi_project-0.2.5/create_fastapi_project/templates/full/backend/app/app/api/v1/endpoints/__init__.py
+-rw-r--r--   0        0        0     2054 2024-05-18 16:03:12.204227 create_fastapi_project-0.2.5/create_fastapi_project/templates/full/backend/app/app/api/v1/endpoints/cache.py
+-rw-r--r--   0        0        0     3122 2024-05-18 16:03:12.204227 create_fastapi_project-0.2.5/create_fastapi_project/templates/full/backend/app/app/api/v1/endpoints/group.py
+-rw-r--r--   0        0        0     4336 2024-05-18 16:03:12.204227 create_fastapi_project-0.2.5/create_fastapi_project/templates/full/backend/app/app/api/v1/endpoints/hero.py
+-rw-r--r--   0        0        0     7902 2024-05-18 16:03:12.204227 create_fastapi_project-0.2.5/create_fastapi_project/templates/full/backend/app/app/api/v1/endpoints/login.py
+-rw-r--r--   0        0        0     3884 2024-05-18 16:03:12.204227 create_fastapi_project-0.2.5/create_fastapi_project/templates/full/backend/app/app/api/v1/endpoints/periodic_tasks.py
+-rw-r--r--   0        0        0     3376 2024-05-18 16:03:12.204227 create_fastapi_project-0.2.5/create_fastapi_project/templates/full/backend/app/app/api/v1/endpoints/report.py
+-rw-r--r--   0        0        0     2515 2024-05-18 16:03:12.204227 create_fastapi_project-0.2.5/create_fastapi_project/templates/full/backend/app/app/api/v1/endpoints/role.py
+-rw-r--r--   0        0        0     3466 2024-05-18 16:03:12.204227 create_fastapi_project-0.2.5/create_fastapi_project/templates/full/backend/app/app/api/v1/endpoints/team.py
+-rw-r--r--   0        0        0    14433 2024-05-18 16:03:12.204227 create_fastapi_project-0.2.5/create_fastapi_project/templates/full/backend/app/app/api/v1/endpoints/user.py
+-rw-r--r--   0        0        0     3622 2024-05-18 16:03:12.204227 create_fastapi_project-0.2.5/create_fastapi_project/templates/full/backend/app/app/api/v1/endpoints/weather.py
+-rw-r--r--   0        0        0        0 2024-05-18 16:03:12.204227 create_fastapi_project-0.2.5/create_fastapi_project/templates/full/backend/app/app/core/__init__.py
+-rw-r--r--   0        0        0     1095 2024-05-18 16:03:12.204227 create_fastapi_project-0.2.5/create_fastapi_project/templates/full/backend/app/app/core/authz.polar
+-rw-r--r--   0        0        0      385 2024-05-18 16:03:12.204227 create_fastapi_project-0.2.5/create_fastapi_project/templates/full/backend/app/app/core/authz.py
+-rw-r--r--   0        0        0      627 2024-05-18 16:03:12.204227 create_fastapi_project-0.2.5/create_fastapi_project/templates/full/backend/app/app/core/celery.py
+-rw-r--r--   0        0        0     4088 2024-05-18 16:03:12.204227 create_fastapi_project-0.2.5/create_fastapi_project/templates/full/backend/app/app/core/config.py
+-rw-r--r--   0        0        0     1676 2024-05-18 16:03:12.204227 create_fastapi_project-0.2.5/create_fastapi_project/templates/full/backend/app/app/core/security.py
+-rw-r--r--   0        0        0      220 2024-05-18 16:03:12.204227 create_fastapi_project-0.2.5/create_fastapi_project/templates/full/backend/app/app/crud/__init__.py
+-rw-r--r--   0        0        0     6856 2024-05-18 16:03:12.204227 create_fastapi_project-0.2.5/create_fastapi_project/templates/full/backend/app/app/crud/base_crud.py
+-rw-r--r--   0        0        0     1474 2024-05-18 16:03:12.204227 create_fastapi_project-0.2.5/create_fastapi_project/templates/full/backend/app/app/crud/group_crud.py
+-rw-r--r--   0        0        0     1347 2024-05-18 16:03:12.204227 create_fastapi_project-0.2.5/create_fastapi_project/templates/full/backend/app/app/crud/hero_crud.py
+-rw-r--r--   0        0        0      302 2024-05-18 16:03:12.204227 create_fastapi_project-0.2.5/create_fastapi_project/templates/full/backend/app/app/crud/image_media_crud.py
+-rw-r--r--   0        0        0      983 2024-05-18 16:03:12.204227 create_fastapi_project-0.2.5/create_fastapi_project/templates/full/backend/app/app/crud/role_crud.py
+-rw-r--r--   0        0        0      600 2024-05-18 16:03:12.204227 create_fastapi_project-0.2.5/create_fastapi_project/templates/full/backend/app/app/crud/team_crud.py
+-rw-r--r--   0        0        0     3981 2024-05-18 16:03:12.204227 create_fastapi_project-0.2.5/create_fastapi_project/templates/full/backend/app/app/crud/user_crud.py
+-rw-r--r--   0        0        0     3752 2024-05-18 16:03:12.204227 create_fastapi_project-0.2.5/create_fastapi_project/templates/full/backend/app/app/crud/user_follow_crud.py
+-rw-r--r--   0        0        0     6148 2024-05-18 16:03:12.204227 create_fastapi_project-0.2.5/create_fastapi_project/templates/full/backend/app/app/db/.DS_Store
+-rw-r--r--   0        0        0        0 2024-05-18 16:03:12.204227 create_fastapi_project-0.2.5/create_fastapi_project/templates/full/backend/app/app/db/__init__.py
+-rw-r--r--   0        0        0     4681 2024-05-18 16:03:12.204227 create_fastapi_project-0.2.5/create_fastapi_project/templates/full/backend/app/app/db/init_db.py
+-rw-r--r--   0        0        0     1247 2024-05-18 16:03:12.204227 create_fastapi_project-0.2.5/create_fastapi_project/templates/full/backend/app/app/db/session.py
+-rw-r--r--   0        0        0      364 2024-05-18 16:03:12.204227 create_fastapi_project-0.2.5/create_fastapi_project/templates/full/backend/app/app/deps/celery_deps.py
+-rw-r--r--   0        0        0      824 2024-05-18 16:03:12.204227 create_fastapi_project-0.2.5/create_fastapi_project/templates/full/backend/app/app/deps/group_deps.py
+-rw-r--r--   0        0        0      790 2024-05-18 16:03:12.204227 create_fastapi_project-0.2.5/create_fastapi_project/templates/full/backend/app/app/deps/role_deps.py
+-rw-r--r--   0        0        0     1299 2024-05-18 16:03:12.204227 create_fastapi_project-0.2.5/create_fastapi_project/templates/full/backend/app/app/deps/user_deps.py
+-rw-r--r--   0        0        0      313 2024-05-18 16:03:12.204227 create_fastapi_project-0.2.5/create_fastapi_project/templates/full/backend/app/app/initial_data.py
+-rw-r--r--   0        0        0     7181 2024-05-18 16:03:12.204227 create_fastapi_project-0.2.5/create_fastapi_project/templates/full/backend/app/app/main.py
+-rw-r--r--   0        0        0      262 2024-05-18 16:03:12.204227 create_fastapi_project-0.2.5/create_fastapi_project/templates/full/backend/app/app/models/__init__.py
+-rw-r--r--   0        0        0      698 2024-05-18 16:03:12.204227 create_fastapi_project-0.2.5/create_fastapi_project/templates/full/backend/app/app/models/base_uuid_model.py
+-rw-r--r--   0        0        0      740 2024-05-18 16:03:12.204227 create_fastapi_project-0.2.5/create_fastapi_project/templates/full/backend/app/app/models/group_model.py
+-rw-r--r--   0        0        0      778 2024-05-18 16:03:12.204227 create_fastapi_project-0.2.5/create_fastapi_project/templates/full/backend/app/app/models/hero_model.py
+-rw-r--r--   0        0        0      571 2024-05-18 16:03:12.204227 create_fastapi_project-0.2.5/create_fastapi_project/templates/full/backend/app/app/models/image_media_model.py
+-rw-r--r--   0        0        0      390 2024-05-18 16:03:12.204227 create_fastapi_project-0.2.5/create_fastapi_project/templates/full/backend/app/app/models/links_model.py
+-rw-r--r--   0        0        0      631 2024-05-18 16:03:12.204227 create_fastapi_project-0.2.5/create_fastapi_project/templates/full/backend/app/app/models/media_model.py
+-rw-r--r--   0        0        0      346 2024-05-18 16:03:12.204227 create_fastapi_project-0.2.5/create_fastapi_project/templates/full/backend/app/app/models/role_model.py
+-rw-r--r--   0        0        0      663 2024-05-18 16:03:12.204227 create_fastapi_project-0.2.5/create_fastapi_project/templates/full/backend/app/app/models/team_model.py
+-rw-r--r--   0        0        0      402 2024-05-18 16:03:12.204227 create_fastapi_project-0.2.5/create_fastapi_project/templates/full/backend/app/app/models/user_follow_model.py
+-rw-r--r--   0        0        0     2049 2024-05-18 16:03:12.204227 create_fastapi_project-0.2.5/create_fastapi_project/templates/full/backend/app/app/models/user_model.py
+-rw-r--r--   0        0        0     1312 2024-05-18 16:03:12.204227 create_fastapi_project-0.2.5/create_fastapi_project/templates/full/backend/app/app/schemas/common_schema.py
+-rw-r--r--   0        0        0      429 2024-05-18 16:03:12.204227 create_fastapi_project-0.2.5/create_fastapi_project/templates/full/backend/app/app/schemas/group_schema.py
+-rw-r--r--   0        0        0      606 2024-05-18 16:03:12.204227 create_fastapi_project-0.2.5/create_fastapi_project/templates/full/backend/app/app/schemas/hero_schema.py
+-rw-r--r--   0        0        0     1022 2024-05-18 16:03:12.204227 create_fastapi_project-0.2.5/create_fastapi_project/templates/full/backend/app/app/schemas/image_media_schema.py
+-rw-r--r--   0        0        0      303 2024-05-18 16:03:12.204227 create_fastapi_project-0.2.5/create_fastapi_project/templates/full/backend/app/app/schemas/media_schema.py
+-rw-r--r--   0        0        0     2666 2024-05-18 16:03:12.204227 create_fastapi_project-0.2.5/create_fastapi_project/templates/full/backend/app/app/schemas/response_schema.py
+-rw-r--r--   0        0        0      382 2024-05-18 16:03:12.204227 create_fastapi_project-0.2.5/create_fastapi_project/templates/full/backend/app/app/schemas/role_schema.py
+-rw-r--r--   0        0        0      463 2024-05-18 16:03:12.204227 create_fastapi_project-0.2.5/create_fastapi_project/templates/full/backend/app/app/schemas/team_schema.py
+-rw-r--r--   0        0        0      305 2024-05-18 16:03:12.204227 create_fastapi_project-0.2.5/create_fastapi_project/templates/full/backend/app/app/schemas/token_schema.py
+-rw-r--r--   0        0        0      518 2024-05-18 16:03:12.204227 create_fastapi_project-0.2.5/create_fastapi_project/templates/full/backend/app/app/schemas/user_follow_schema.py
+-rw-r--r--   0        0        0     1181 2024-05-18 16:03:12.204227 create_fastapi_project-0.2.5/create_fastapi_project/templates/full/backend/app/app/schemas/user_schema.py
+-rw-r--r--   0        0        0        0 2024-05-18 16:03:12.204227 create_fastapi_project-0.2.5/create_fastapi_project/templates/full/backend/app/app/utils/__init__.py
+-rw-r--r--   0        0        0      317 2024-05-18 16:03:12.204227 create_fastapi_project-0.2.5/create_fastapi_project/templates/full/backend/app/app/utils/exceptions/__init__.py
+-rw-r--r--   0        0        0     2477 2024-05-18 16:03:12.204227 create_fastapi_project-0.2.5/create_fastapi_project/templates/full/backend/app/app/utils/exceptions/common_exception.py
+-rw-r--r--   0        0        0      398 2024-05-18 16:03:12.204227 create_fastapi_project-0.2.5/create_fastapi_project/templates/full/backend/app/app/utils/exceptions/user_exceptions.py
+-rw-r--r--   0        0        0     1895 2024-05-18 16:03:12.204227 create_fastapi_project-0.2.5/create_fastapi_project/templates/full/backend/app/app/utils/exceptions/user_follow_exceptions.py
+-rw-r--r--   0        0        0     4018 2024-05-18 16:03:12.204227 create_fastapi_project-0.2.5/create_fastapi_project/templates/full/backend/app/app/utils/fastapi_globals.py
+-rw-r--r--   0        0        0      317 2024-05-18 16:03:12.204227 create_fastapi_project-0.2.5/create_fastapi_project/templates/full/backend/app/app/utils/map_schema.py
+-rw-r--r--   0        0        0     2210 2024-05-18 16:03:12.204227 create_fastapi_project-0.2.5/create_fastapi_project/templates/full/backend/app/app/utils/minio_client.py
+-rw-r--r--   0        0        0      608 2024-05-18 16:03:12.204227 create_fastapi_project-0.2.5/create_fastapi_project/templates/full/backend/app/app/utils/partial.py
+-rw-r--r--   0        0        0      341 2024-05-18 16:03:12.204227 create_fastapi_project-0.2.5/create_fastapi_project/templates/full/backend/app/app/utils/print_model.py
+-rw-r--r--   0        0        0      279 2024-05-18 16:03:12.204227 create_fastapi_project-0.2.5/create_fastapi_project/templates/full/backend/app/app/utils/requestvars.py
+-rw-r--r--   0        0        0      751 2024-05-18 16:03:12.204227 create_fastapi_project-0.2.5/create_fastapi_project/templates/full/backend/app/app/utils/resize_image.py
+-rw-r--r--   0        0        0     1475 2024-05-18 16:03:12.204227 create_fastapi_project-0.2.5/create_fastapi_project/templates/full/backend/app/app/utils/snowflake.py
+-rw-r--r--   0        0        0     1083 2024-05-18 16:03:12.204227 create_fastapi_project-0.2.5/create_fastapi_project/templates/full/backend/app/app/utils/token.py
+-rw-r--r--   0        0        0     4562 2024-05-18 16:03:12.204227 create_fastapi_project-0.2.5/create_fastapi_project/templates/full/backend/app/app/utils/uuid6.py
+-rw-r--r--   0        0        0        0 2024-05-18 16:03:12.204227 create_fastapi_project-0.2.5/create_fastapi_project/templates/full/backend/app/test/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-18 16:03:12.204227 create_fastapi_project-0.2.5/create_fastapi_project/templates/full/backend/app/test/api/__init__.py
+-rw-r--r--   0        0        0     2018 2024-05-18 16:03:12.204227 create_fastapi_project-0.2.5/create_fastapi_project/templates/full/backend/app/test/api/test_login.py
+-rw-r--r--   0        0        0     2271 2024-05-18 16:03:12.204227 create_fastapi_project-0.2.5/create_fastapi_project/templates/full/backend/app/test/api/test_user.py
+-rw-r--r--   0        0        0      653 2024-05-18 16:03:12.204227 create_fastapi_project-0.2.5/create_fastapi_project/templates/full/backend/app/test/test_main.py
+-rw-r--r--   0        0        0      652 2024-05-18 16:03:12.204227 create_fastapi_project-0.2.5/create_fastapi_project/templates/full/backend/sonar-project.properties
+-rw-r--r--   0        0        0      971 2024-05-18 16:03:12.204227 create_fastapi_project-0.2.5/create_fastapi_project/templates/full/caddy/Caddyfile
+-rw-r--r--   0        0        0       65 2024-05-18 16:03:12.204227 create_fastapi_project-0.2.5/create_fastapi_project/templates/full/create-dbs.sql
+-rw-r--r--   0        0        0     3109 2024-05-18 16:03:12.204227 create_fastapi_project-0.2.5/create_fastapi_project/templates/full/docker-compose-dev.yml
+-rw-r--r--   0        0        0      346 2024-05-18 16:03:12.204227 create_fastapi_project-0.2.5/create_fastapi_project/templates/full/docker-compose-sonarqube.yml
+-rw-r--r--   0        0        0     3121 2024-05-18 16:03:12.204227 create_fastapi_project-0.2.5/create_fastapi_project/templates/full/docker-compose-test.yml
+-rw-r--r--   0        0        0     3138 2024-05-18 16:03:12.204227 create_fastapi_project-0.2.5/create_fastapi_project/templates/full/docker-compose.yml
+-rw-r--r--   0        0        0        0 2024-05-18 16:03:12.204227 create_fastapi_project-0.2.5/create_fastapi_project/templates/full/eslintrc.json
+-rw-r--r--   0        0        0      243 2024-05-18 16:03:12.204227 create_fastapi_project-0.2.5/create_fastapi_project/templates/full/pgadmin/servers.json
+-rw-r--r--   0        0        0      895 2024-05-18 16:03:12.204227 create_fastapi_project-0.2.5/create_fastapi_project/templates/full/pgadmin.yml
+-rw-r--r--   0        0        0      263 2024-05-18 16:03:12.208227 create_fastapi_project-0.2.5/create_fastapi_project/templates/langchain_basic/.env.example
+-rw-r--r--   0        0        0     1858 2024-05-18 16:03:12.208227 create_fastapi_project-0.2.5/create_fastapi_project/templates/langchain_basic/.gitignore
+-rw-r--r--   0        0        0     1686 2024-05-18 16:03:12.208227 create_fastapi_project-0.2.5/create_fastapi_project/templates/langchain_basic/Makefile
+-rw-r--r--   0        0        0     6060 2024-05-18 16:03:12.208227 create_fastapi_project-0.2.5/create_fastapi_project/templates/langchain_basic/README.md
+-rw-r--r--   0        0        0      719 2024-05-18 16:03:12.208227 create_fastapi_project-0.2.5/create_fastapi_project/templates/langchain_basic/backend/Dockerfile
+-rw-r--r--   0        0        0        0 2024-05-18 16:03:12.208227 create_fastapi_project-0.2.5/create_fastapi_project/templates/langchain_basic/backend/app/README.md
+-rw-r--r--   0        0        0        0 2024-05-18 16:03:12.208227 create_fastapi_project-0.2.5/create_fastapi_project/templates/langchain_basic/backend/app/app/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-18 16:03:12.208227 create_fastapi_project-0.2.5/create_fastapi_project/templates/langchain_basic/backend/app/app/api/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-18 16:03:12.208227 create_fastapi_project-0.2.5/create_fastapi_project/templates/langchain_basic/backend/app/app/api/v1/__init__.py
+-rw-r--r--   0        0        0      173 2024-05-18 16:03:12.208227 create_fastapi_project-0.2.5/create_fastapi_project/templates/langchain_basic/backend/app/app/api/v1/api.py
+-rw-r--r--   0        0        0        0 2024-05-18 16:03:12.208227 create_fastapi_project-0.2.5/create_fastapi_project/templates/langchain_basic/backend/app/app/api/v1/endpoints/__init__.py
+-rw-r--r--   0        0        0     4890 2024-05-18 16:03:12.208227 create_fastapi_project-0.2.5/create_fastapi_project/templates/langchain_basic/backend/app/app/api/v1/endpoints/chat.py
+-rw-r--r--   0        0        0        0 2024-05-18 16:03:12.208227 create_fastapi_project-0.2.5/create_fastapi_project/templates/langchain_basic/backend/app/app/core/__init__.py
+-rw-r--r--   0        0        0     1024 2024-05-18 16:03:12.208227 create_fastapi_project-0.2.5/create_fastapi_project/templates/langchain_basic/backend/app/app/core/config.py
+-rw-r--r--   0        0        0     1478 2024-05-18 16:03:12.208227 create_fastapi_project-0.2.5/create_fastapi_project/templates/langchain_basic/backend/app/app/main.py
+-rw-r--r--   0        0        0      144 2024-05-18 16:03:12.208227 create_fastapi_project-0.2.5/create_fastapi_project/templates/langchain_basic/backend/app/app/schemas/adaptive_cards_schema.py
+-rw-r--r--   0        0        0      926 2024-05-18 16:03:12.208227 create_fastapi_project-0.2.5/create_fastapi_project/templates/langchain_basic/backend/app/app/schemas/message_schema.py
+-rw-r--r--   0        0        0     2701 2024-05-18 16:03:12.208227 create_fastapi_project-0.2.5/create_fastapi_project/templates/langchain_basic/backend/app/app/schemas/response_schema.py
+-rw-r--r--   0        0        0      702 2024-05-18 16:03:12.208227 create_fastapi_project-0.2.5/create_fastapi_project/templates/langchain_basic/backend/app/app/templates/chat.py
+-rw-r--r--   0        0        0        0 2024-05-18 16:03:12.208227 create_fastapi_project-0.2.5/create_fastapi_project/templates/langchain_basic/backend/app/app/utils/__init__.py
+-rw-r--r--   0        0        0     4959 2024-05-18 16:03:12.208227 create_fastapi_project-0.2.5/create_fastapi_project/templates/langchain_basic/backend/app/app/utils/adaptive_cards/cards.py
+-rw-r--r--   0        0        0    10084 2024-05-18 16:03:12.208227 create_fastapi_project-0.2.5/create_fastapi_project/templates/langchain_basic/backend/app/app/utils/callback.py
+-rw-r--r--   0        0        0     1179 2024-05-18 16:03:12.208227 create_fastapi_project-0.2.5/create_fastapi_project/templates/langchain_basic/backend/app/app/utils/chains.py
+-rw-r--r--   0        0        0     1510 2024-05-18 16:03:12.208227 create_fastapi_project-0.2.5/create_fastapi_project/templates/langchain_basic/backend/app/app/utils/partial.py
+-rw-r--r--   0        0        0     1502 2024-05-18 16:03:12.208227 create_fastapi_project-0.2.5/create_fastapi_project/templates/langchain_basic/backend/app/app/utils/prompt_zero.py
+-rw-r--r--   0        0        0     6275 2024-05-18 16:03:12.208227 create_fastapi_project-0.2.5/create_fastapi_project/templates/langchain_basic/backend/app/app/utils/tools.py
+-rw-r--r--   0        0        0     4562 2024-05-18 16:03:12.208227 create_fastapi_project-0.2.5/create_fastapi_project/templates/langchain_basic/backend/app/app/utils/uuid6.py
+-rw-r--r--   0        0        0      270 2024-05-18 16:03:12.208227 create_fastapi_project-0.2.5/create_fastapi_project/templates/langchain_basic/caddy/Caddyfile
+-rw-r--r--   0        0        0      983 2024-05-18 16:03:12.208227 create_fastapi_project-0.2.5/create_fastapi_project/templates/langchain_basic/docker-compose-dev.yml
+-rw-r--r--   0        0        0     1066 2024-05-18 16:03:12.208227 create_fastapi_project-0.2.5/create_fastapi_project/templates/langchain_basic/docker-compose.yml
+-rw-r--r--   0        0        0      701 2024-05-18 16:03:12.208227 create_fastapi_project-0.2.5/create_fastapi_project/templates/langchain_basic/frontend/Dockerfile
+-rw-r--r--   0        0        0     2345 2024-05-18 16:03:12.208227 create_fastapi_project-0.2.5/create_fastapi_project/templates/langchain_basic/frontend/app/main.py
+-rw-r--r--   0        0        0      307 2024-05-18 16:03:12.208227 create_fastapi_project-0.2.5/create_fastapi_project/templates/langchain_basic/streamlit.yml
+-rw-r--r--   0        0        0     1457 2024-05-18 16:03:20.196207 create_fastapi_project-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0    11882 1970-01-01 00:00:00.000000 create_fastapi_project-0.2.5/PKG-INFO
```

### Comparing `create_fastapi_project-0.2.4/LICENSE` & `create_fastapi_project-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `create_fastapi_project-0.2.4/README.md` & `create_fastapi_project-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `create_fastapi_project-0.2.4/create_fastapi_project/.DS_Store` & `create_fastapi_project-0.2.5/create_fastapi_project/.DS_Store`

 * *Files identical despite different names*

### Comparing `create_fastapi_project-0.2.4/create_fastapi_project/create_app.py` & `create_fastapi_project-0.2.5/create_fastapi_project/create_app.py`

 * *Files identical despite different names*

### Comparing `create_fastapi_project-0.2.4/create_fastapi_project/helpers/git.py` & `create_fastapi_project-0.2.5/create_fastapi_project/helpers/git.py`

 * *Files identical despite different names*

### Comparing `create_fastapi_project-0.2.4/create_fastapi_project/helpers/install.py` & `create_fastapi_project-0.2.5/create_fastapi_project/helpers/install.py`

 * *Files identical despite different names*

### Comparing `create_fastapi_project-0.2.4/create_fastapi_project/main.py` & `create_fastapi_project-0.2.5/create_fastapi_project/main.py`

 * *Files identical despite different names*

### Comparing `create_fastapi_project-0.2.4/create_fastapi_project/templates/__init__.py` & `create_fastapi_project-0.2.5/create_fastapi_project/templates/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -43,74 +43,72 @@
         poetry_frontend_path = os.path.join(root, "frontend", "app")
     
     has_pyproject = add_configuration_to_pyproject(poetry_path)
 
     if has_pyproject:
         dependencies = [
             "fastapi[all]",
-            "fastapi-pagination[sqlalchemy]@^0.12.7",
-            "asyncer@^0.0.2",
-            "httpx@^0.24.1",
+            "fastapi-pagination[sqlalchemy]",
+            "asyncer",
+            "httpx",
         ]
         dev_dependencies = [
-            "pytest@^7.4.0",
-            "mypy@^1.5.0",
-            "ruff@^0.0.284",
-            "black@^23.7.0",
+            "pytest",
+            "mypy",
+            "ruff",
+            "black",
         ]
         if template == ITemplate.langchain_basic:
             langchain_dependencies = [
-                "langchain@^0.0.265",
-                "openai@^0.27.8",
-                "adaptive-cards-py@^0.0.7",
-                "google-search-results@^2.4.2",
+                "langchain",
+                "openai",
+                "adaptive-cards-py",
+                "google-search-results",
             ]
             frontend_dependencies = [
                 "streamlit",
                 "websockets",
             ]
-            dependencies[0] = "fastapi[all]@^0.99.1"
             dependencies.extend(langchain_dependencies)
         if template == ITemplate.full:
             full_dependencies = [
-                "alembic@^1.10.2",
-                "asyncpg@^0.27.0",
-                "sqlmodel@^0.0.8",
-                "python-jose@^3.3.0",
-                "cryptography@^38.0.3",
-                "passlib@^1.7.4",
-                "SQLAlchemy-Utils@^0.38.3",
-                "SQLAlchemy@^1.4.40",
-                "minio@^7.1.13",
-                "Pillow@^9.4.0",
-                "watchfiles@^0.18.1",
-                "asyncer@^0.0.2",
-                "httpx@^0.23.1",
-                "pandas@^1.5.3",
-                "openpyxl@^3.0.10",
-                "redis@^4.5.1",
-                "fastapi-async-sqlalchemy@^0.3.12",
-                "oso@^0.26.4",
-                "celery@^5.2.7",
-                "transformers@^4.28.1",
-                "requests@^2.29.0",
-                "wheel@^0.40.0",
-                "setuptools@^67.7.2",
-                "langchain@^0.0.262",
-                "openai@^0.27.5",
-                "celery-sqlalchemy-scheduler@^0.3.0",
-                "psycopg2-binary@^2.9.5",
-                "fastapi-limiter@^0.1.5 ",
-                "fastapi-pagination[sqlalchemy]@^0.11.4 ",
-                "fastapi-cache2[redis]@^0.2.1 ",
+                "alembic",
+                "asyncpg",
+                "sqlmodel",
+                "python-jose",
+                "cryptography",
+                "passlib",
+                "SQLAlchemy-Utils",
+                "SQLAlchemy",
+                "minio",
+                "Pillow",
+                "watchfiles",
+                "asyncer",
+                "httpx",
+                "pandas",
+                "openpyxl",
+                "redis",
+                "fastapi-async-sqlalchemy",
+                "oso",
+                "celery",
+                "transformers",
+                "requests",
+                "wheel",
+                "setuptools",
+                "langchain",
+                "openai",
+                "celery-sqlalchemy-scheduler",
+                "psycopg2-binary",
+                "fastapi-limiter",
+                "fastapi-pagination[sqlalchemy]",
+                "fastapi-cache2[redis]",
             ]
             full_dev_dependencies = [
-                "pytest-asyncio@^0.21.1",
+                "pytest-asyncio",
             ]
-            dependencies[0] = "fastapi[all]@^0.95.2"
             dependencies.extend(full_dependencies)
             dev_dependencies.extend(full_dev_dependencies)
 
         print("- Installing main packages. This might take a couple of minutes.")
         print("poetry_path", poetry_path)
         print("template", template)
         install_dependencies(poetry_path, dependencies)
```

### Comparing `create_fastapi_project-0.2.4/create_fastapi_project/templates/basic/.gitignore` & `create_fastapi_project-0.2.5/create_fastapi_project/templates/basic/.gitignore`

 * *Files identical despite different names*

### Comparing `create_fastapi_project-0.2.4/create_fastapi_project/templates/basic/Makefile` & `create_fastapi_project-0.2.5/create_fastapi_project/templates/basic/Makefile`

 * *Files identical despite different names*

### Comparing `create_fastapi_project-0.2.4/create_fastapi_project/templates/basic/README.md` & `create_fastapi_project-0.2.5/create_fastapi_project/templates/basic/README.md`

 * *Files identical despite different names*

### Comparing `create_fastapi_project-0.2.4/create_fastapi_project/templates/basic/backend/Dockerfile` & `create_fastapi_project-0.2.5/create_fastapi_project/templates/basic/backend/Dockerfile`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,20 @@
-FROM tiangolo/uvicorn-gunicorn-fastapi:python3.11
+FROM tiangolo/uvicorn-gunicorn-fastapi:python3.11-slim
 ENV PYTHONUNBUFFERED=1
+ENV PIP_DEFAULT_TIMEOUT=100
 WORKDIR /code
 # Install Poetry
 RUN apt clean && apt update && apt install curl -y
 RUN curl -sSL https://install.python-poetry.org | POETRY_HOME=/opt/poetry python && \
     cd /usr/local/bin && \
     ln -s /opt/poetry/bin/poetry && \
     poetry config virtualenvs.create false
 
 # Copy poetry.lock* in case it doesn't exist in the repo
 COPY app/pyproject.toml app/poetry.lock* /code/
 
 # Allow installing dev dependencies to run tests
 ARG INSTALL_DEV=false
-RUN bash -c "if [ $INSTALL_DEV == 'true' ] ; then poetry install --no-root ; else poetry install --no-root --no-dev ; fi"
+RUN bash -c "if [ $INSTALL_DEV == 'true' ] ; then poetry install --no-root ; else poetry install --no-root --only main ; fi"
 
 ENV PYTHONPATH=/code
 EXPOSE 8000
```

### Comparing `create_fastapi_project-0.2.4/create_fastapi_project/templates/basic/backend/app/app/api/v1/endpoints/weather.py` & `create_fastapi_project-0.2.5/create_fastapi_project/templates/basic/backend/app/app/api/v1/endpoints/weather.py`

 * *Files identical despite different names*

### Comparing `create_fastapi_project-0.2.4/create_fastapi_project/templates/basic/backend/app/app/core/config.py` & `create_fastapi_project-0.2.5/create_fastapi_project/templates/basic/backend/app/app/core/config.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 
 class ModeEnum(str, Enum):
     development = "development"
     production = "production"
     testing = "testing"
 
 
-class Settings(BaseSettings):
+class Settings(BaseSettings, extra='ignore'):
     PROJECT_NAME: str = "app"
     BACKEND_CORS_ORIGINS: list[str] | list[AnyHttpUrl]
     MODE: ModeEnum = ModeEnum.development
     API_VERSION: str = "v1"
     API_V1_STR: str = f"/api/{API_VERSION}"
     WHEATER_URL: str = "https://wttr.in"
 
     
     class Config:
         case_sensitive = True
-        env_file = os.path.expanduser("~/.env")
+        env_file = os.path.expanduser("../../.env")
 
 
 settings = Settings()
```

### Comparing `create_fastapi_project-0.2.4/create_fastapi_project/templates/basic/backend/app/app/main.py` & `create_fastapi_project-0.2.5/create_fastapi_project/templates/basic/backend/app/app/main.py`

 * *Files identical despite different names*

### Comparing `create_fastapi_project-0.2.4/create_fastapi_project/templates/basic/backend/app/app/schemas/response_schema.py` & `create_fastapi_project-0.2.5/create_fastapi_project/templates/basic/backend/app/app/schemas/response_schema.py`

 * *Files identical despite different names*

### Comparing `create_fastapi_project-0.2.4/create_fastapi_project/templates/basic/backend/app/app/utils/exceptions/common_exception.py` & `create_fastapi_project-0.2.5/create_fastapi_project/templates/basic/backend/app/app/utils/exceptions/common_exception.py`

 * *Files identical despite different names*

### Comparing `create_fastapi_project-0.2.4/create_fastapi_project/templates/basic/backend/app/app/utils/exceptions/user_follow_exceptions.py` & `create_fastapi_project-0.2.5/create_fastapi_project/templates/basic/backend/app/app/utils/exceptions/user_follow_exceptions.py`

 * *Files identical despite different names*

### Comparing `create_fastapi_project-0.2.4/create_fastapi_project/templates/basic/backend/app/app/utils/partial.py` & `create_fastapi_project-0.2.5/create_fastapi_project/templates/basic/backend/app/app/utils/partial.py`

 * *Files identical despite different names*

### Comparing `create_fastapi_project-0.2.4/create_fastapi_project/templates/basic/backend/app/app/utils/uuid6.py` & `create_fastapi_project-0.2.5/create_fastapi_project/templates/basic/backend/app/app/utils/uuid6.py`

 * *Files identical despite different names*

### Comparing `create_fastapi_project-0.2.4/create_fastapi_project/templates/basic/docker-compose-dev.yml` & `create_fastapi_project-0.2.5/create_fastapi_project/templates/basic/docker-compose-dev.yml`

 * *Files identical despite different names*

### Comparing `create_fastapi_project-0.2.4/create_fastapi_project/templates/basic/docker-compose.yml` & `create_fastapi_project-0.2.5/create_fastapi_project/templates/basic/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `create_fastapi_project-0.2.4/create_fastapi_project/templates/full/.env.example` & `create_fastapi_project-0.2.5/create_fastapi_project/templates/full/.env.example`

 * *Files identical despite different names*

### Comparing `create_fastapi_project-0.2.4/create_fastapi_project/templates/full/.gitignore` & `create_fastapi_project-0.2.5/create_fastapi_project/templates/full/.gitignore`

 * *Files identical despite different names*

### Comparing `create_fastapi_project-0.2.4/create_fastapi_project/templates/full/LICENSE` & `create_fastapi_project-0.2.5/create_fastapi_project/templates/full/LICENSE`

 * *Files identical despite different names*

### Comparing `create_fastapi_project-0.2.4/create_fastapi_project/templates/full/Makefile` & `create_fastapi_project-0.2.5/create_fastapi_project/templates/full/Makefile`

 * *Files identical despite different names*

### Comparing `create_fastapi_project-0.2.4/create_fastapi_project/templates/full/README.md` & `create_fastapi_project-0.2.5/create_fastapi_project/templates/full/README.md`

 * *Files identical despite different names*

### Comparing `create_fastapi_project-0.2.4/create_fastapi_project/templates/full/backend/Dockerfile` & `create_fastapi_project-0.2.5/create_fastapi_project/templates/langchain_basic/frontend/Dockerfile`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,21 @@
-FROM tiangolo/uvicorn-gunicorn-fastapi:python3.10-slim-2022-11-25
+FROM python:3.10-slim
 ENV PYTHONUNBUFFERED=1
 WORKDIR /code
 # Install Poetry
 RUN apt clean && apt update && apt install curl -y
 RUN curl -sSL https://install.python-poetry.org | POETRY_HOME=/opt/poetry python && \
     cd /usr/local/bin && \
     ln -s /opt/poetry/bin/poetry && \
     poetry config virtualenvs.create false
 
 # Copy poetry.lock* in case it doesn't exist in the repo
 COPY app/pyproject.toml app/poetry.lock* /code/
 
-# Allow installing dev dependencies to run tests
+ENV PYTHONPATH=/code
+EXPOSE 8501
+
 ARG INSTALL_DEV=false
 RUN bash -c "if [ $INSTALL_DEV == 'true' ] ; then poetry install --no-root ; else poetry install --no-root --no-dev ; fi"
 
-ENV PYTHONPATH=/code
-EXPOSE 8000
+
+ENTRYPOINT ["streamlit", "run", "main.py", "--server.port=8501", "--server.address=0.0.0.0"]
```

### Comparing `create_fastapi_project-0.2.4/create_fastapi_project/templates/full/backend/app/alembic/env.py` & `create_fastapi_project-0.2.5/create_fastapi_project/templates/full/backend/app/alembic/env.py`

 * *Files identical despite different names*

### Comparing `create_fastapi_project-0.2.4/create_fastapi_project/templates/full/backend/app/alembic/script.py.mako` & `create_fastapi_project-0.2.5/create_fastapi_project/templates/full/backend/app/alembic/script.py.mako`

 * *Files identical despite different names*

### Comparing `create_fastapi_project-0.2.4/create_fastapi_project/templates/full/backend/app/alembic/versions/2022-09-25-19-46_60d49bf413b8.py` & `create_fastapi_project-0.2.5/create_fastapi_project/templates/full/backend/app/alembic/versions/2022-09-25-19-46_60d49bf413b8.py`

 * *Files identical despite different names*

### Comparing `create_fastapi_project-0.2.4/create_fastapi_project/templates/full/backend/app/alembic/versions/2022-10-03-18-32_3223652d21bd.py` & `create_fastapi_project-0.2.5/create_fastapi_project/templates/full/backend/app/alembic/versions/2022-10-03-18-32_3223652d21bd.py`

 * *Files identical despite different names*

### Comparing `create_fastapi_project-0.2.4/create_fastapi_project/templates/full/backend/app/alembic/versions/2022-10-23-04-07_cc36a024e8ed.py` & `create_fastapi_project-0.2.5/create_fastapi_project/templates/full/backend/app/alembic/versions/2022-10-23-04-07_cc36a024e8ed.py`

 * *Files identical despite different names*

### Comparing `create_fastapi_project-0.2.4/create_fastapi_project/templates/full/backend/app/alembic/versions/2022-11-03-14-16_3293815eb23c.py` & `create_fastapi_project-0.2.5/create_fastapi_project/templates/full/backend/app/alembic/versions/2022-11-03-14-16_3293815eb23c.py`

 * *Files identical despite different names*

### Comparing `create_fastapi_project-0.2.4/create_fastapi_project/templates/full/backend/app/alembic/versions/2023-03-04-23-15_5591a516fc47.py` & `create_fastapi_project-0.2.5/create_fastapi_project/templates/full/backend/app/alembic/versions/2023-03-04-23-15_5591a516fc47.py`

 * *Files identical despite different names*

### Comparing `create_fastapi_project-0.2.4/create_fastapi_project/templates/full/backend/app/alembic/versions/2023-03-17-17-34_13d2068684ab.py` & `create_fastapi_project-0.2.5/create_fastapi_project/templates/full/backend/app/alembic/versions/2023-03-17-17-34_13d2068684ab.py`

 * *Files identical despite different names*

### Comparing `create_fastapi_project-0.2.4/create_fastapi_project/templates/full/backend/app/alembic.ini` & `create_fastapi_project-0.2.5/create_fastapi_project/templates/full/backend/app/alembic.ini`

 * *Files identical despite different names*

### Comparing `create_fastapi_project-0.2.4/create_fastapi_project/templates/full/backend/app/app/api/celery_task.py` & `create_fastapi_project-0.2.5/create_fastapi_project/templates/full/backend/app/app/api/celery_task.py`

 * *Files identical despite different names*

### Comparing `create_fastapi_project-0.2.4/create_fastapi_project/templates/full/backend/app/app/api/deps.py` & `create_fastapi_project-0.2.5/create_fastapi_project/templates/full/backend/app/app/api/deps.py`

 * *Files identical despite different names*

### Comparing `create_fastapi_project-0.2.4/create_fastapi_project/templates/full/backend/app/app/api/v1/api.py` & `create_fastapi_project-0.2.5/create_fastapi_project/templates/full/backend/app/app/api/v1/api.py`

 * *Files identical despite different names*

### Comparing `create_fastapi_project-0.2.4/create_fastapi_project/templates/full/backend/app/app/api/v1/endpoints/cache.py` & `create_fastapi_project-0.2.5/create_fastapi_project/templates/full/backend/app/app/api/v1/endpoints/cache.py`

 * *Files identical despite different names*

### Comparing `create_fastapi_project-0.2.4/create_fastapi_project/templates/full/backend/app/app/api/v1/endpoints/group.py` & `create_fastapi_project-0.2.5/create_fastapi_project/templates/full/backend/app/app/api/v1/endpoints/group.py`

 * *Files identical despite different names*

### Comparing `create_fastapi_project-0.2.4/create_fastapi_project/templates/full/backend/app/app/api/v1/endpoints/hero.py` & `create_fastapi_project-0.2.5/create_fastapi_project/templates/full/backend/app/app/api/v1/endpoints/hero.py`

 * *Files identical despite different names*

### Comparing `create_fastapi_project-0.2.4/create_fastapi_project/templates/full/backend/app/app/api/v1/endpoints/login.py` & `create_fastapi_project-0.2.5/create_fastapi_project/templates/full/backend/app/app/api/v1/endpoints/login.py`

 * *Files identical despite different names*

### Comparing `create_fastapi_project-0.2.4/create_fastapi_project/templates/full/backend/app/app/api/v1/endpoints/periodic_tasks.py` & `create_fastapi_project-0.2.5/create_fastapi_project/templates/full/backend/app/app/api/v1/endpoints/periodic_tasks.py`

 * *Files identical despite different names*

### Comparing `create_fastapi_project-0.2.4/create_fastapi_project/templates/full/backend/app/app/api/v1/endpoints/report.py` & `create_fastapi_project-0.2.5/create_fastapi_project/templates/full/backend/app/app/api/v1/endpoints/report.py`

 * *Files identical despite different names*

### Comparing `create_fastapi_project-0.2.4/create_fastapi_project/templates/full/backend/app/app/api/v1/endpoints/role.py` & `create_fastapi_project-0.2.5/create_fastapi_project/templates/full/backend/app/app/api/v1/endpoints/role.py`

 * *Files identical despite different names*

### Comparing `create_fastapi_project-0.2.4/create_fastapi_project/templates/full/backend/app/app/api/v1/endpoints/team.py` & `create_fastapi_project-0.2.5/create_fastapi_project/templates/full/backend/app/app/api/v1/endpoints/team.py`

 * *Files identical despite different names*

### Comparing `create_fastapi_project-0.2.4/create_fastapi_project/templates/full/backend/app/app/api/v1/endpoints/user.py` & `create_fastapi_project-0.2.5/create_fastapi_project/templates/full/backend/app/app/api/v1/endpoints/user.py`

 * *Files identical despite different names*

### Comparing `create_fastapi_project-0.2.4/create_fastapi_project/templates/full/backend/app/app/api/v1/endpoints/weather.py` & `create_fastapi_project-0.2.5/create_fastapi_project/templates/full/backend/app/app/api/v1/endpoints/weather.py`

 * *Files identical despite different names*

### Comparing `create_fastapi_project-0.2.4/create_fastapi_project/templates/full/backend/app/app/core/authz.polar` & `create_fastapi_project-0.2.5/create_fastapi_project/templates/full/backend/app/app/core/authz.polar`

 * *Files identical despite different names*

### Comparing `create_fastapi_project-0.2.4/create_fastapi_project/templates/full/backend/app/app/core/celery.py` & `create_fastapi_project-0.2.5/create_fastapi_project/templates/full/backend/app/app/core/celery.py`

 * *Files identical despite different names*

### Comparing `create_fastapi_project-0.2.4/create_fastapi_project/templates/full/backend/app/app/core/config.py` & `create_fastapi_project-0.2.5/create_fastapi_project/templates/full/backend/app/app/core/config.py`

 * *Files identical despite different names*

### Comparing `create_fastapi_project-0.2.4/create_fastapi_project/templates/full/backend/app/app/core/security.py` & `create_fastapi_project-0.2.5/create_fastapi_project/templates/full/backend/app/app/core/security.py`

 * *Files identical despite different names*

### Comparing `create_fastapi_project-0.2.4/create_fastapi_project/templates/full/backend/app/app/crud/base_crud.py` & `create_fastapi_project-0.2.5/create_fastapi_project/templates/full/backend/app/app/crud/base_crud.py`

 * *Files identical despite different names*

### Comparing `create_fastapi_project-0.2.4/create_fastapi_project/templates/full/backend/app/app/crud/group_crud.py` & `create_fastapi_project-0.2.5/create_fastapi_project/templates/full/backend/app/app/crud/group_crud.py`

 * *Files identical despite different names*

### Comparing `create_fastapi_project-0.2.4/create_fastapi_project/templates/full/backend/app/app/crud/hero_crud.py` & `create_fastapi_project-0.2.5/create_fastapi_project/templates/full/backend/app/app/crud/hero_crud.py`

 * *Files identical despite different names*

### Comparing `create_fastapi_project-0.2.4/create_fastapi_project/templates/full/backend/app/app/crud/role_crud.py` & `create_fastapi_project-0.2.5/create_fastapi_project/templates/full/backend/app/app/crud/role_crud.py`

 * *Files identical despite different names*

### Comparing `create_fastapi_project-0.2.4/create_fastapi_project/templates/full/backend/app/app/crud/team_crud.py` & `create_fastapi_project-0.2.5/create_fastapi_project/templates/full/backend/app/app/crud/team_crud.py`

 * *Files identical despite different names*

### Comparing `create_fastapi_project-0.2.4/create_fastapi_project/templates/full/backend/app/app/crud/user_crud.py` & `create_fastapi_project-0.2.5/create_fastapi_project/templates/full/backend/app/app/crud/user_crud.py`

 * *Files identical despite different names*

### Comparing `create_fastapi_project-0.2.4/create_fastapi_project/templates/full/backend/app/app/crud/user_follow_crud.py` & `create_fastapi_project-0.2.5/create_fastapi_project/templates/full/backend/app/app/crud/user_follow_crud.py`

 * *Files identical despite different names*

### Comparing `create_fastapi_project-0.2.4/create_fastapi_project/templates/full/backend/app/app/db/.DS_Store` & `create_fastapi_project-0.2.5/create_fastapi_project/templates/full/backend/app/app/db/.DS_Store`

 * *Files identical despite different names*

### Comparing `create_fastapi_project-0.2.4/create_fastapi_project/templates/full/backend/app/app/db/init_db.py` & `create_fastapi_project-0.2.5/create_fastapi_project/templates/full/backend/app/app/db/init_db.py`

 * *Files identical despite different names*

### Comparing `create_fastapi_project-0.2.4/create_fastapi_project/templates/full/backend/app/app/db/session.py` & `create_fastapi_project-0.2.5/create_fastapi_project/templates/full/backend/app/app/db/session.py`

 * *Files identical despite different names*

### Comparing `create_fastapi_project-0.2.4/create_fastapi_project/templates/full/backend/app/app/deps/group_deps.py` & `create_fastapi_project-0.2.5/create_fastapi_project/templates/full/backend/app/app/deps/group_deps.py`

 * *Files identical despite different names*

### Comparing `create_fastapi_project-0.2.4/create_fastapi_project/templates/full/backend/app/app/deps/role_deps.py` & `create_fastapi_project-0.2.5/create_fastapi_project/templates/full/backend/app/app/deps/role_deps.py`

 * *Files identical despite different names*

### Comparing `create_fastapi_project-0.2.4/create_fastapi_project/templates/full/backend/app/app/deps/user_deps.py` & `create_fastapi_project-0.2.5/create_fastapi_project/templates/full/backend/app/app/deps/user_deps.py`

 * *Files identical despite different names*

### Comparing `create_fastapi_project-0.2.4/create_fastapi_project/templates/full/backend/app/app/main.py` & `create_fastapi_project-0.2.5/create_fastapi_project/templates/full/backend/app/app/main.py`

 * *Files identical despite different names*

### Comparing `create_fastapi_project-0.2.4/create_fastapi_project/templates/full/backend/app/app/models/base_uuid_model.py` & `create_fastapi_project-0.2.5/create_fastapi_project/templates/full/backend/app/app/models/base_uuid_model.py`

 * *Files identical despite different names*

### Comparing `create_fastapi_project-0.2.4/create_fastapi_project/templates/full/backend/app/app/models/group_model.py` & `create_fastapi_project-0.2.5/create_fastapi_project/templates/full/backend/app/app/models/group_model.py`

 * *Files identical despite different names*

### Comparing `create_fastapi_project-0.2.4/create_fastapi_project/templates/full/backend/app/app/models/hero_model.py` & `create_fastapi_project-0.2.5/create_fastapi_project/templates/full/backend/app/app/models/hero_model.py`

 * *Files identical despite different names*

### Comparing `create_fastapi_project-0.2.4/create_fastapi_project/templates/full/backend/app/app/models/image_media_model.py` & `create_fastapi_project-0.2.5/create_fastapi_project/templates/full/backend/app/app/models/image_media_model.py`

 * *Files identical despite different names*

### Comparing `create_fastapi_project-0.2.4/create_fastapi_project/templates/full/backend/app/app/models/media_model.py` & `create_fastapi_project-0.2.5/create_fastapi_project/templates/full/backend/app/app/models/media_model.py`

 * *Files identical despite different names*

### Comparing `create_fastapi_project-0.2.4/create_fastapi_project/templates/full/backend/app/app/models/team_model.py` & `create_fastapi_project-0.2.5/create_fastapi_project/templates/full/backend/app/app/models/team_model.py`

 * *Files identical despite different names*

### Comparing `create_fastapi_project-0.2.4/create_fastapi_project/templates/full/backend/app/app/models/user_model.py` & `create_fastapi_project-0.2.5/create_fastapi_project/templates/full/backend/app/app/models/user_model.py`

 * *Files identical despite different names*

### Comparing `create_fastapi_project-0.2.4/create_fastapi_project/templates/full/backend/app/app/schemas/common_schema.py` & `create_fastapi_project-0.2.5/create_fastapi_project/templates/full/backend/app/app/schemas/common_schema.py`

 * *Files identical despite different names*

### Comparing `create_fastapi_project-0.2.4/create_fastapi_project/templates/full/backend/app/app/schemas/hero_schema.py` & `create_fastapi_project-0.2.5/create_fastapi_project/templates/full/backend/app/app/schemas/hero_schema.py`

 * *Files identical despite different names*

### Comparing `create_fastapi_project-0.2.4/create_fastapi_project/templates/full/backend/app/app/schemas/image_media_schema.py` & `create_fastapi_project-0.2.5/create_fastapi_project/templates/full/backend/app/app/schemas/image_media_schema.py`

 * *Files identical despite different names*

### Comparing `create_fastapi_project-0.2.4/create_fastapi_project/templates/full/backend/app/app/schemas/response_schema.py` & `create_fastapi_project-0.2.5/create_fastapi_project/templates/full/backend/app/app/schemas/response_schema.py`

 * *Files identical despite different names*

### Comparing `create_fastapi_project-0.2.4/create_fastapi_project/templates/full/backend/app/app/schemas/user_follow_schema.py` & `create_fastapi_project-0.2.5/create_fastapi_project/templates/full/backend/app/app/schemas/user_follow_schema.py`

 * *Files identical despite different names*

### Comparing `create_fastapi_project-0.2.4/create_fastapi_project/templates/full/backend/app/app/schemas/user_schema.py` & `create_fastapi_project-0.2.5/create_fastapi_project/templates/full/backend/app/app/schemas/user_schema.py`

 * *Files identical despite different names*

### Comparing `create_fastapi_project-0.2.4/create_fastapi_project/templates/full/backend/app/app/utils/exceptions/common_exception.py` & `create_fastapi_project-0.2.5/create_fastapi_project/templates/full/backend/app/app/utils/exceptions/common_exception.py`

 * *Files identical despite different names*

### Comparing `create_fastapi_project-0.2.4/create_fastapi_project/templates/full/backend/app/app/utils/exceptions/user_follow_exceptions.py` & `create_fastapi_project-0.2.5/create_fastapi_project/templates/full/backend/app/app/utils/exceptions/user_follow_exceptions.py`

 * *Files identical despite different names*

### Comparing `create_fastapi_project-0.2.4/create_fastapi_project/templates/full/backend/app/app/utils/fastapi_globals.py` & `create_fastapi_project-0.2.5/create_fastapi_project/templates/full/backend/app/app/utils/fastapi_globals.py`

 * *Files identical despite different names*

### Comparing `create_fastapi_project-0.2.4/create_fastapi_project/templates/full/backend/app/app/utils/minio_client.py` & `create_fastapi_project-0.2.5/create_fastapi_project/templates/full/backend/app/app/utils/minio_client.py`

 * *Files identical despite different names*

### Comparing `create_fastapi_project-0.2.4/create_fastapi_project/templates/full/backend/app/app/utils/partial.py` & `create_fastapi_project-0.2.5/create_fastapi_project/templates/full/backend/app/app/utils/partial.py`

 * *Files identical despite different names*

### Comparing `create_fastapi_project-0.2.4/create_fastapi_project/templates/full/backend/app/app/utils/resize_image.py` & `create_fastapi_project-0.2.5/create_fastapi_project/templates/full/backend/app/app/utils/resize_image.py`

 * *Files identical despite different names*

### Comparing `create_fastapi_project-0.2.4/create_fastapi_project/templates/full/backend/app/app/utils/snowflake.py` & `create_fastapi_project-0.2.5/create_fastapi_project/templates/full/backend/app/app/utils/snowflake.py`

 * *Files identical despite different names*

### Comparing `create_fastapi_project-0.2.4/create_fastapi_project/templates/full/backend/app/app/utils/token.py` & `create_fastapi_project-0.2.5/create_fastapi_project/templates/full/backend/app/app/utils/token.py`

 * *Files identical despite different names*

### Comparing `create_fastapi_project-0.2.4/create_fastapi_project/templates/full/backend/app/app/utils/uuid6.py` & `create_fastapi_project-0.2.5/create_fastapi_project/templates/full/backend/app/app/utils/uuid6.py`

 * *Files identical despite different names*

### Comparing `create_fastapi_project-0.2.4/create_fastapi_project/templates/full/backend/app/test/api/test_login.py` & `create_fastapi_project-0.2.5/create_fastapi_project/templates/full/backend/app/test/api/test_login.py`

 * *Files identical despite different names*

### Comparing `create_fastapi_project-0.2.4/create_fastapi_project/templates/full/backend/app/test/api/test_user.py` & `create_fastapi_project-0.2.5/create_fastapi_project/templates/full/backend/app/test/api/test_user.py`

 * *Files identical despite different names*

### Comparing `create_fastapi_project-0.2.4/create_fastapi_project/templates/full/backend/app/test/test_main.py` & `create_fastapi_project-0.2.5/create_fastapi_project/templates/full/backend/app/test/test_main.py`

 * *Files identical despite different names*

### Comparing `create_fastapi_project-0.2.4/create_fastapi_project/templates/full/backend/sonar-project.properties` & `create_fastapi_project-0.2.5/create_fastapi_project/templates/full/backend/sonar-project.properties`

 * *Files identical despite different names*

### Comparing `create_fastapi_project-0.2.4/create_fastapi_project/templates/full/caddy/Caddyfile` & `create_fastapi_project-0.2.5/create_fastapi_project/templates/full/caddy/Caddyfile`

 * *Files identical despite different names*

### Comparing `create_fastapi_project-0.2.4/create_fastapi_project/templates/full/docker-compose-dev.yml` & `create_fastapi_project-0.2.5/create_fastapi_project/templates/full/docker-compose-dev.yml`

 * *Files identical despite different names*

### Comparing `create_fastapi_project-0.2.4/create_fastapi_project/templates/full/docker-compose-test.yml` & `create_fastapi_project-0.2.5/create_fastapi_project/templates/full/docker-compose-test.yml`

 * *Files identical despite different names*

### Comparing `create_fastapi_project-0.2.4/create_fastapi_project/templates/full/docker-compose.yml` & `create_fastapi_project-0.2.5/create_fastapi_project/templates/full/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `create_fastapi_project-0.2.4/create_fastapi_project/templates/full/pgadmin.yml` & `create_fastapi_project-0.2.5/create_fastapi_project/templates/full/pgadmin.yml`

 * *Files identical despite different names*

### Comparing `create_fastapi_project-0.2.4/create_fastapi_project/templates/langchain_basic/.gitignore` & `create_fastapi_project-0.2.5/create_fastapi_project/templates/langchain_basic/.gitignore`

 * *Files identical despite different names*

### Comparing `create_fastapi_project-0.2.4/create_fastapi_project/templates/langchain_basic/Makefile` & `create_fastapi_project-0.2.5/create_fastapi_project/templates/langchain_basic/Makefile`

 * *Files identical despite different names*

### Comparing `create_fastapi_project-0.2.4/create_fastapi_project/templates/langchain_basic/README.md` & `create_fastapi_project-0.2.5/create_fastapi_project/templates/langchain_basic/README.md`

 * *Files identical despite different names*

### Comparing `create_fastapi_project-0.2.4/create_fastapi_project/templates/langchain_basic/backend/Dockerfile` & `create_fastapi_project-0.2.5/create_fastapi_project/templates/full/backend/Dockerfile`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,20 @@
-FROM tiangolo/uvicorn-gunicorn-fastapi:python3.11
+FROM tiangolo/uvicorn-gunicorn-fastapi:python3.11-slim
 ENV PYTHONUNBUFFERED=1
+ENV PIP_DEFAULT_TIMEOUT=100
 WORKDIR /code
 # Install Poetry
 RUN apt clean && apt update && apt install curl -y
 RUN curl -sSL https://install.python-poetry.org | POETRY_HOME=/opt/poetry python && \
     cd /usr/local/bin && \
     ln -s /opt/poetry/bin/poetry && \
     poetry config virtualenvs.create false
 
 # Copy poetry.lock* in case it doesn't exist in the repo
 COPY app/pyproject.toml app/poetry.lock* /code/
 
 # Allow installing dev dependencies to run tests
 ARG INSTALL_DEV=false
-RUN bash -c "if [ $INSTALL_DEV == 'true' ] ; then poetry install --no-root ; else poetry install --no-root --no-dev ; fi"
+RUN bash -c "if [ $INSTALL_DEV == 'true' ] ; then poetry install --no-root ; else poetry install --no-root --only main ; fi"
 
 ENV PYTHONPATH=/code
 EXPOSE 8000
```

### Comparing `create_fastapi_project-0.2.4/create_fastapi_project/templates/langchain_basic/backend/app/app/api/v1/endpoints/chat.py` & `create_fastapi_project-0.2.5/create_fastapi_project/templates/langchain_basic/backend/app/app/api/v1/endpoints/chat.py`

 * *Files identical despite different names*

### Comparing `create_fastapi_project-0.2.4/create_fastapi_project/templates/langchain_basic/backend/app/app/main.py` & `create_fastapi_project-0.2.5/create_fastapi_project/templates/langchain_basic/backend/app/app/main.py`

 * *Files identical despite different names*

### Comparing `create_fastapi_project-0.2.4/create_fastapi_project/templates/langchain_basic/backend/app/app/schemas/message_schema.py` & `create_fastapi_project-0.2.5/create_fastapi_project/templates/langchain_basic/backend/app/app/schemas/message_schema.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from pydantic import BaseModel, validator
+from pydantic import BaseModel, field_validator
 from app.utils.uuid6 import uuid7
 from typing import Any
 
 
 class IUserMessage(BaseModel):
     """User message schema."""
 
@@ -15,24 +15,24 @@
     id: str
     message_id: str
     sender: str
     message: Any
     type: str
     suggested_responses: list[str] = []
 
-    @validator("id", "message_id", pre=True, allow_reuse=True)
+    @field_validator("id", "message_id")
     def check_ids(cls, v):
         if v == "" or v is None:
             return str(uuid7())
         return v
 
-    @validator("sender")
+    @field_validator("sender")
     def sender_must_be_bot_or_you(cls, v):
         if v not in ["bot", "you"]:
             raise ValueError("sender must be bot or you")
         return v
 
-    @validator("type")
+    @field_validator("type")
     def validate_message_type(cls, v):
         if v not in ["start", "stream", "end", "error", "info"]:
             raise ValueError("type must be start, stream or end")
-        return v
+        return v
```

### Comparing `create_fastapi_project-0.2.4/create_fastapi_project/templates/langchain_basic/backend/app/app/schemas/response_schema.py` & `create_fastapi_project-0.2.5/create_fastapi_project/templates/langchain_basic/backend/app/app/schemas/response_schema.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 from math import ceil
 from typing import Any, Generic, TypeVar
 from collections.abc import Sequence
 from fastapi_pagination import Params, Page
 from fastapi_pagination.bases import AbstractPage, AbstractParams
 from pydantic import Field
-from pydantic.generics import GenericModel
+from pydantic import BaseModel
 
 DataType = TypeVar("DataType")
 T = TypeVar("T")
 
 
 class PageBase(Page[T], Generic[T]):
     previous_page: int | None = Field(
-        None, description="Page number of the previous page"
+        default=None, description="Page number of the previous page"
+    )
+    next_page: int | None = Field(
+        default=None, description="Page number of the next page"
     )
-    next_page: int | None = Field(None, description="Page number of the next page")
 
 
-class IResponseBase(GenericModel, Generic[T]):
+class IResponseBase(BaseModel, Generic[T]):
     message: str = ""
-    meta: dict = {}
-    data: T | None
+    meta: dict | Any | None = {}
+    data: T | None = None
 
 
 class IGetResponsePaginated(AbstractPage[T], Generic[T]):
     message: str | None = ""
     meta: dict = {}
     data: PageBase[T]
```

### Comparing `create_fastapi_project-0.2.4/create_fastapi_project/templates/langchain_basic/backend/app/app/templates/chat.py` & `create_fastapi_project-0.2.5/create_fastapi_project/templates/langchain_basic/backend/app/app/templates/chat.py`

 * *Files identical despite different names*

### Comparing `create_fastapi_project-0.2.4/create_fastapi_project/templates/langchain_basic/backend/app/app/utils/adaptive_cards/cards.py` & `create_fastapi_project-0.2.5/create_fastapi_project/templates/langchain_basic/backend/app/app/utils/adaptive_cards/cards.py`

 * *Files identical despite different names*

### Comparing `create_fastapi_project-0.2.4/create_fastapi_project/templates/langchain_basic/backend/app/app/utils/callback.py` & `create_fastapi_project-0.2.5/create_fastapi_project/templates/langchain_basic/backend/app/app/utils/callback.py`

 * *Files identical despite different names*

### Comparing `create_fastapi_project-0.2.4/create_fastapi_project/templates/langchain_basic/backend/app/app/utils/chains.py` & `create_fastapi_project-0.2.5/create_fastapi_project/templates/langchain_basic/backend/app/app/utils/chains.py`

 * *Files identical despite different names*

### Comparing `create_fastapi_project-0.2.4/create_fastapi_project/templates/langchain_basic/backend/app/app/utils/prompt_zero.py` & `create_fastapi_project-0.2.5/create_fastapi_project/templates/langchain_basic/backend/app/app/utils/prompt_zero.py`

 * *Files identical despite different names*

### Comparing `create_fastapi_project-0.2.4/create_fastapi_project/templates/langchain_basic/backend/app/app/utils/tools.py` & `create_fastapi_project-0.2.5/create_fastapi_project/templates/langchain_basic/backend/app/app/utils/tools.py`

 * *Files identical despite different names*

### Comparing `create_fastapi_project-0.2.4/create_fastapi_project/templates/langchain_basic/backend/app/app/utils/uuid6.py` & `create_fastapi_project-0.2.5/create_fastapi_project/templates/langchain_basic/backend/app/app/utils/uuid6.py`

 * *Files identical despite different names*

### Comparing `create_fastapi_project-0.2.4/create_fastapi_project/templates/langchain_basic/docker-compose-dev.yml` & `create_fastapi_project-0.2.5/create_fastapi_project/templates/langchain_basic/docker-compose-dev.yml`

 * *Files identical despite different names*

### Comparing `create_fastapi_project-0.2.4/create_fastapi_project/templates/langchain_basic/docker-compose.yml` & `create_fastapi_project-0.2.5/create_fastapi_project/templates/langchain_basic/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `create_fastapi_project-0.2.4/create_fastapi_project/templates/langchain_basic/frontend/app/main.py` & `create_fastapi_project-0.2.5/create_fastapi_project/templates/langchain_basic/frontend/app/main.py`

 * *Files identical despite different names*

### Comparing `create_fastapi_project-0.2.4/pyproject.toml` & `create_fastapi_project-0.2.5/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "create-fastapi-project"
-version = "0.2.4"
+version = "0.2.5"
 description = ""
 authors = ["jonra1993 <jvargas@allient.io>"]
 readme = "README.md"
 packages = [{include = "create_fastapi_project"}]
 
 [tool.black]
 line-length = 88
@@ -41,15 +41,15 @@
 
 
 [tool.poetry.scripts]
 create-fastapi-project = "create_fastapi_project.main:app"
 
 [tool.poetry.dependencies]
 python = "^3.10"
-typer = {extras = ["all"], version = "^0.9.0"}
+typer = {extras = ["all"], version = "^0.12.0"}
 questionary = "^2.0.0"
 toml = "^0.10.2"
 python-dotenv = "^1.0.0"
 
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.7.0"
```

### Comparing `create_fastapi_project-0.2.4/PKG-INFO` & `create_fastapi_project-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: create-fastapi-project
-Version: 0.2.4
+Version: 0.2.5
 Summary: 
 Author: jonra1993
 Author-email: jvargas@allient.io
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: questionary (>=2.0.0,<3.0.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
-Requires-Dist: typer[all] (>=0.9.0,<0.10.0)
+Requires-Dist: typer[all] (>=0.12.0,<0.13.0)
 Description-Content-Type: text/markdown
 
 # Create FastAPI Project
 
 We love ❤️ [FastAPI](https://fastapi.tiangolo.com/) and its ecosystem so we decided to make easier to get started with [FastAPI](https://fastapi.tiangolo.com/) projects. By using the `create-fastapi-project` CLI tool, you can quickly start building a new FastAPI application with a basic folder structure, with everything set up for you.
 
 To get started, use the following command:
```

