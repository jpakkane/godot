project('godot', 'cpp', 'c')

if get_option('xml')
  add_global_arguments('-DXML_ENABLED', language : 'cpp')
endif

vc = configuration_data()
vc.set('VERSION_SHORT_NAME', 'godot')
vc.set('VERSION_NAME', 'Godot engine')
vc.set('VERSION_MAJOR', 1)
vc.set('VERSION_MINOR', 0)
vc.set('VERSION_REVISION', 'rev')
vc.set('VERSION_STATUS', 'beta')
configure_file(input : 'version.h.in', output : 'version.h', configuration : vc)

python_int = find_program('python')
core_inc = include_directories('.', 'core', 'core/math', 'platform/x11')
subdir('core')
subdir('drivers')

