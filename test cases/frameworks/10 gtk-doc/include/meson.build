cdata = configuration_data()
parts = meson.project_version().split('.')
cdata.set('FOO_MAJOR_VERSION', parts[0])
cdata.set('FOO_MINOR_VERSION', parts[1])
cdata.set('FOO_MICRO_VERSION', parts[2])
configure_file(input : 'foo-version.h.in',
  output : 'foo-version.h',
  configuration : cdata,
  install : true,
  install_dir : get_option('includedir'))
