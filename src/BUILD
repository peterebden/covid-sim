cc_library(
    name = "lib",
    srcs = glob(["*.cpp"], exclude=["CovidSim.cpp"]),
    hdrs = glob(["*.h"]),
    defines = ["UNIX"],
    # TODO(peterebden): Should remove this, after various unused / uninitialised variable warnings are cleaned up.
    cflags = ["-Wno-error"],
)

cc_binary(
    name = "sim",
    srcs = ["CovidSim.cpp"],
    cflags = ["-Wno-error"],
    deps = [
        ":lib",
    ],
)
