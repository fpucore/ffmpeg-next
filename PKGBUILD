# Maintainer: Chris McGimpsey-Jones <chrisjones.unixmen@gmail.com>
# Contributors: Daniel Bermond <dbermond@archlinux.org>, Kamran Mackey <kamranm1200@gmail.com>, richteer <richteer@lastprime.net>, DrZaius <lou@fakeoutdoorsman.com>

pkgname=ffmpeg-next
pkgver=10.1
pkgrel=2
pkgdesc='Bleeding-edge, hybrid-upstream ffmpeg suite.'
arch=('x86_64')
url='https://www.freedompublishersunion.net/h-linux.html'
license=('GPL-3.0-or-later')
depends=(
  alsa-lib
  aom
  bzip2
  cairo
  dav1d
  fontconfig
  freetype2
  fribidi
  glib2
  glibc
  glslang
  gmp
  gnutls
  gsm
  harfbuzz
  jack
  lame
  lcms2
  libass
  libavc1394
  libbluray
  libbs2b
  libdrm
  libdvdnav
  libdvdread
  libgcc
  libiec61883
  libjxl
  libmodplug
  libopenmpt
  libplacebo
  libpulse
  libraw1394
  librsvg
  libsoxr
  libssh
  libtheora
  libva
  libvdpau
  libvorbis
  libvpl
  libvpx
  libwebp
  libx11
  libxcb
  libxext
  libxml2
  libxv
  ocl-icd
  opencore-amr
  openjpeg2
  opus
  rav1e
  rubberband
  sdl2
  snappy
  speex
  srt
  svt-av1
  v4l-utils
  vid.stab
  vmaf
  vulkan-icd-loader
  x264
  x265
  xvidcore
  xz
  zeromq
  zimg
  zlib)
makedepends=(
  amf-headers
  avisynthplus
  clang
  ffnvcodec-headers
  frei0r-plugins
  git
  ladspa
  libgl
  nasm
  opencl-headers
  spirv-headers
  vapoursynth
  vulkan-headers)
optdepends=(
  'avisynthplus: for AviSynthPlus support'
  'frei0r-plugins: for Frei0r video effects support'
  'ladspa: for LADSPA filters'
  'nvidia-utils: for NVIDIA NVDEC/NVENC support'
  'vapoursynth: for VapourSynth demuxer support'
  'vpl-runtime: for Intel Quick Sync Video')
provides=(
  'ffmpeg'
  'libavcodec.so'
  'libavdevice.so'
  'libavfilter.so'
  'libavformat.so'
  'libavutil.so'
  'libswresample.so'
  'libswscale.so')
conflicts=('ffmpeg')

# 'git+https://git.ffmpeg.org/ffmpeg.git'
source=('040-ffmpeg-add-av_stream_get_first_dts-for-chromium.patch')
sha256sums=('SKIP')

prepare() {
    patch -d ffmpeg -Np1 -i "${srcdir}/040-ffmpeg-add-av_stream_get_first_dts-for-chromium.patch"
}

#pkgver() {
#    printf '%s.r%s.g%s' "$(git -C ffmpeg describe --tags --long | awk -F'-' '{ sub(/^n/, "", $1); print $1 }')" \
#                        "$(git -C ffmpeg describe --tags --match 'N' | awk -F'-' '{ print $2 }')" \
#                        "$(git -C ffmpeg rev-parse --short HEAD)"
#}

build() {
    cd ffmpeg
    printf '%s\n' '  -> Running ffmpeg configure script...'

    make tools/qt-faststart
}

package() {
    make -C ffmpeg DESTDIR="$pkgdir" install
    install -D -m755 ffmpeg/tools/qt-faststart -t "${pkgdir}/usr/bin"
}
