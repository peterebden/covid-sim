cc_library(
    name = "lib",
    srcs = glob(["*.cpp"], exclude=["CovidSim.cpp"]),
    hdrs = glob(["*.h"]),
)

cc_binary(
    name = "sim",
    srcs = ["CovidSim.cpp"],
    deps = [
        ":lib",
    ],
)
