java_library(
    name = "dagger",
    licenses = [
        "permissive",
    ],
    visibility = [
        "//visibility:public",
    ],
    exports = [
        "//external:jar/mvncom/google/dagger/dagger",
    ],
    runtime_deps = [
        "//third_party/maven/javax/inject:javax_inject",
    ],
)

java_library(
    name = "dagger_compiler",
    licenses = [
        "permissive",
    ],
    visibility = [
        "//visibility:public",
    ],
    exports = [
        "//external:jar/mvncom/google/dagger/dagger_compiler",
    ],
    runtime_deps = [
        ":dagger",
        ":dagger_producers",
        ":dagger_spi",
        "//third_party/maven/com/google/googlejavaformat:google_java_format",
        "//third_party/maven/com/google/guava",
        "//third_party/maven/com/squareup:javapoet",
        "//third_party/maven/javax/annotation:jsr250_api",
        "//third_party/maven/javax/inject:javax_inject",
    ],
)

java_library(
    name = "dagger_producers",
    licenses = [
        "permissive",
    ],
    visibility = [
        "//third_party/maven:__subpackages__",
    ],
    exports = [
        "//external:jar/mvncom/google/dagger/dagger_producers",
    ],
    runtime_deps = [
        ":dagger",
        "//third_party/maven/com/google/guava",
        "//third_party/maven/javax/inject:javax_inject",
        "//third_party/maven/org/checkerframework:checker_compat_qual",
    ],
)

java_library(
    name = "dagger_spi",
    licenses = [
        "permissive",
    ],
    visibility = [
        "//third_party/maven:__subpackages__",
    ],
    exports = [
        "//external:jar/mvncom/google/dagger/dagger_spi",
    ],
    runtime_deps = [
        ":dagger",
        ":dagger_producers",
        "//third_party/maven/com/google/guava",
        "//third_party/maven/javax/inject:javax_inject",
    ],
)
