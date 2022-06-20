omenrgb_lnx_sources = [
  'main.c',
  'omenrgb_lnx-window.c',
  'omenrgb_lnx-application.c',
]

omenrgb_lnx_deps = [
  dependency('libadwaita-1', version: '>= 1.0'),
]

gnome = import('gnome')

omenrgb_lnx_sources += gnome.compile_resources('omenrgb_lnx-resources',
  'omenrgb_lnx.gresource.xml',
  c_name: 'omenrgb_lnx'
)

executable('omenrgb-lnx', omenrgb_lnx_sources,
  dependencies: omenrgb_lnx_deps,
  install: true,
)
