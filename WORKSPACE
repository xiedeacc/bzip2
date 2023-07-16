workspace(name = "bzip2")

load("@bazel_tools//tools/build_defs/repo:git.bzl", "git_repository", "new_git_repository")
load("@bazel_tools//tools/build_defs/repo:http.bzl", "http_archive")

http_archive(
    name = "platforms",
    sha256 = "d62cb553b378d2acb4e63de21dce82d025ce2ef2bdfcee2c2b742788314df0b1",
    strip_prefix = "platforms-0.0.2",
    urls = [
        "https://code.wifi.com/xieyz01/platforms/-/archive/0.0.2/platforms-0.0.2.tar.gz",
    ],
)

http_archive(
    name = "bazel_gazelle",
    sha256 = "f795b82792edeb03a7a060a908bc2cfc9702273b1387479fb99d208e83a3d7ad",
    strip_prefix = "bazel-gazelle-v0.24.0",
    urls = [
        "https://code.wifi.com/xieyz01/bazel-gazelle/-/archive/v0.24.0/bazel-gazelle-v0.24.0.tar.gz",
    ],
)

http_archive(
    name = "bazel_skylib",
    sha256 = "3b620033ca48fcd6f5ef2ac85e0f6ec5639605fa2f627968490e52fc91a9932f",
    strip_prefix = "bazel-skylib-1.3.0",
    urls = [
        "https://code.wifi.com/xieyz01/bazel-skylib/-/archive/1.3.0/bazel-skylib-1.3.0.tar.gz",
    ],
)

load("@bazel_skylib//lib:versions.bzl", "versions")

versions.check("5.2.0")

http_archive(
    name = "rules_cc",
    sha256 = "af6cc82d87db94585bceeda2561cb8a9d55ad435318ccb4ddfee18a43580fb5d",
    strip_prefix = "rules_cc-0.0.4",
    urls = [
        "https://code.wifi.com/xieyz01/rules_cc/-/archive/0.0.4/rules_cc-0.0.4.tar.gz",
    ],
)

http_archive(
    name = "rules_foreign_cc",
    sha256 = "c7527231b3e10643efc6add713311e8eb4f707a5a8f3835fc2d335db5fbe7217",
    strip_prefix = "rules_foreign_cc-fe3c552dda3a1f5d31ed6014ba6229a5a9283161",
    urls = [
        "https://code.wifi.com/xieyz01/rules_foreign_cc/-/archive/fe3c552dda3a1f5d31ed6014ba6229a5a9283161/rules_foreign_cc-fe3c552dda3a1f5d31ed6014ba6229a5a9283161.tar.gz",
    ],
)

load("@rules_foreign_cc//foreign_cc:repositories.bzl", "rules_foreign_cc_dependencies")

http_archive(
    name = "rules_proto",
    sha256 = "9850fcf6ad40fa348e6f13b2cfef4bb4639762f804794f2bf61d988f4ba0dae9",
    strip_prefix = "rules_proto-4.0.0-3.19.2-2",
    urls = [
        "https://code.wifi.com/xieyz01/rules_proto/-/archive/4.0.0-3.19.2-2/rules_proto-4.0.0-3.19.2-2.tar.gz",
    ],
)

load("@rules_proto//proto:repositories.bzl", "rules_proto_dependencies", "rules_proto_toolchains")

http_archive(
    name = "rules_perl",
    sha256 = "0f234dbaf4acacee9e131a117c8b02bc8910724427ec8e3d69df5e3b36899477",
    strip_prefix = "rules_perl-ca8ea624afc939bdb70100ac8d609d2b8d81308c",
    urls = [
        "https://code.wifi.com/xieyz01/rules_perl/-/archive/ca8ea624afc939bdb70100ac8d609d2b8d81308c/rules_perl-ca8ea624afc939bdb70100ac8d609d2b8d81308c.tar.gz",
    ],
)

load("@rules_perl//perl:deps.bzl", "perl_register_toolchains")

perl_register_toolchains()

