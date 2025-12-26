# Overlay UI Engine

## Build

### Prerequisites

```bash
# Install pixi
curl -fsSL https://pixi.sh/install.sh | sh
hash -r
```

```bash
# Get RmlUi (Using vcpkg is easiest, or clone & build manually)
git clone https://github.com/microsoft/vcpkg.git
./vcpkg/bootstrap-vcpkg.sh -disableMetrics
hash -r
./vcpkg/vcpkg install freetype glfw3

export VCPKG_ROOT=`pwd`/vcpkg
export PATH=$VCPKG_ROOT:$PATH

git clone https://github.com/mikke89/RmlUi.git

pixi run build-rmlui
./RmlUi/build/rmlui_tutorial_template  # This will cause a freeze.
```
