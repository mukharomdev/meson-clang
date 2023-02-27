## setup ##

project('meson-clang', 'c',
  version : '0.1',
  default_options : ['warning_level=3'])
# sources tracking
main_sources = []

# setup folder 
inc = include_directories('include')
subdir('include')
subdir('src')





## Target ##
exe = executable('meson_clang',
 main_sources,
 include_directories:inc,
 link_with:libtr,
  install : true)
## test ##
test('basic', exe)
