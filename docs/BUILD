genrule(
    name = "github-pages",
    srcs = glob(["build/*.html"], allow_empty = True),  # ✅ Now it won't fail if no .html files exist
    outs = ["github-pages.tar"],
    cmd = "tar -cf $@ $(SRCS)",
    visibility = ["//visibility:public"],
)
