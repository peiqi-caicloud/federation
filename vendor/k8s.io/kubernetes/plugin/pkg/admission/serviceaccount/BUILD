load("@io_bazel_rules_go//go:def.bzl", "go_library")

go_library(
    name = "go_default_library",
    srcs = [
        "admission.go",
        "doc.go",
    ],
    importpath = "k8s.io/kubernetes/plugin/pkg/admission/serviceaccount",
    visibility = ["//visibility:public"],
    deps = [
        "//vendor/k8s.io/apimachinery/pkg/api/errors:go_default_library",
        "//vendor/k8s.io/apimachinery/pkg/apis/meta/v1:go_default_library",
        "//vendor/k8s.io/apimachinery/pkg/labels:go_default_library",
        "//vendor/k8s.io/apimachinery/pkg/runtime/schema:go_default_library",
        "//vendor/k8s.io/apimachinery/pkg/util/sets:go_default_library",
        "//vendor/k8s.io/apiserver/pkg/admission:go_default_library",
        "//vendor/k8s.io/apiserver/pkg/storage/names:go_default_library",
        "//vendor/k8s.io/kubernetes/pkg/api/pod:go_default_library",
        "//vendor/k8s.io/kubernetes/pkg/apis/core:go_default_library",
        "//vendor/k8s.io/kubernetes/pkg/client/clientset_generated/internalclientset:go_default_library",
        "//vendor/k8s.io/kubernetes/pkg/client/informers/informers_generated/internalversion:go_default_library",
        "//vendor/k8s.io/kubernetes/pkg/client/listers/core/internalversion:go_default_library",
        "//vendor/k8s.io/kubernetes/pkg/kubeapiserver/admission:go_default_library",
        "//vendor/k8s.io/kubernetes/pkg/kubeapiserver/admission/util:go_default_library",
        "//vendor/k8s.io/kubernetes/pkg/serviceaccount:go_default_library",
    ],
)

filegroup(
    name = "package-srcs",
    srcs = glob(["**"]),
    tags = ["automanaged"],
    visibility = ["//visibility:private"],
)

filegroup(
    name = "all-srcs",
    srcs = [":package-srcs"],
    tags = ["automanaged"],
    visibility = ["//visibility:public"],
)
