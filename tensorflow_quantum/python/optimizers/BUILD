package(default_visibility = ["//visibility:public"])

licenses(["notice"])

# Export for the PIP package.
exports_files(["__init__.py"])

py_library(
    name = "rotosolve_minimizer",
    srcs = ["rotosolve_minimizer.py"],
)

py_test(
    name = "rotosolve_minimizer_test",
    srcs = ["rotosolve_minimizer_test.py"],
    python_version = "PY3",
    deps = [
        ":rotosolve_minimizer",
        "//tensorflow_quantum/python/layers/high_level:pqc",
        "//tensorflow_quantum/core/ops:tfq_ps_util_ops_py"
    ],
)
