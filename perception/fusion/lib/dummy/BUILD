load("@rules_cc//cc:defs.bzl", "cc_library", "cc_test")
load("//tools:cpplint.bzl", "cpplint")

package(default_visibility = ["//visibility:public"])

cc_library(
    name = "dummy_algorithms",
    srcs = ["dummy_algorithms.cc"],
    hdrs = ["dummy_algorithms.h"],
    deps = [
        "//cyber",
        "//modules/perception/fusion/base",
        "//modules/perception/fusion/lib/interface",
        "//modules/perception/fusion/lib/interface:base_fusion_system",
        "@eigen",
    ],
)

cc_test(
    name = "dummy_algorithms_test",
    size = "small",
    srcs = ["dummy_algorithms_test.cc"],
    deps = [
        ":dummy_algorithms",
        "@com_google_googletest//:gtest_main",
        "//modules/perception/fusion/lib/interface:base_fusion_system",
    ],
)

cpplint()
