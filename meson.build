project(
    'diffpdf', 'cpp',
    version: '3.0.0',
    default_options: [
        'cpp_std=c++17',
        'werror=true',
    ]    
)

add_project_arguments(
  '-Wno-sfinae-incomplete',
  language: 'cpp',
)

qt6 = import('qt6')
qt6_dep = dependency(
    'qt6',
    modules: [
        'Core',
        'Gui',
        'Widgets',
        'Core5Compat',
        'PrintSupport'
    ]
)

poppler_qt6_dep = dependency('poppler-qt6')

subdir('src')
subdir('resources')

executable(
    'diffpdf',
    [
        sources,
        mocs,
        translations,
        resources,
    ],
    dependencies: [
        qt6_dep,
        poppler_qt6_dep,
    ]
)