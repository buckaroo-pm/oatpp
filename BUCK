load('//:subdir_glob.bzl', 'subdir_glob')
load('//:buckaroo_macros.bzl', 'buckaroo_deps_from_package')

cxx_library(
  name = 'oatpp', 
  header_namespace = 'oatpp', 
  exported_headers = glob([
    'algorithm/**/*.hpp', 
    'codegen/**/*.hpp', 
    'core/**/*.hpp', 
    'encoding/**/*.hpp', 
    'network/**/*.hpp', 
    'parser/**/*.hpp', 
    'web/**/*.hpp', 
  ]), 
  headers = glob([
    'test/**/*.hpp', 
  ]), 
  srcs = glob([
    'algorithm/**/*.cpp', 
    'core/**/*.cpp', 
    'encoding/**/*.cpp', 
    'network/**/*.cpp', 
    'parser/**/*.cpp', 
    'web/**/*.cpp', 
  ]), 
  platform_deps = [
    ('linux.*', buckaroo_deps_from_package('github.com/buckaroo-pm/host-pthread')), 
  ], 
  visibility = [
    'PUBLIC', 
  ], 
)
