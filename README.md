# mesa-build

GitHub Actions builds of Mesa's Intel Vulkan driver (ANV) and Intel tools (`aubinator_error_decode`, hang replay)
from [gitlab.freedesktop.org/mesa/mesa](https://gitlab.freedesktop.org/mesa/mesa), in a Fedora 45 container, for
testing on a Bazzite handheld (MSI Claw 8 EX, Intel Panther Lake) without installing them system-wide.

Run the workflow with a Mesa ref (branch, tag or commit); the artifact is the installed tree (`usr/…`). Use the driver
for one program with `VK_DRIVER_FILES=<path to a copy of intel_icd.x86_64.json that points to the extracted .so>`.
