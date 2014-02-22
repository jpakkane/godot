bindgen = generator(python_int, outputs : '@BASENAME@.inc', arguments : ['@SOURCE_DIR@/make_binders.py', '@OUTPUT@'])
generated_inc = bindgen.process('method_bind.h')

subdir('os')
subdir('math')
subdir('io')

core_src = ['array.cpp',
'color.cpp',
'command_queue_mt.cpp',
'compressed_translation.cpp',
'core_string_names.cpp',
'dictionary.cpp',
'dvector.cpp',
'error_macros.cpp',
'event_queue.cpp',
'fpstr.cpp',
'global_constants.cpp',
'globals.cpp',
'image.cpp',
'image_quantize.cpp',
'input_map.cpp',
'message_queue.cpp',
'method_bind.cpp',
'object.cpp',
'object_type_db.cpp',
'packed_data_container.cpp',
'pair.cpp',
'path_db.cpp',
'path_remap.cpp',
'pool_allocator.cpp',
'print_string.cpp',
'reference.cpp',
'ref_ptr.cpp',
'register_core_types.cpp',
'resource.cpp',
'res_ptr.cpp',
'rid.cpp',
'safe_refcount.cpp',
'script_debugger_debugger.cpp',
'script_debugger_local.cpp',
'script_debugger_remote.cpp',
'script_language.cpp',
'string_db.cpp',
'translation.cpp',
'undo_redo.cpp',
'ustring.cpp',
'variant_call.cpp',
'variant.cpp',
'variant_op.cpp',
'vmap.cpp',
'vset.cpp']

corelib = static_library('core', sources : core_src, include_dirs : core_inc)

