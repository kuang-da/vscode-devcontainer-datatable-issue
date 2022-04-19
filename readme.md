# Readme

## Pip version

```bash
pip --version
pip 22.0.4 from /usr/local/lib/python3.10/site-packages/pip (python 3.10)
```

## Error log

```bash
vscode ➜ /workspaces/parse $ pip install datatable
Defaulting to user installation because normal site-packages is not writeable
Collecting datatable
  Downloading datatable-1.0.0.tar.gz (1.1 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 1.1/1.1 MB 29.9 MB/s eta 0:00:00
  Getting requirements to build wheel ... done
  Preparing metadata (pyproject.toml) ... error
  error: subprocess-exited-with-error
  
  × Preparing metadata (pyproject.toml) did not run successfully.
  │ exit code: 1
  ╰─> [39 lines of output]
      Building extension _datatable
      Build directory = 'build/build'
      Created directory 'build/build'
      Destination directory = 'src/datatable/lib'
      Added 309 source files from pattern src/core/**/*.cc: ['src/core/set_funcs.cc', 'src/core/sort_groups.cc', 'src/core/cstring.cc', 'src/core/rowindex_array.cc', 'src/core/mmm.cc', 'src/core/groupby.cc', 'src/core/api.cc', 'src/core/stats.cc', 'src/core/datatable.cc', 'src/core/writebuf.cc', 'src/core/call_logger.cc', 'src/core/datatablemodule.cc', 'src/core/wstringcol.cc', 'src/core/sort_insert.cc', 'src/core/column.cc', 'src/core/rowindex_slice.cc', 'src/core/column_from_python.cc', 'src/core/options.cc', 'src/core/py_buffers.cc', 'src/core/column_from_arrow.cc', 'src/core/py_encodings.cc', 'src/core/sort.cc', 'src/core/buffer.cc', 'src/core/rowindex.cc', 'src/core/stype.cc', 'src/core/ltype.cc', 'src/core/encodings.cc', 'src/core/write/value_writer.cc', 'src/core/write/write_manager.cc', 'src/core/write/writing_context.cc', 'src/core/write/write_chronicler.cc', 'src/core/write/csv_writer.cc', 'src/core/jay/open_jay.cc', 'src/core/jay/save_jay.cc', 'src/core/expr/fexpr_func.cc', 'src/core/expr/fexpr_cut.cc', 'src/core/expr/py_update.cc', 'src/core/expr/fexpr_func_unary.cc', 'src/core/expr/head.cc', 'src/core/expr/head_func_isclose.cc', 'src/core/expr/fexpr_list.cc', 'src/core/expr/fexpr_literal_none.cc', 'src/core/expr/fexpr_literal_sliceint.cc', 'src/core/expr/fexpr_literal_string.cc', 'src/core/expr/fexpr_literal_slicestr.cc', 'src/core/expr/fexpr_ifelse.cc', 'src/core/expr/py_sort.cc', 'src/core/expr/fexpr_frame.cc', 'src/core/expr/args_registry.cc', 'src/core/expr/fexpr_literal.cc', 'src/core/expr/fexpr_literal_sliceall.cc', 'src/core/expr/fexpr_literal_bool.cc', 'src/core/expr/fexpr_slice.cc', 'src/core/expr/head_func_unary.cc', 'src/core/expr/py_by.cc', 'src/core/expr/head_reduce_binary.cc', 'src/core/expr/head_reduce.cc', 'src/core/expr/fexpr_column_asattr.cc', 'src/core/expr/fexpr_round.cc', 'src/core/expr/py_join.cc', 'src/core/expr/fexpr_dict.cc', 'src/core/expr/head_func_colset.cc', 'src/core/expr/namespace.cc', 'src/core/expr/fexpr_column_asarg.cc', 'src/core/expr/fexpr_literal_type.cc', 'src/core/expr/eval_context.cc', 'src/core/expr/fexpr_literal_float.cc', 'src/core/expr/fexpr_literal_range.cc', 'src/core/expr/head_func_binary.cc', 'src/core/expr/workframe.cc', 'src/core/expr/fexpr.cc', 'src/core/expr/fexpr_qcut.cc', 'src/core/expr/expr.cc', 'src/core/expr/head_reduce_nullary.cc', 'src/core/expr/head_reduce_unary.cc', 'src/core/expr/fexpr_literal_int.cc', 'src/core/expr/fexpr_astype.cc', 'src/core/expr/head_func_shift.cc', 'src/core/expr/head_func.cc', 'src/core/expr/re/fexpr_match.cc', 'src/core/expr/funary/hyperbolic.cc', 'src/core/expr/funary/pyfn.cc', 'src/core/expr/funary/special.cc', 'src/core/expr/funary/basic.cc', 'src/core/expr/funary/umaker.cc', 'src/core/expr/funary/floating.cc', 'src/core/expr/funary/exponential.cc', 'src/core/expr/funary/trigonometric.cc', 'src/core/expr/fnary/rowsum.cc', 'src/core/expr/fnary/rowall.cc', 'src/core/expr/fnary/rowsd.cc', 'src/core/expr/fnary/rowcount.cc', 'src/core/expr/fnary/rowany.cc', 'src/core/expr/fnary/rowminmax.cc', 'src/core/expr/fnary/rowmean.cc', 'src/core/expr/fnary/rowfirstlast.cc', 'src/core/expr/fnary/fnary.cc', 'src/core/expr/time/fexpr_hour_min_sec.cc', 'src/core/expr/time/fexpr_ymdt.cc', 'src/core/expr/time/fexpr_day_of_week.cc', 'src/core/expr/time/fexpr_ymd.cc', 'src/core/expr/time/fexpr_year_month_day.cc', 'src/core/expr/fbinary/fexpr__le__.cc', 'src/core/expr/fbinary/fexpr__mod__.cc', 'src/core/expr/fbinary/math.cc', 'src/core/expr/fbinary/pyfn.cc', 'src/core/expr/fbinary/bimaker.cc', 'src/core/expr/fbinary/bitwise.cc', 'src/core/expr/fbinary/fexpr__add__.cc', 'src/core/expr/fbinary/fexpr__eq__.cc', 'src/core/expr/fbinary/fexpr__gt__.cc', 'src/core/expr/fbinary/fexpr__mul__.cc', 'src/core/expr/fbinary/fexpr_binaryop.cc', 'src/core/expr/fbinary/fexpr__ne__.cc', 'src/core/expr/fbinary/fexpr__sub__.cc', 'src/core/expr/fbinary/fexpr__pow__.cc', 'src/core/expr/fbinary/fexpr__truediv__.cc', 'src/core/expr/fbinary/fexpr__lt__.cc', 'src/core/expr/fbinary/fexpr__compare__.cc', 'src/core/expr/fbinary/fexpr__floordiv__.cc', 'src/core/expr/fbinary/fexpr__ge__.cc', 'src/core/expr/str/fexpr_len.cc', 'src/core/frame/to_pandas.cc', 'src/core/frame/integrity_check.cc', 'src/core/frame/to_arrow.cc', 'src/core/frame/__init__.cc', 'src/core/frame/stats.cc', 'src/core/frame/__sizeof__.cc', 'src/core/frame/__iter__.cc', 'src/core/frame/key.cc', 'src/core/frame/replace.cc', 'src/core/frame/to_csv.cc', 'src/core/frame/cbind.cc', 'src/core/frame/to_numpy.cc', 'src/core/frame/to_python.cc', 'src/core/frame/rbind.cc', 'src/core/frame/names.cc', 'src/core/frame/repeat.cc', 'src/core/frame/__getbuffer__.cc', 'src/core/frame/join.cc', 'src/core/frame/__repr__.cc', 'src/core/frame/py_frame.cc', 'src/core/frame/__getitem__.cc', 'src/core/frame/repr/widget.cc', 'src/core/frame/repr/text_column.cc', 'src/core/frame/repr/terminal_widget.cc', 'src/core/frame/repr/repr_options.cc', 'src/core/frame/repr/html_styles.cc', 'src/core/models/column_hasher.cc', 'src/core/models/dt_linearmodel.cc', 'src/core/models/column_caster.cc', 'src/core/models/dt_linearmodel_base.cc', 'src/core/models/py_linearmodel.cc', 'src/core/models/label_encode.cc', 'src/core/models/murmurhash.cc', 'src/core/models/utils.cc', 'src/core/models/dt_ftrl_base.cc', 'src/core/models/aggregate.cc', 'src/core/models/py_ftrl.cc', 'src/core/models/kfold.cc', 'src/core/models/dt_ftrl.cc', 'src/core/models/py_validator.cc', 'src/core/sort/sorter.cc', 'src/core/column/date_from_weeks.cc', 'src/core/column/latent.cc', 'src/core/column/cast_numeric.cc', 'src/core/column/pysources.cc', 'src/core/column/arrow_bool.cc', 'src/core/column/cast_to_bool.cc', 'src/core/column/cast_to_obj.cc', 'src/core/column/npmasked.cc', 'src/core/column/ifelsen.cc', 'src/core/column/virtual.cc', 'src/core/column/cast.cc', 'src/core/column/const_na.cc', 'src/core/column/arrow_str.cc', 'src/core/column/re_match.cc', 'src/core/column/arrow_fw.cc', 'src/core/column/view.cc', 'src/core/column/cast_to_time64.cc', 'src/core/column/cast_string.cc', 'src/core/column/sentinel_str.cc', 'src/core/column/ifelse.cc', 'src/core/column/cast_object.cc', 'src/core/column/nafilled.cc', 'src/core/column/string_slice.cc', 'src/core/column/sentinel_fw.cc', 'src/core/column/const.cc', 'src/core/column/date_from_years.cc', 'src/core/column/time_scaled.cc', 'src/core/column/repeated.cc', 'src/core/column/cast_to_date32.cc', 'src/core/column/string_plus.cc', 'src/core/column/range.cc', 'src/core/column/sentinel.cc', 'src/core/column/arrow_void.cc', 'src/core/column/column_impl.cc', 'src/core/column/rbound.cc', 'src/core/column/truncated.cc', 'src/core/column/cast_to_string.cc', 'src/core/column/date_from_months.cc', 'src/core/column/cast_date32.cc', 'src/core/column/cast_bool.cc', 'src/core/python/iter.cc', 'src/core/python/int.cc', 'src/core/python/list.cc', 'src/core/python/float.cc', 'src/core/python/date.cc', 'src/core/python/slice.cc', 'src/core/python/tuple.cc', 'src/core/python/namedtuple.cc', 'src/core/python/dict.cc', 'src/core/python/bool.cc', 'src/core/python/obj.cc', 'src/core/python/xargs.cc', 'src/core/python/set.cc', 'src/core/python/xobject.cc', 'src/core/python/range.cc', 'src/core/python/pybuffer.cc', 'src/core/python/args.cc', 'src/core/python/string.cc', 'src/core/python/arg.cc', 'src/core/read/constants.cc', 'src/core/read/input_column.cc', 'src/core/read/output_column.cc', 'src/core/read/py_fread.cc', 'src/core/read/multisource.cc', 'src/core/read/preframe.cc', 'src/core/read/parallel_reader.cc', 'src/core/read/chunk_coordinates.cc', 'src/core/read/thread_context.cc', 'src/core/read/py_read_iterator.cc', 'src/core/read/source.cc', 'src/core/read/parse_context.cc', 'src/core/read/fread/fread_parallel_reader.cc', 'src/core/read/fread/fread_thread_context.cc', 'src/core/read/parsers/parse_bool.cc', 'src/core/read/parsers/parse_float.cc', 'src/core/read/parsers/info.cc', 'src/core/read/parsers/ptype_iterator.cc', 'src/core/read/parsers/parse_string.cc', 'src/core/read/parsers/parse_void.cc', 'src/core/read/parsers/parse_date.cc', 'src/core/read/parsers/parse_int.cc', 'src/core/read/parsers/parse_time.cc', 'src/core/types/typeimpl.cc', 'src/core/types/type_object.cc', 'src/core/types/type.cc', 'src/core/types/typeimpl_numeric.cc', 'src/core/types/py_type.cc', 'src/core/types/type_string.cc', 'src/core/types/type_invalid.cc', 'src/core/types/type_bool.cc', 'src/core/types/type_time.cc', 'src/core/types/type_date.cc', 'src/core/types/type_void.cc', 'src/core/types/type_int.cc', 'src/core/types/type_float.cc', 'src/core/csv/toa.cc', 'src/core/csv/reader_arff.cc', 'src/core/csv/fread.cc', 'src/core/csv/reader_fread.cc', 'src/core/csv/reader.cc', 'src/core/progress/work.cc', 'src/core/progress/progress_manager.cc', 'src/core/progress/_options.cc', 'src/core/progress/progress_bar.cc', 'src/core/utils/alloc.cc', 'src/core/utils/exceptions.cc', 'src/core/utils/logger.cc', 'src/core/utils/fuzzy_match.cc', 'src/core/utils/misc.cc', 'src/core/utils/file.cc', 'src/core/utils/tests.cc', 'src/core/utils/wcwidth.cc', 'src/core/utils/temporary_file.cc', 'src/core/utils/terminal/tstring_impl.cc', 'src/core/utils/terminal/tstring_styled.cc', 'src/core/utils/terminal/tstring.cc', 'src/core/utils/terminal/terminal.cc', 'src/core/utils/terminal/tstring_plain.cc', 'src/core/utils/terminal/tstring_mixed.cc', 'src/core/utils/terminal/terminal_stream.cc', 'src/core/parallel/thread_pool.cc', 'src/core/parallel/parallel_for_dynamic.cc', 'src/core/parallel/job_shutdown.cc', 'src/core/parallel/thread_team.cc', 'src/core/parallel/job_idle.cc', 'src/core/parallel/parallel_for_ordered.cc', 'src/core/parallel/python_lock.cc', 'src/core/parallel/string_utils.cc', 'src/core/parallel/parallel_region.cc', 'src/core/parallel/thread_job.cc', 'src/core/parallel/thread_worker.cc', 'src/core/parallel/api_primitives.cc', 'src/core/tests/test_parallel_for.cc', 'src/core/tests/test_shared_mutex.cc', 'src/core/tests/test_parallel_for_ordered.cc', 'src/core/tests/test_barrier.cc', 'src/core/tests/test_atomic.cc', 'src/core/tests/test_progress.cc', 'src/core/str/split_into_nhot.cc', 'src/core/lib/hh/date.cc', 'src/core/lib/mman/mman.cc', 'src/core/lib/zlib/zutil.cc', 'src/core/lib/zlib/adler32.cc', 'src/core/lib/zlib/deflate.cc', 'src/core/lib/zlib/crc32.cc', 'src/core/lib/zlib/trees.cc']
      Using compiler of class xbuild.compiler.Compiler
      Using compiler gcc
      Added include directory 'src/core'
      Added include directory '/usr/local/include/python3.10'
      Output file name will be 'src/datatable/lib/_datatable.cpython-310-x86_64-linux-gnu.so'
      ==== BUILD ====
      [1] Loading previous state from file build/build/.xbuild
          The file does not exist
          All source files will be recompiled
      Traceback (most recent call last):
        File "/usr/local/lib/python3.10/site-packages/pip/_vendor/pep517/in_process/_in_process.py", line 156, in prepare_metadata_for_build_wheel
          hook = backend.prepare_metadata_for_build_wheel
      AttributeError: module 'ext' has no attribute 'prepare_metadata_for_build_wheel'
      
      During handling of the above exception, another exception occurred:
      
      Traceback (most recent call last):
        File "/usr/local/lib/python3.10/site-packages/pip/_vendor/pep517/in_process/_in_process.py", line 363, in <module>
          main()
        File "/usr/local/lib/python3.10/site-packages/pip/_vendor/pep517/in_process/_in_process.py", line 345, in main
          json_out['return_val'] = hook(**hook_input['kwargs'])
        File "/usr/local/lib/python3.10/site-packages/pip/_vendor/pep517/in_process/_in_process.py", line 160, in prepare_metadata_for_build_wheel
          whl_basename = backend.build_wheel(metadata_directory, config_settings)
        File "/tmp/pip-install-yj98d7rn/datatable_5170178362c243ada75fdc1ec0b0bf9d/ci/ext.py", line 587, in build_wheel
          so_file = build_extension(cmd=("debug" if debug_wheel else "build"),
        File "/tmp/pip-install-yj98d7rn/datatable_5170178362c243ada75fdc1ec0b0bf9d/ci/ext.py", line 360, in build_extension
          ext.build()
        File "/tmp/pip-install-yj98d7rn/datatable_5170178362c243ada75fdc1ec0b0bf9d/ci/xbuild/extension.py", line 439, in build
          self._run_prebuild_triggers()
        File "/tmp/pip-install-yj98d7rn/datatable_5170178362c243ada75fdc1ec0b0bf9d/ci/xbuild/extension.py", line 488, in _run_prebuild_triggers
          fn(self)
        File "/tmp/pip-install-yj98d7rn/datatable_5170178362c243ada75fdc1ec0b0bf9d/ci/ext.py", line 369, in generate_documentation
          import gendoc
      ModuleNotFoundError: No module named 'gendoc'
      [end of output]
  
  note: This error originates from a subprocess, and is likely not a problem with pip.
error: metadata-generation-failed

× Encountered error while generating package metadata.
╰─> See above for output.

note: This is an issue with the package mentioned above, not pip.
hint: See above for details.
```