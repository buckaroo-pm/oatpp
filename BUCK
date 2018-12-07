load('//:subdir_glob.bzl', 'subdir_glob')

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
  visibility = [
    'PUBLIC', 
  ], 
)
