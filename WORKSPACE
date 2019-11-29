workspace(name = "csharp_examples")

load("@bazel_tools//tools/build_defs/repo:http.bzl", "http_archive")

http_archive(
    name = "d2l_rules_csharp",

    # Pin a commit in my fork of rules_jrbeverly
    #
    # Navigate to:
    #   https://github.com/jrbeverly/rules_csharp/commits/master
    # to list the commit for each of the branches (or pin a branch)

    # version pin
    # strip_prefix = "rules_csharp-0.6",
    # urls = ["https://github.com/Brightspace/rules_csharp/archive/v0.6.tar.gz"],

    # # master
    # strip_prefix = "rules_csharp-a31980f706ef71e571bbd4f1e34d9ba8adf3decd",
    # urls = [
    #     "https://github.com/jrbeverly/rules_csharp/archive/a31980f706ef71e571bbd4f1e34d9ba8adf3decd.tar.gz",
    # ],

    # # resgen/compile-resx-files
    # strip_prefix = "rules_csharp-a31980f706ef71e571bbd4f1e34d9ba8adf3decd",
    # urls = [
    #     "https://github.com/jrbeverly/rules_csharp/archive/a31980f706ef71e571bbd4f1e34d9ba8adf3decd.tar.gz",
    # ],

    # # dotnet/wrap-the-dotnet-exe
    # strip_prefix = "rules_csharp-ad39050ba88f2ff0002f51be7ec2eb389b519fe6",
    # urls = [
    #     "https://github.com/jrbeverly/rules_csharp/archive/ad39050ba88f2ff0002f51be7ec2eb389b519fe6.tar.gz",
    # ],

    # proto/resx-as-macro
    strip_prefix = "rules_csharp-fc3863501e115f299d50240174d2c4b519a86565",
    urls = [
        "https://github.com/jrbeverly/rules_csharp/archive/fc3863501e115f299d50240174d2c4b519a86565.tar.gz",
    ],
)

load(
    "@d2l_rules_csharp//csharp:defs.bzl",
    "csharp_register_toolchains",
    "csharp_repositories",
)

csharp_repositories()

csharp_register_toolchains()
