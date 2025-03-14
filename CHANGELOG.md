# Changelog

All notable changes to this project will be documented here.

## [v1.0.0] - 2022-07-29

### Fix

- Fix `http.py/do_request` method stream read bug.
<br/>
<br/>


## [v1.0.0] - 2023-05-29

### Test

- Add test cases.

### Support

- Supported `asyncio-oss` package in PyPI.
<br/>
<br/>


## [v1.0.1] - 2023-05-30

### Build

- Bump version to 1.0.1 for PyPI package description updating.
<br/>
<br/>


## [v1.0.2] - 2023-06-24

### Refactor & Fix & Test

- Remove unused fields add params in `asyncio_oss/http.py api.py` files.

### Fix

- Fix `asyncio_oss/iterators.py/_BaseIterator/__aiter__` method bug.

### Test

- Add `list_buckets` test case in `tests/service_test.py` for `Service` class.
<br/>
<br/>


## [v1.1.0] - 2023-06-25

### Refactor

- Remove unused objects and methods in `asyncio_oss/models.py` and `asyncio_oss/utils.py` to streamline sdk package.

### Feature

- Support oss2==2.18.0 newest apis.
- Support global log.
<br/>
<br/>


## [v1.1.1] - 2023-06-28

### Fix

- Fix the bug of wrong signature of `put_object_tagging` interface caused by default `Content-Type` of aiohttp.
<br/>
<br/>


## [v1.1.2] - 2023-08-11

### Build

- Remove test module from package.

### Test

- Add `upload_big_file` test case in `tests/bucket_test.py` for `Bucket` class.

### Docs

- Extract `ChangeLogs` from `README.md` to `CHANGELOG.md`.


## [v1.1.3] - 2024-01-18

### Fix

- Fix a bug that prevented Bucket from closing a session by calling the close method because the close method was not implemented in the `http` module.

### Test

- Add `close` test case for session closing.
