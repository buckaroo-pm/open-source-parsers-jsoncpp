load('//:buckaroo_macros.bzl', 'buckaroo_deps')
load('//:subdir_glob.bzl', 'subdir_glob')

cxx_library(
  name = 'jsoncpp',
  header_namespace = '',
  exported_headers = subdir_glob([
    ('include', '**/*.h'),
  ]),
  srcs = glob([
    'src/lib_json/**/*.cpp',
  ]),
  deps = buckaroo_deps(),
  visibility = [
    'PUBLIC',
  ],
)
