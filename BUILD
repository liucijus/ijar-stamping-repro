genrule(
    name = "stamp_and_corrupt_manifest_with_sections",
    outs = ["scala_library_stamped.jar"],
    cmd = "./$(location @bazel_tools//tools/jdk:ijar) --nostrip_jar --target_label @my_label $(location scala_library.jar) $@",
    tools = ["@bazel_tools//tools/jdk:ijar"],
    srcs = ["scala_library.jar"],
)
