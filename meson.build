project(
    'libaco',
    'c',
    version: '1.0',
    default_options: ['warning_level=3'],
)

libco_sources  = [
    'libco.c',
]

libco = static_library(
    'libco',
    libco_sources,
    c_args: ['-fomit-frame-pointer', '-std=c89', '-O3', '-Wdeclaration-after-statement'],
)

libco_dep = declare_dependency(
    include_directories: include_directories('.'),
    link_with: libco,
)

subdir('doc/examples')
