project('godot', 'cpp', 'c')

if get_option('xml')
  add_global_arguments('-DXML_ENABLED', language : 'cpp')
endif

python_int = find_program('python')
core_inc = include_directories('.', 'core', 'core/math', 'platform/x11')
subdir('core')
subdir('drivers')

