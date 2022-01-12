licenses(["restricted"])

package(default_visibility = ["//visibility:public"])

java_runtime(
    name = "windows_jdk8",
    srcs = [],
    java_home = "C:/openjdk",
)

platform(
    name = "rbe_windows_ltsc2019",
    constraint_values = [
        "@bazel_tools//platforms:x86_64",
        "@bazel_tools//platforms:windows",
    ],
    remote_execution_properties = """
        properties:{
          name: "container-image"
          value: "docker://gcr.io/tensorflow-testing/tf-win2019-rbe@sha256:aebcc7c24e57a761bc2674a2c6c6e34cefbf6a09c6b61e029b054e4372d227c0"
        }
        properties:{
          name: "OSFamily"
          value: "Windows"
        }
        properties:{
          name: "Pool" value: "default"
        }
        """,
)
