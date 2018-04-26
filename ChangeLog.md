2018.04 - version 1.1.0

* Private method BlobRestProxy::getBlobUrl now preserves primary URI path when exists.
* MD files are modified for better readability and formatting.
* CACERT can now be set when creating RestProxies using `$options` parameter.
* Added a sample in `BlobSamples.php` to list all blobs with certain prefix. This is a recommended implementation of using continuation token to list all the blobs.
* Removed unnecessary trailing spaces.
* Assertions are re-factored in test cases.
* Now the test framework uses `PHPUnit\Framework\TestCase` instead of `PHPUnit_Framework_TestCase`.

2018.01 - version 1.0.0

* Created `BlobSharedAccessSignatureHelper` and moved method `SharedAccessSignatureHelper::generateBlobServiceSharedAccessSignatureToken()` into `BlobSharedAccessSignatureHelper`.
* Added static builder methods `createBlobService` and `createContainerAnonymousAccess` into `BlobRestProxy`.
* Removed `dataSerializer` parameter from `BlobRextProxy` constructor.
* Added `setUseTransactionalMD5` method for options of `BlobRestProxy::CreateBlockBlob` and `BlobRestProxy::CreatePageBlobFromContent`. Default false, enabling transactional MD5 validation will take more cpu and memory resources.
* Fixed a bug that CopyBlobFromURLOptions not found.
* Deprecated PHP 5.5 support.