http_archive(
    name = "rules_python",
    sha256 = "94750828b18044533e98a129003b6a68001204038dc4749f40b195b24c38f49f",
    strip_prefix = "rules_python-0.21.0",
    urls = [
        "https://code.wifi.com/xieyz01/rules_python/-/archive/0.21.0/rules_python-0.21.0.tar.gz",
    ],
)

http_archive(
    name = "rules_java",
    sha256 = "7436356107f1cf24b45f95909753e521efe2d06622de184ea25e13cb7a0d72f9",
    strip_prefix = "rules_java-5.5.0",
    urls = [
        "https://code.wifi.com/xieyz01/rules_java/-/archive/5.5.0/rules_java-5.5.0.tar.gz",
    ],
)

http_archive(
    name = "build_bazel_rules_swift",
    sha256 = "104b16612b1084918d58083b3ee2f6521eb202b4502019870da7351d10a4777f",
    strip_prefix = "rules_swift-1.5.1",
    urls = [
        "https://code.wifi.com/xieyz01/rules_swift/-/archive/1.5.1/rules_swift-1.5.1.tar.gz",
    ],
)

http_archive(
    name = "build_bazel_rules_apple",
    sha256 = "d6735ed25754dbcb4fce38e6d72c55b55f6afa91408e0b72f1357640b88bb49c",
    strip_prefix = "rules_apple-0.31.3",
    urls = [
        "https://code.wifi.com/xieyz01/rules_apple/-/archive/0.31.3/rules_apple-0.31.3.tar.gz",
    ],
)

http_archive(
    name = "build_bazel_apple_support",
    sha256 = "c02a8c902f405e5ea12b815f426fbe429bc39a2628b290e50703d956d40f5542",
    strip_prefix = "apple_support-0.10.0",
    urls = [
        "https://code.wifi.com/xieyz01/apple_support/-/archive/0.10.0/apple_support-0.10.0.tar.gz",
    ],
)

http_archive(
    name = "io_bazel_rules_docker",
    sha256 = "91844808532e5ce316b3c010929493c0244f3d37593afd6de04f71821d5136d9",
    strip_prefix = "rules_docker-v0.9.0",
    urls = [
        "https://code.wifi.com/xieyz01/rules_docker/-/archive/v0.9.0/rules_docker-v0.9.0.tar.gz",
    ],
)

http_archive(
    name = "io_bazel_rules_go",
    sha256 = "5169057086cacb107e0c8e8430f90b17518fc8052e1ab0ce25cbc227287f1cd4",
    strip_prefix = "rules_go-b397ab7ace3c4131f48b5f4d4d7e7e9e6809e0d2",
    urls = [
        "https://code.wifi.com/xieyz01/rules_go/-/archive/b397ab7ace3c4131f48b5f4d4d7e7e9e6809e0d2/rules_go-b397ab7ace3c4131f48b5f4d4d7e7e9e6809e0d2.tar.gz",
    ],
)

load("@io_bazel_rules_go//go:deps.bzl", "go_register_toolchains", "go_rules_dependencies")

http_archive(
    name = "rules_pkg",
    sha256 = "d258fb6965cf3d7ebdbe146ec7e28b605f0644cb880101604e166e35d4ca62bc",
    strip_prefix = "rules_pkg-0.7.1",
    url = "https://code.wifi.com/xieyz01/rules_pkg/-/archive/0.7.1/rules_pkg-0.7.1.tar.gz",
)

load("@rules_pkg//:deps.bzl", "rules_pkg_dependencies")

http_archive(
    name = "rules_jvm_external",
    sha256 = "f36441aa876c4f6427bfb2d1f2d723b48e9d930b62662bf723ddfb8fc80f0140",
    strip_prefix = "rules_jvm_external-4.1",
    urls = ["https://code.wifi.com/xieyz01//rules_jvm_external/-/archive/4.1/rules_jvm_external-4.1.tar.gz"],
)

rules_foreign_cc_dependencies()

rules_proto_dependencies()

rules_proto_toolchains()

go_rules_dependencies()

go_register_toolchains(version = "1.18")

rules_pkg_dependencies()
